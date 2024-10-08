# appraisal

\n**التقييم هو عملية يتم من خلالها توثيق أداء الموظف وتقييمه.**

لإنشاء دورة تقييم ، انتقل إلى:

> الصفحة الرئيسية> الموارد البشرية> الأداء> التقييم

### 1. المتطلبات الأساسية

قبل إنشاء التقييم ، يجب عليك إنشاء ما يلي:

* [نموذج التقييم](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/appraisal-template)
* [دورة التقييم](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/appraisal-cycle)

### 2. كيفية إنشاء التقييم

يمكن إنشاء التقييمات بشكل مجمّع من [دورة التقييم](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/appraisal-cycle).

ومع ذلك ، إذا كنت تريد إنشاء تقييم يدويًا ، فإليك الخطوات:

1. اذهب إلى قائمة التقييم ، وانقر على جديد.
2. حدد الموظف
3. حدد دورة التقييم.
4. إذا تم تعيين نموذج التقييم للموظف بالفعل في الجدول الفرعي للموظفين في الدورة ، فسيتم جلبه تلقائيًا. عدا ذلك ، يمكنك تحديد قالب للموظف. يحفظ.

### 3. سمات

#### 3.1 تقييم KRA

استنادًا إلى طريقة تقييم KRA المحددة في [دورة التقييم](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/appraisal-cycle) ستكون إحدى العمليات التالية قابلة للتطبيق :

**3.1.1 آلي بناءً على تقدم الهدف**

هذه هي طريقة تقييم KRA الافتراضية.

في هذه الطريقة ، يمكنك إنشاء أهداف وأهداف فرعية تتوافق مع KRAs الخاصة بك.

سيكون جدول KRA vs Goals مرئيًا في مستند التقييم الخاص بك.

\***KRA والوزن**: تم جلبها من نموذج التقييم \***إكمال الهدف (٪)**: سيتم احتساب نسبة إكمال الهدف تلقائيًا بناءً على**التقدم**للأهداف المرتبطة بـ KRAs الخاصة بك. \***نتيجة الهدف (مرجحة)**: بناءً على الوزن المخصص لكل KRA ، سيتم حساب درجة الهدف من نسبة الإنجاز. على سبيل المثال: في لقطة الشاشة أدناه ، يمتلك Development KRA وزنًا بنسبة 30٪ وأكمل الموظف 75٪ من الأهداف. لذا فإن نتيجة الهدف هي 22.5 من 30 ، وهكذا.

ستحصل أخيرًا على**إجمالي نقاط الهدف**(من 5) بناءً على**درجة الهدف (٪)**.

![kra vs Goals](https://docs.erpnext.com/files/kra-vs-goals.png)

**3.1.2 التصنيف اليدوي**

يمكنك اختيار تقييم الأهداف / KRAs يدويًا. هذه هي طريقة التقييم الأصلية المستخدمة حتى الإصدار 13.

1. بناءً على النموذج المحدد ، سيتم جلب KRAs في قسم الأهداف.
2. أدخل النتيجة (0-5) لكل KRA.
3. بناءً على الوزن المذكور ، سيتم احتساب**الدرجة المكتسبة**لكل KRA.
4. حفظ.

بناءً على الدرجة المكتسبة لكل KRA ، سيحسب النظام إجمالي الدرجات (من 5) للموظف.

![التصنيف اليدوي](https://docs.erpnext.com/files/manual-rating.png)

#### 3.2 الملاحظات

يتم تسجيل تعليقات أداء الموظف في [ملاحظات أداء الموظف](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/employee-performance-feedback) DocType.

ولكن للحصول على نظرة عامة على أداء الموظف ، يمكنك الاطلاع على سجل جميع التعليقات التي تلقاها الموظف في الدورة ضمن علامة التبويب "التعليقات".

يمكنك الاطلاع على ملخص التقييم بمتوسط ​​درجة التعليقات ، وعدد المراجعات ، والتوزيع النسبي للنجوم التي حصل عليها الموظف.

![سجل التعليقات](https://docs.erpnext.com/files/feedback-history.png)

> ملاحظة: فقط مستندات الملاحظات المرسلة تكون مرئية في هذا المحفوظات ويكون العرض حساسًا للإذن.

في كل مراجعة ، يمكنك رؤية المراجع وتعيينه ومتوسط ​​التقييم الممنوح للموظف والتعليقات والوقت الذي تم فيه تقديم التعليقات. يمكنك أيضًا النقر فوق رمز الارتباط لرؤية مستند ملاحظات أداء الموظف بالكامل.

![رابط التعليقات](https://docs.erpnext.com/files/feedback-link.png)

إذا كانت لديك الأذونات المطلوبة ، فيمكنك إرسال ملاحظات الأداء مباشرةً من طريقة العرض هذه بالنقر فوق الزر**تعليقات جديدة**.

![إضافة تعليق](https://docs.erpnext.com/files/add-feedback.png)

#### 3.3 التقييم الذاتي

ضمن علامة التبويب التقييم الذاتي ، يمكن للموظفين تقييم أنفسهم وإضافة انعكاسات على أدائهم. يتم احتساب إجمالي الدرجات الذاتية بناءً على التصنيف والوزن مقابل كل معيار من معايير الملاحظات.

![تقييم ذاتي](https://docs.erpnext.com/files/self-appraisal.png)

#### 3.4 حساب النتيجة النهائية

يتم احتساب النتيجة النهائية كمتوسط ​​نقاط الهدف ، ومتوسط ​​نقاط التقييم ، ودرجة التقييم الذاتي.

![النتيجة النهائية](https://docs.erpnext.com/files/final-score.png)

#### 3.5 عرض الأهداف

يمكنك عرض أهداف الموظف المرتبطة بدورة التقييم هذه من خلال النقر على زر عرض الأهداف:

![تقييم الأهداف](https://docs.erpnext.com/files/goals-appraisal.png)

#### 3.6 الموافقات للتقييم

أخيرًا ، بمجرد حصولك على جميع التعليقات والأهداف المحدثة والتقييم الذاتي في وثيقة التقييم ، يمكنك إرسالها.

يمكنك أيضًا إعداد [Workflow](https://docs.erpnext.com/docs/v14/user/manual/en/setting-up/workflows) للموافقات قبل إرسال التقييم.

1. [الهدف](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/goal)
2. [ملاحظات أداء الموظف](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/employee-performance-feedback)
