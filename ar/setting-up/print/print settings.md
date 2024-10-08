---
description: print settings
---

# إعدادات الطباعة

### إعدادات الطباعة

**في إعدادات الطباعة ، يمكنك تعيين تفضيلات الطباعة مثل حجم الورق ، وحجم النص الافتراضي ، سواء كنت تريد الإخراج بتنسيق PDF أو HTML ، وما إلى ذلك.**

نظرًا لأن ERPNext هو تطبيق قائم على المستعرض ، يتم تنفيذ أمر الطباعة الفعلي بواسطة المتصفح الذي تستخدمه.

لتحرير إعدادات الطباعة ، انتقل إلى:

> الصفحة الرئيسية> الإعدادات> إعدادات الطباعة

![إعدادات الطباعة](https://docs.erpnext.com/files/print-settings.png)

هناك العديد من التكوينات المتوفرة في Print Settings (إعدادات الطباعة). دعونا نتعلم عنهم.

### 1. إعدادات PDF

#### 1.1 PDF أو HTML

عند إرسال أي مستند بالبريد الإلكتروني (مثل أمر المبيعات / الفاتورة) من ERPNext ، يتم إرساله بتنسيق PDF أو HTML. يتم إرسال الملف بشكل افتراضي بتنسيق PDF. إذا كنت ترغب في إرسال مستند بتنسيق HTML ، فما عليك سوى إلغاء تحديد الخيار "إرسال طباعة بتنسيق PDF".

#### 1.2 كرر الرأس والتذييل في PDF

ورقة ذات رأسية رئيسية حيث يمكنك تحديد رأس وتذييل قياسي يتم إلحاقه بتنسيق طباعة المستند. إذا تم تمكين هذه الخاصية ، فسيتم إضافة رأس وتذييل إلى كل صفحة. إذا كنت لا تريد تكرار رأس الصفحة وتذييلها في كل صفحة ، فما عليك سوى تعطيل هذا الإعداد.

#### 1.3 حجم صفحة PDF

الحجم الافتراضي لطباعة صفحات PDF هو A4 ، ويمكنك اختيار أي حجم من الخيارات المحددة [هنا](https://doc.qt.io/archives/qt-4.8/qprinter.html#PaperSize-enum) ، بما في ذلك الأبعاد المخصصة المحددة بالمليمترات.

### 2. إعدادات الصفحة

#### 2.1 طباعة مع ورقة ذات رأسية

سيؤدي تمكين هذه الخاصية إلى تحديد خيار Letter Head تلقائيًا عند طباعة مستند. لاحظ أنك تحتاج إما إلى تعيين Letter Head كإعداد افتراضي أو تحديد واحد في المعاملة حتى يظهر في عرض الطباعة.

#### 2.2 طباعة عنصر مضغوط

تحتوي المعاملات مثل أوامر المبيعات / الفواتير على جدول يوضح بالتفصيل العناصر التي تم شراؤها أو بيعها. يحتوي على أعمدة متعددة مثل اسم العنصر ، والوصف ، ووحدة القياس ، ومبلغ السعر ، وما إلى ذلك. إذا كان هناك العديد من الأعمدة في جدول العناصر ، فإن تنسيق الطباعة يبدو مشوشًا بعض الشيء. يمكنك تحسين عرض الجدول عن طريق تمكين طباعة العنصر المضغوط.

وفقًا لهذا الإعداد ، سيكون هناك أربعة أعمدة فقط في تنسيق الطباعة ، وهي: الوصف والكمية والمعدل والمبلغ.

قيم الأعمدة الأخرى (مثل الاسم والوصف والصورة والأرقام التسلسلية وما إلى ذلك) متسلسلة في عمود الوصف.

عندما لا يتم تحديد مربع الاختيار ، يبدو تنسيق الطباعة كما يلي:![Incompact Print Format Settings](https://docs.erpnext.com/files/incompact-print.png)

هذا ما يبدو عليه تنسيق الطباعة المضغوطة:![إعدادات تنسيق الطباعة المضغوطة](https://docs.erpnext.com/files/compact-print.png)

#### 2.3 السماح بطباعة المسودة

تحتوي المستندات (معظمها معاملات) على مرحلتين من المصادقة ، حفظ وإرسال. المستندات المحفوظة هي المسودة الأولى ولم يتم إرسالها إلى النظام. ومن ثم فإن الطباعة مقيدة للمستندات في هذه المرحلة. ومع ذلك ، إذا كنت ترغب في السماح للمستخدمين بطباعة المستندات في مرحلة المسودة أيضًا ، فقم بتمكين مربع الاختيار هذا.

#### 2.4 أضف دائمًا عنوان "مسودة" لطباعة مسودات المستندات

يؤدي تمكين هذا الإعداد أيضًا إلى طباعة "مسودة" بتنسيق الطباعة ، مما يشير إلى أن المستند المشترك لم تتم مصادقته بالكامل بعد.

#### 2.5 السماح باستراحة الصفحة داخل الجدول

إذا كان وصف عنصر ما يلتقط مساحة أكبر من المعتاد في الصفحة ، فإن تمكين هذا الإعداد سيؤدي إلى تقسيم تفاصيل العنصر إلى الصفحة التالية. ومن ثم ، سيتم إدراج فاصل صفحة بين وصف العنصر ، وسيتم دفع باقي التفاصيل إلى الصفحة التالية.

#### 2.6 السماح بإلغاء الطباعة

المعاملات الملغاة هي المعاملات التي ليس لها أي تأثير على التقارير. إذا كنت ترغب في السماح بطباعة المعاملات الملغاة ، فقم بتمكين هذا الإعداد. لا يمكن إلغاء الصفقة إلا بعد تقديمها.

#### 2.7 طباعة الضرائب بالمبلغ الصفري

في معاملات البيع والشراء ، يمكنك إضافة تطبيق ضرائب متعددة على الصنف. بشكل افتراضي ، في تنسيق الطباعة ، تظهر فقط الضرائب التي تم حساب بعض المبالغ فيها. إذا كنت ترغب أيضًا في طباعة الضريبة التي لم يتم تطبيقها والتي لا تحتوي على مبلغ ضريبي ، فقم بتمكين هذا الإعداد.

### 3. طابعة الشبكة / خادم الطباعة

يمكنك تمكين خادم الطباعة عن طريق ملء عنوان IP الخاص بخادم الطباعة والمنفذ. ثم اختر الطابعة الافتراضية.

قبل تمكين هذه الميزة ، يجب عليك تثبيت مكتبة "pycups".

قد تحتاج أولاً إلى تثبيت مكتبة "cups" إذا لم تكن موجودة بالفعل على نظامك

لعائلة نظام تشغيل دبيان:

`sudo apt-get install libcups2-dev`

لعائلة Red Hat OS:

"sudo yum install cups-libs"

بعد ذلك ، قم بتثبيت "pycups" في env باستخدام الأمر:

"./env/bin/pip تثبيت pycups\`

يتم تنفيذ ذلك من دليل "frappe-bench".

### 4. طباعة خام

يمكنك تمكين الطباعة الأولية والطباعة للعديد من الطابعات الحرارية المدعومة. اقرأ [الطباعة الأولية](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/raw-printing) لمعرفة المزيد.

1. [تنسيق الطباعة](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-format)
2. [نمط الطباعة](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-style)
3. [عناوين الطباعة](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-headings)
4. [ترجمات مخصصة](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/custom-translations)
