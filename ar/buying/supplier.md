## المورد

**الموردون هم شركات أو أفراد يقدمون لك منتجات أو خدمات.**

للوصول إلى قائمة الموردين ، انتقل إلى:

> الصفحة الرئيسية> الشراء> المورد> المورد

## 1. كيفية إنشاء مورد

1. اذهب إلى قائمة الموردين وانقر على جديد.
2. أدخل اسمًا للمورد.
3. حدد مجموعة الموردين سواء أكانت أدوية أم أجهزة وما إلى ذلك.
4. حفظ. ![مدير المورد](https://docs.erpnext.com/files/supplier-master.png)

ستتوفر خيارات Warn RFQs و POs و Prevent RFQs و POs بمجرد إنشاء [بطاقة نقاط المورد](https://docs.erpnext.com/docs/v13/user/manual/en/buying/supplier-scorecard) ويتم إجراء المعاملات.

## 2. سمات

سيتم ملء الحقول في المعاملات المستقبلية تلقائيًا إذا تم تعيين الحقول "الافتراضية" مثل الحساب المصرفي الافتراضي ونموذج شروط الدفع الافتراضية وما إلى ذلك في المورد.

### 2.1 التفاصيل الضريبية

***الدولة**: إذا كان المورد من دولة أخرى ، يمكنك تغييره هنا.
***المعرف الضريبي**: رقم التعريف الضريبي للمورد.
***فئة الضريبة**: هذا مرتبط بـ [القاعدة الضريبية](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/tax-rule). إذا تم تعيين فئة ضريبة هنا ، عند تحديد هذا المورد ، فسيتم تطبيق نموذج ضريبة الشراء والرسوم ذات الصلة. هذا القالب مرتبط بالقاعدة الضريبية وقاعدة الضرائب مرتبطة بفئة ضريبية. يمكن استخدام فئة الضريبة لتجميع الموردين الذين سيتم تطبيق نفس الضريبة عليهم. على سبيل المثال: حكومية ، تجارية ، إلخ.
***لغة الطباعة**: اللغة التي سيتم طباعة المستند بها.
***فئة الاستقطاع الضريبي**: بالنسبة للهند ، فئة المواد الصلبة الذائبة للمورد. عند تعيين فئة هنا ، سيتم جلبها في [فاتورة الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/purchase-invoice). لمزيد من المعلومات ، تفضل بزيارة صفحة [فئة الاستقطاع الضريبي](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/tax-withholding-category).
***معطل**: يعطل المورد ولن يتم عرضه في قائمة الموردين.
***ناقل**: إذا كان المورد يبيع خدمات النقل الخاصة بك ، فحدد هذا المربع. سيكون حقل "معرّف ناقل ضريبة السلع والخدمات" مرئيًا إذا تم تحديد هذا الحقل.
***المورد الداخلي**: إذا كان المورد من شركة شقيقة أو أم / شركة فرعية ، حدد هذا الحقل وحدد الشركة التي يمثلونها.

للهند:

***فئة ضريبة السلع والخدمات**: حدد فئة ضريبة السلع والخدمات للمورد.
***PAN**: للهند ، تفاصيل بطاقة PAN (رقم الحساب الدائم) للمورد.

### 2.2 السماح بإنشاء فاتورة الشراء بدون أمر الشراء وإيصال الشراء

إذا تم تكوين الخيار "أمر الشراء مطلوب" أو "إيصال الشراء مطلوب" على أنه "نعم" في [إعدادات الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/buying/buying- الإعدادات) ، يمكن تجاوزها لمورد معين عن طريق تمكين "السماح بإنشاء فاتورة الشراء بدون أمر شراء" أو "السماح بإنشاء فاتورة الشراء بدون إيصال شراء" في مدير المورد.

![مدير المورد](https://docs.erpnext.com/files/supplier-po-pr-required.png)

### 2.3 قائمة العملات والأسعار

**عملة الفوترة**: يمكن أن تختلف عملة المورد الخاص بك عن عملة شركتك. إذا اخترت الين الياباني لأحد الموردين ، فسيتم ملء العملة بالين الياباني وسعر الصرف المعروض لمعاملات الشراء المستقبلية.

![عملة المورد](https://docs.erpnext.com/files/supplier-currency.gif)

يمكن أن يكون لكل مورد**قائمة أسعار**افتراضية بحيث يتم تحديث قائمة الأسعار المرتبطة بالمورد أيضًا في كل مرة تشتري فيها عنصرًا جديدًا من هذا المورد بأسعار مختلفة. تحت قائمة الأسعار يأتي سعر العنصر ، يمكنك رؤية الأسعار في الشراء> العناصر والتسعير> سعر العنصر.

إذا حددت هذا المورد المعين ، فسيتم جلب قائمة الأسعار المرتبطة في معاملات الشراء.

### 2.4 حد الائتمان

***قالب شروط الدفع الافتراضية**: إذا تم تعيين قالب شروط الدفع هنا ، فسيتم تحديده تلقائيًا لمعاملات الشراء المستقبلية.
***حظر المورد**: يمكنك حظر الفواتير أو المدفوعات أو كليهما من المورد حتى تاريخ محدد. اختر "نوع الحجز" ، إذا لم تحدد نوع الحجز ، فسيقوم ERPNext بتعيينه على "الكل". عندما يتم حظر مورد ، ستظهر حالته على أنها "قيد الانتظار".
    
    أنواع الحجز هي كما يلي:
    
    * الفواتير: لن يسمح ERPNext بإنشاء فواتير الشراء أو أوامر الشراء للمورد
    * المدفوعات: لن يسمح ERPNext بإنشاء إدخالات الدفع للمورد
    * الكل: سيطبق ERPNext كلا نوعي التعليق أعلاه
    
    إذا لم تحدد تاريخ إصدار ، فستحتفظ ERPNext بالمورد**إلى أجل غير مسمى**.
    

### 2.5 حسابات الدفع الافتراضية

أضف الحساب الافتراضي الذي سيتم من خلاله دفع الفواتير لهذا المورد. أضف صفوفًا إضافية لمزيد من الشركات ، يمكنك تحديد حساب واحد فقط لكل شركة.

يمكنك**دمج**مورد مع حساب. بالنسبة لجميع الموردين ، تم تعيين حساب "الدائن" كحساب الدفع الافتراضي. عند إنشاء فاتورة الشراء ، يتم حجز المدفوعات المستحقة للمورد مقابل حساب "الدائنين".

إذا كنت ترغب في تخصيص حساب الدفع للمورد ، فيجب عليك أولاً إضافة حساب مستحق الدفع في مخطط الحساب ، ثم تحديد حساب الدفع هذا في مدير المورد.

![مدير المورد](https://docs.erpnext.com/files/supplier-payable-account.png)

إذا كنت لا ترغب في تخصيص حساب الدفع ، والمتابعة مع حساب الدفع الافتراضي "الدائن" ، فلا تقم بتحديث أي قيمة في جدول حساب المورد الافتراضي.

> نصيحة: تم تعيين حساب الدفع الافتراضي في مدير الشركة. إذا كنت ترغب في تعيين حساب آخر كحساب افتراضي للدفع بدلاً من حساب الدائنين ، فانتقل إلى مدير الشركة ، وقم بتعيين هذا الحساب على أنه "حساب الدفع الافتراضي".

بناءً على [خطتك](https://erpnext.com/pricing) ، يمكنك إضافة شركات متعددة في مثيل ERPNext الخاص بك. يمكن استخدام مورد واحد عبر عدة شركات. في هذه الحالة ، يجب عليك تحديد حساب المدفوعات من جانب الشركة للمورد في جدول "حسابات المدفوعات الافتراضية" ، أي إضافة صفوف متعددة.

### 2.6 مزيد من المعلومات

يمكنك إضافة موقع المورد وأي تفاصيل إضافية حول المورد الخاص بك في هذا القسم. إذا قمت بتجميد مورد باستخدام الخيار "Is Frozen" ، فسيتم تجميد قيود المحاسبة الخاصة بالمورد. في هذه الحالة ، المستخدم الوحيد الذي ستتجاوز إدخالاته "التجميد" هو الدور المعين في "الدور المسموح به لتعيين الحسابات المجمدة وتحرير الإدخالات المجمدة" في المحاسبة> الإعدادات> إعدادات الحسابات. يكون هذا مفيدًا عندما يتم تعديل اسم المورد أو التفاصيل المصرفية.

### 2.7 العنوان وجهات الاتصال

يتم تخزين جهات الاتصال والعناوين في ERPNext بشكل منفصل بحيث يمكنك إنشاء جهات اتصال وعناوين متعددة لمورد واحد. بمجرد حفظ المورد ، ستجد خيار إنشاء جهة اتصال وعنوان لهذا المورد.

![مدير المورد](https://docs.erpnext.com/files/supplier-new-address-contact.png)

> نصيحة: عند تحديد مورد في أي معاملة ، جهة الاتصال التي تم تحديد معرف الحقل "أساسي" لها ، سيتم جلبها تلقائيًا مع تفاصيل المورد.

### 2.8 بعد الحفظ

بمجرد ملء جميع التفاصيل اللازمة ، احفظ المستند. عند الحفظ ، ستظهر خيارات إنشاء ما يلي في لوحة التحكم الرئيسية:

***طلب عرض أسعار**: طلب عرض أسعار مقابل هذا المورد.
***عرض أسعار المورد**: أي عروض أسعار أرسلها لك المورد وقمت بإرسالها إلى النظام.
***أمر الشراء**: أوامر الشراء التي قمت بها ضد هذا المورد.
***إيصال الشراء**: إيصالات الشراء التي قدمها هذا المورد والتي قمت بحفظها في النظام.
***فاتورة الشراء**: فواتير الشراء التي قمت بها لهذا المورد.
***إدخال الدفع**: إدخالات الدفع لفواتير الشراء لهذا المورد.
***قاعدة التسعير**: أي قواعد تسعير مرتبطة بهذا المورد. راجع القسم _2.2 قائمة العملات والأسعار_ لمعرفة كيفية عملها.

![حفظ المورد](https://docs.erpnext.com/files/supplier-save.png)

بالنقر فوق الزر "عرض" ، يمكنك عرض دفتر الأستاذ أو الحسابات الدائنة مباشرة لهذا المورد.

يوجد زر "لإرسال تذكير بتحديث ضريبة السلع والخدمات" إلى المورد. يجب أن يكون لديك [حساب بريد إلكتروني] افتراضي (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/email/email-account) أولاً.

## 3. فيديو

1. [عرض أسعار المورد](https://docs.erpnext.com/docs/v13/user/manual/en/buying/supplier-quotation)
2. [بطاقة أداء المورد](https://docs.erpnext.com/docs/v13/user/manual/en/buying/supplier-scorecard)
3. [الاحتفاظ برمز عنصر المورد في مدير السلعة](https://docs.erpnext.com/docs/v13/user/manual/en/buying/articles/maintaining-suppliers-part-no-in-item)