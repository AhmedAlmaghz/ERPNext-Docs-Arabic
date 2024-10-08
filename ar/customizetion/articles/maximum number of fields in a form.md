---
description: maximum number of fields in a form
---

# الحد الأقصى لعدد الحقول في النموذج

في بعض الأحيان أثناء إنشاء حقول مخصصة ، ربما واجهت رسالة خطأ تبدو كالتالي:

> حجم الصف كبير جدًا. الحد الأقصى لحجم الصف لنوع الجدول المستخدم ، دون احتساب كائنات التخزين الثنائية الكبيرة ، هو 65535. وهذا يشمل سعة التخزين ، راجع الدليل. يجب عليك تغيير بعض الأعمدة إلى TEXT أو BLOBs.

#### ماذا يعني ذلك؟

بعبارات بسيطة ، فهذا يعني أنك وصلت إلى الحد الأقصى لعدد الحقول للنموذج / نوع المستند المحدد. إذن ، ما هو الحد الأقصى للحقول؟

في MySQL ، يوجد حد صارم يبلغ 4096 عمودًا لكل جدول ، ولكن الحد الأقصى الفعال قد يكون أقل بالنسبة لجدول معين. يعتمد الحد الدقيق على عدة عوامل متفاعلة.

كل جدول (بغض النظر عن محرك التخزين) له حجم صف أقصى يبلغ 65.535 بايت. قد تضع محركات التخزين قيودًا إضافية على هذا الحد ، مما يقلل من الحد الأقصى الفعال لحجم الصف.

يقيد الحد الأقصى لحجم الصف عدد الأعمدة (وربما حجمها) لأن الطول الإجمالي لجميع الأعمدة لا يمكن أن يتجاوز هذا الحجم (65.535 بايت). على سبيل المثال ، تتطلب أحرف `utf8mb3` ما يصل إلى 3 بايت لكل حرف ، لذلك بالنسبة لعمود`VARCHAR (140)`، يجب على الخادم تخصيص `140 × 3 = 420` بايت لكل قيمة. وبالتالي ، لا يمكن أن يحتوي الجدول على أكثر من "65.535 / 420 = 156" من هذه الأعمدة.

في إطار عمل Frappe ، يتم إنشاء أعمدة نوع `VARCHAR (140)` بناءً على أنواع الحقول "البيانات" و "الرابط" و "تحديد" و "الرابط الديناميكي" و "كلمة المرور" و "للقراءة فقط". وبالتالي ، يمكنك إنشاء ما يقرب من 156 عمودًا من هذا القبيل في النظام.

#### حل:

لإضافة المزيد من الحقول إلى النظام ، يمكنك إجراء بعض التغييرات.

1. قم بتحويل بعض الحقول إلى حقل نوع "نص" أو "نص صغير" أو "محرر نص" أو "رمز". في MySQL ، يتم احتساب أعمدة BLOB و TEXT من واحد إلى أربعة زائد ثمانية بايت لكل منها نحو حد حجم الصف لأن محتوياتها يتم تخزينها بشكل منفصل عن باقي الصف. لذا ، فإن التحويل إلى هذه الأنواع من الحقول سيوفر بعض المساحات ويسمح بإضافة المزيد من الحقول.
2. عيّن قيمة أصغر في خاصية "الطول" أثناء إنشاء الحقول ، القيمة الافتراضية هي 140. يعيّن النظام طول "VARCHAR" بناءً على هذه الخاصية ويخصص حجمًا لتلك الأعمدة. وبالتالي ، يؤدي الطول الأصغر إلى إضافة المزيد من الحقول.
