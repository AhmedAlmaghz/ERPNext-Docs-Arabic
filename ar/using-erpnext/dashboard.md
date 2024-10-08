## لوحة القيادة

> مقدمة في الإصدار 12

**توفر لوحة المعلومات نظرة سريعة على مؤشرات الأداء الرئيسية ذات الصلة بعملية الأعمال.**

تتكون كل لوحة معلومات من مخطط واحد أو أكثر من مخططات لوحة المعلومات ، تم تكوين كل منها باستخدام مصدر بيانات يُعرف باسم مصدر مخطط لوحة المعلومات.

للوصول إلى لوحة التحكم ، انتقل إلى ،

> الصفحة الرئيسية> التخصيص> لوحات المعلومات> لوحة المعلومات

## 1. كيفية إنشاء لوحة تحكم جديدة

1. اذهب إلى قائمة لوحات المعلومات وانقر على جديد.
2. أدخل اسم الوحدة النمطية التي تريد رؤية لوحة المعلومات الخاصة بها.
3. أدخل مخططات لوحة المعلومات التي تريد أن تكون معلمات للوحة المعلومات هذه.
4. حفظ.

عند النقر فوق "إظهار لوحة التحكم" ، ستتمكن من رؤية لوحة المعلومات التي تقدم تمثيلاً رسوميًا لمعاملاتك.

![لوحة بيانات المحاسبة](https://docs.erpnext.com/files/dashboard.png)

## 2. إضافة الرسوم البيانية إلى لوحة القيادة

أضف المخططات إلى لوحة التحكم هذه إما عن طريق تحديد "مخطط لوحة المعلومات" الحالي أو إنشاء مخططات جديدة.

![إضافة لوحة التحكم إلى الرسوم البيانية](https://docs.erpnext.com/files/dashboard-add-charts.png)

احفظ التغييرات وانقر على زر "إظهار لوحة التحكم" لرؤية لوحة القيادة.

![إظهار زر لوحة التحكم](https://docs.erpnext.com/files/dashboard-show-dashboard-button.png)

## 3. إنشاء مخطط لوحة معلومات جديد

لإنشاء مخطط لوحة معلومات جديد ، انتقل إلى

> الصفحة الرئيسية> التخصيصات> لوحات المعلومات> مخطط لوحة المعلومات> جديد

أدخل اسمًا للمخطط ، وسيظهر هذا في لوحة المعلومات كتسمية المخطط ، وحدد نوع المخطط كـ "مخصص" وحدد "مصدر مخطط لوحة المعلومات" كمصدر بيانات لهذا المخطط.

**ملاحظة:**لا يمكن إنشاء "مصدر مخطط لوحة المعلومات" الجديد إلا بواسطة المستخدم المسؤول في وضع المطور.

![حدد مصدر مخطط لوحة التحكم](https://docs.erpnext.com/files/dashboard-chart-from-source.png)

بعد تعيين حقل مصدر المخطط ، سيظهر جدول عوامل التصفية.

انقر فوق الجدول لتحرير عوامل التصفية.

![عامل تصفية مخطط لوحة التحكم](https://docs.erpnext.com/files/dashboard-chart-filter.png)

سيظهر مشروط لضبط المرشحات. انقر فوق "تعيين" لتعيين عوامل التصفية. ![نموذج عامل تصفية مخطط لوحة التحكم](https://docs.erpnext.com/files/dashboard-chart-filter-modal.png)

بعد تعيين حقل مصدر المخطط ، سيتم تحديث جدول عوامل التصفية بقيم عامل التصفية المحددة. ![عامل تصفية مخطط لوحة التحكم](https://docs.erpnext.com/files/dashboard-chart-filter-updated.png)

في المثال أعلاه ، أنشأنا "مخطط لوحة معلومات" مخصصًا كان لدينا بالفعل "مصدر مخطط لوحة المعلومات".

يمكنك أيضًا إنشاء مخططات أساسية مثل العدد / المجموع / المتوسط ​​/ المجموعة حسب المهام بناءً على تاريخ الإنشاء / التعديل عن طريق تحديد "العدد / المجموع / المتوسط ​​/ المجموعة حسب" كـ "نوع المخطط" كما يمكنك استخدام تقرير موجود كمصدر في الحقل "اسم التقرير" لإنشاء مخطط عن طريق تحديد "تقرير" على أنه "نوع المخطط".

بالنسبة إلى "Count" ، تحتاج إلى تحديد "Doctype" الذي تحتاج إلى الرسم البياني له في الحقل "Document Type" والحقل "Based On Date" في "Time Series Based On".

![مخطط لوحة التحكم](https://docs.erpnext.com/files/dashboard-chart-count.png)

**ملاحظة:**إذا قمت بتحديد نوع مستند لجدول فرعي في "نوع المستند" ، فيجب عليك أيضًا تحديد نوع المستند الأصلي لهذا الجدول الفرعي في "نوع المستند الأصلي" (لن يكون هذا الحقل مرئيًا إلا عند تحديد نوع مستند الجدول الفرعي في حقل "نوع المستند").

![نوع المستند الأصل لمخطط لوحة التحكم الرئيسية](https://docs.erpnext.com/files/dashboard-chart-parent-document-type.png)

بالنسبة إلى "المجموع" و "المتوسط" ، يتعين عليك أيضًا تحديد الحقل "استنادًا إلى القيمة" في "استنادًا إلى القيمة".

![مخطط لوحة معلومات المجموع](https://docs.erpnext.com/files/dashboard-chart-sum.png)

بالنسبة إلى "تجميع حسب" ، يمكنك تحديد "تجميع حسب النوع" كعدد / مجموع / متوسط ​​، و "تجميع حسب استنادًا إلى" كما تم الإنشاء بواسطة / معدَّل بواسطة ، و "عدد المجموعات".

![تجميع حسب مخطط لوحة التحكم](https://docs.erpnext.com/files/dashboard-chart-group-by.png)

## 4. باستخدام لوحات القيادة

سيتم عرض كل مخطط وفقًا للحقول المحددة في مخطط لوحة المعلومات المقابل. يتم تخزين النتيجة من مصدر مخطط لوحة المعلومات مؤقتًا لتجنب الاستعلامات المتكررة. نظرًا لأن بيانات المخطط يمكن أن تكون قديمة ، سيعرض كل مخطط أيضًا آخر وقت تمت مزامنته.

![آخر مزامنة للوحة البيانات](https://docs.erpnext.com/files/dashboard-last-synced.png)

يمكن أيضًا تغيير عوامل التصفية المستخدمة لإنشاء بيانات الرسم البياني بالنقر فوق "تعيين عوامل التصفية". سيتم تحديث الرسم البياني تلقائيًا وفقًا لعوامل التصفية التي تم تعيينها مؤخرًا.

![عوامل تصفية لوحة التحكم](https://docs.erpnext.com/files/dashboard-filters.png)

للحصول على أحدث البيانات ، يجب تحديث كل مخطط بقوة من خلال النقر فوق الزر**فرض التحديث**من القائمة المنسدلة.