\nالعناصر التي يتم الاحتفاظ برقم المسلسل ورقم الدُفعة لها ، ويتم تحديث إدخال رصيد المخزون المفتوح لها عن طريق إدخال المخزون. [انقر هنا لمعرفة كيفية إدارة المخزون المتسلسل في ERPNext](https://docs.erpnext.com/docs/v13/user/manual/en/stock/serial-no.html).

**السؤال:**لماذا لا يمكن تحديث إدخال الرصيد الافتتاحي للبند المسلسل والدُفعي من خلال تسوية المخزون؟

في ERPNext ، يتم اشتقاق مستوى المخزون الخاص بالعنصر المتسلسل بناءً على عدد الأرقام التسلسلية لهذا العنصر. وبالتالي ، ما لم يتم إنشاء الأرقام التسلسلية للصنف المتسلسل ، فلن يتم تحديث مستوى المخزون الخاص به. في أداة تسوية المخزون ، يمكنك فقط تحديث الكمية الافتتاحية لعنصر ما ، ولكن ليس الرقم التسلسلي ورقم الدُفعة.

### الرصيد الافتتاحي للسلعة المسلسلة

فيما يلي خطوات إنشاء إدخال رصيد المخزون الافتتاحي للبند المسلسل والدُفعي.

#### الخطوة 1: إدخال مخزون جديد

"مخزون> إدخال مخزون> جديد"

#### الخطوة 2: حدد الغرض

يجب تحديث غرض إدخال المخزون على أنه "استلام المواد".

#### الخطوة الثالثة: تحديث تاريخ النشر

يجب أن يكون تاريخ الإرسال هو التاريخ الذي ترغب في تحديث الرصيد الافتتاحي فيه لأحد العناصر.

#### الخطوة الرابعة: تحديث المستودع المستهدف

سيكون المستودع المستهدف هو المستودع الذي سيتم فيه تحديث الرصيد الافتتاحي للعنصر.

#### الخطوة 5: حدد العناصر

حدد العناصر التي سيتم تحديث الرصيد الافتتاحي لها.

#### الخطوة 6: تحديث فتح الكمية

بالنسبة إلى العنصر المتسلسل ، قم بتحديث الكمية حيث أن العديد من الأرقام المسلسلة هي.

بالنسبة إلى العنصر المتسلسل ، اذكر الأرقام التسلسلية المكافئة للكمية. أو إذا تم تكوين الأرقام المسلسلة ليتم إنشاؤها استنادًا إلى البادئة ، فلا داعي لذكر الأرقام المسلسلة يدويًا. انقر [هنا](https://docs.erpnext.com/docs/v13/user/manual/en/stock/articles/serial-no-naming.html) لمعرفة المزيد حول تسمية الرقم التسلسلي.

بالنسبة لصنف الدُفعة ، قم بتوفير معرف الدُفعة الذي سيتم فيه تحديث الرصيد الافتتاحي. احتفظ بدفعة رئيسية جاهزة ، وقم بتحديثها لعنصر الدُفعة. لإنشاء دفعة جديدة ، انتقل إلى:

"مخزون> إعداد> دفعة> جديد"

[انقر هنا لمعرفة كيفية إدارة مخزون Batchwise في ERPNext.](https://docs.erpnext.com/docs/v13/user/manual/en/stock/articles/managing-batch-wise-inventory.html)

#### الخطوة 7: تحديث معدل تقييم السلعة

تحديث معدل التقييم ، والذي سيكون حسب قيمة الوحدة للعنصر. إذا كانت الوحدات المختلفة من نفس العناصر لها معدل تقييم مختلف ، فيجب تحديثها في صف منفصل ، بمعدلات تقييم مختلفة.

#### الخطوة 8: حساب الفرق

وفقًا لنظام تقييم المخزون الدائم ، يتم إنشاء إدخال محاسبي لكل حركة مخزون. يتطلب نظام محاسبة القيد المزدوج مطابقة إجمالي الخصم مع إجمالي الائتمان في الإدخال. عند تقديم إدخال المخزون ، يقوم النظام بخصم حساب المستودع حسب القيمة الإجمالية للأصناف. لتحقيق التوازن ، نستخدم حساب الفتح المؤقت كحساب فرق.

![حساب الفرق](https://docs.erpnext.com/files/difference-account-1.png)

#### الخطوة التاسعة: حفظ إدخال المخزون وإرساله

عند تقديم إدخال المخزون ، سيتم ترحيل ترحيل دفتر الأستاذ ، وسيتم تحديث الرصيد الافتتاحي للعناصر في تاريخ ترحيل معين.