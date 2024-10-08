## إعدادات الحسابات

هناك العديد من إعدادات الحساب في ERPNext لتقييد الإجراءات وتكوينها في وحدة المحاسبة.

## إعدادات المعاملات

![إعدادات المعاملات](https://docs.erpnext.com/files/CleanShot٪202021-08-26٪20at٪2011.56.43@2xff68e5.png)

### 1. بدل الفواتير (٪)

النسبة المئوية التي يمكنك من خلالها المبالغة في فواتير المعاملات. على سبيل المثال ، إذا كانت قيمة الطلب هي 100 دولار لعنصر ما وتم تعيين النسبة المئوية هنا على 10٪ ، فيُسمح لك بالفوترة بمبلغ 110 دولارات.

### 2. الدور المسموح به لأكثر من بيل

يُسمح للمستخدمين الذين لديهم هذا الدور بزيادة الفاتورة فوق نسبة البدل.

### 3. الدور المسموح به لتجاوز حد الائتمان

حدد الدور المسموح به لإرسال المعاملات التي تتجاوز الحدود الائتمانية المعينة. يمكن تعيين حد الائتمان في نموذج العميل.

### 4. تحقق من تفرد رقم فاتورة المورد

عند التحديد ، لن يُسمح بفواتير الشراء التي تحمل "رقم فاتورة المورد" نفسها. هذا مفيد لتجنب الإدخالات المكررة.

### 5. إلغاء ربط الدفع عند إلغاء الفاتورة

إذا تم تحديده ، فسيقوم النظام بإلغاء ربط الدفعة بالفاتورة المعنية. بشكل افتراضي ، إذا تم تقديم إدخال الدفع ، فلا يمكن إلغاء الفاتورة المرتبطة حتى يتم أيضًا إلغاء إدخال الدفع. عند إلغاء الربط ، يمكنك الآن إلغاء الفواتير وتعديلها. لكن المدفوعات لا يتم ربطها وتعتبر مدفوعات مقدمة.

### 6. جلب شروط الدفع تلقائيًا من الطلب

سيؤدي تمكين هذا إلى جلب شروط الدفع تلقائيًا من أمر الشراء / المبيعات إلى فاتورة الشراء / المبيعات المرتبطة به.

### 7. حذف إدخالات المحاسبة ودفتر الأستاذ عند حذف المعاملة

سيسمح تمكين هذا بحذف إدخالات دفتر الأستاذ العام ودفتر الأستاذ المرتبطين عند حذف الفواتير والإيصالات. يمكن التحقق من ذلك إذا كنت لا تريد أن تفقد معرف المستند بعد إلغاء المستند. يمكنك الآن إلغاء وحذف المستند للحصول على نفس معرف المستند مرة أخرى.

### 8. دفتر إدخال إهلاك الأصول تلقائيًا

عند تحديده ، سيتم إنشاء إدخال تلقائي لاستهلاك الأصول بناءً على أول تاريخ محدد. على سبيل المثال ، ستتم جدولة الإهلاك السنوي لأحد العناصر خلال 3/4 سنوات التالية استنادًا إلى عدد الإهلاك المحجوز المحدد في مدير الأصول. لمزيد من التفاصيل ، تفضل بزيارة صفحة [إهلاك الأصول](https://docs.erpnext.com/docs/v13/user/manual/en/asset/asset-depreciation).

### 9. إلغاء ربط الدفع المسبق عند إلغاء الطلب

على غرار الخيار السابق ، يؤدي هذا إلى إلغاء ربط أي مدفوعات مقدمة مقابل أوامر الشراء / المبيعات.

### 10. قم بتمكين محاسبة الطرف المشتركة

إذا تم تحديده ، فسيتم ترحيل إدخال دفتر اليومية للتعديل تلقائيًا عند إنشاء فواتير المبيعات / الشراء مقابل العميل والمورد المشترك. لمزيد من التفاصيل ، تفضل بزيارة [Common Party Accounting](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/articles/common_party_accounting)

### 11. إنشاء إدخالات دفتر الأستاذ لتغيير المبلغ

إذا تم تحديده ، بالنسبة لفاتورة نقاط البيع ، فسيقوم النظام بترحيل إدخالات دفتر الأستاذ مع مراعاة مبلغ التغيير المحدد.

### 12. تفعيل محاسبة الخصم

إذا تم تحديده ، يمكن إضافة حسابات الخصم في جدول الأصناف لفواتير المبيعات ، مما سيسمح لك بحساب الخصومات المطبقة على الأصناف بشكل أكثر كفاءة. يتيح لك أيضًا إضافة حسابات الخصم الافتراضية للعناصر ، والتي سيتم جلبها تلقائيًا عند إضافة العنصر إلى فاتورة المبيعات.

## إعدادات الضرائب

![إعدادات الضرائب](https://docs.erpnext.com/files/Tax_Settings_Revised.png)

### 1. تحديد فئة ضريبة العنوان من

يمكن تعيين [فئة الضرائب](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/tax-category) على العناوين. يمكن أن يكون العنوان هو عنوان الشحن أو الفواتير. قم بتعيين العناصر التي سيتم تحديدها عند تطبيق فئة الضريبة.

### 2. إضافة الضرائب والرسوم تلقائيًا من نموذج ضريبة العنصر

سيؤدي تمكين هذا إلى ملء جدول الضرائب في المعاملات إذا تم تعيين [قالب ضريبة العنصر](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/item-tax-template) لعنصر ويتم تحديد هذا العنصر في المعاملة.

### 3. سجل خسارة الضريبة على خصم السداد المبكر

سيؤدي تمكين هذا إلى تقسيم استقطاعات خصم إدخال الدفع إلى خسارة الدخل وخسارة ضريبية إذا كان المستند مقابل إدخال الدفع يحتوي على [خصم الدفع المبكر](https://docs.erpnext.com/docs/v14/user/manual/en/ حسابات / شروط الدفع # 11-إعداد-خصم-على-المدفوعات المبكرة).

## إعدادات إقفال الفترة

![إعدادات إغلاق الفترة](https://docs.erpnext.com/files/Period٪20Closing٪20Settings.png)

### 1. الحسابات المجمدة حتى تاريخ

تجميد المعاملات المحاسبية حتى تاريخ محدد ، لا يمكن لأي شخص إجراء / تعديل الإدخال باستثناء الدور المحدد.

### 2. الدور مسموح به لتعيين حسابات مجمدة وتعديل الإدخالات المجمدة

يُسمح للمستخدمين الذين لهم هذا الدور بتعيين حسابات مجمدة وإنشاء / تعديل إدخالات المحاسبة ضد الحسابات المجمدة.

## إعدادات المحاسبة المؤجلة

![إعدادات المحاسبة المؤجلة](https://docs.erpnext.com/files/Defirmed٪20Accounting٪20Settings٪20.png)

### 1. حجز إدخالات مؤجلة على أساس

يمكن حجز مبلغ الإيرادات المؤجلة بناءً على معيارين. الخيار الافتراضي هنا هو "الأيام". إذا تم تحديد "الأيام" ، فسيتم حجز مبلغ الإيرادات المؤجلة بناءً على عدد الأيام في كل شهر وإذا تم تحديد "الأشهر" ، فسيتم حجزها بناءً على عدد الأشهر.**على سبيل المثال:**إذا تم تحديد "أيام" وتوجب تأجيل عائد 12000 دولار أمريكي على مدى 12 شهرًا ، فسيكون 986.30 دولارًا أمريكيًا للشهر الذي يحتوي على 30 يومًا وسيتم حجز 1019.17 دولارًا أمريكيًا للشهر الذي يتكون من 31 يومًا. إذا تم تحديد "الأشهر" ، فسيتم حجز 1000 دولار من الإيرادات المؤجلة كل شهر بغض النظر عن عدد أيام الشهر.

### 2. معالجة الإدخال المؤجل للمحاسبة تلقائيًا

يتم تمكين هذا الإعداد الافتراضي. في حالة عدم رغبتك في ترحيل إدخالات المحاسبة المؤجلة تلقائيًا ، يمكنك تعطيل هذا الإعداد. إذا تم تعطيل هذا الإعداد ، فسيتعين معالجة المحاسبة المؤجلة يدويًا باستخدام [معالجة المحاسبة المؤجلة](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/process-defirmed-accounting)

### 3. كتاب مؤجل إدخالات عن طريق إدخال دفتر اليومية

بشكل افتراضي ، يتم ترحيل إدخالات دفتر الأستاذ مباشرة لتسجيل الإيرادات المؤجلة مقابل الفاتورة. من أجل حجز هذا المبلغ المؤجل الترحيل عبر إدخال دفتر اليومية ، يمكن تمكين هذا الخيار.

### 4. إرسال إدخالات دفتر اليومية

هذا الخيار قابل للتطبيق فقط إذا تم ترحيل إدخالات المحاسبة المؤجلة عبر إدخال دفتر اليومية. بشكل افتراضي ، يتم الاحتفاظ بإدخالات دفتر اليومية للترحيل المؤجل في حالة المسودة ويتعين على المستخدم التحقق من تلك الإدخالات وإرسالها يدويًا. إذا تم تمكين هذا الخيار ، فسيتم إرسال إدخالات دفتر اليومية تلقائيًا دون أي تدخل من المستخدم. لن يتم عرض هذا الخيار إلا إذا تم تحديد**Book المؤجلة الإدخالات عبر إدخال دفتر اليومية**.

## إعدادات الطباعة

![إعدادات الطباعة](https://docs.erpnext.com/files/Print٪20Settings.png)

### 1. عرض الضرائب الشاملة في الطباعة

سيتم عرض الضرائب المطبقة في طريقة عرض الطباعة.

### 2. إظهار جدول الدفع في الطباعة

يظهر جدول الدفع عند استخدام [شروط الدفع](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/payment-terms). سيؤدي تمكين هذا إلى إظهار هذا الجدول في طريقة عرض الطباعة.

## إعدادات صرف العملات

![إعدادات صرف العملات](https://docs.erpnext.com/files/Currency٪20Exchange٪20Settings٪20.png)

### 1. السماح بأسعار الصرف القديمة

يجب إلغاء تحديد هذا إذا كنت تريد أن يتحقق ERPNext من عمر السجلات التي تم جلبها من صرف العملات في معاملات العملات الأجنبية. إذا لم يتم تحديده ، فسيكون حقل سعر الصرف للقراءة فقط في المستندات.

الأيام التي لا معنى لها هو عدد الأيام التي يجب استخدامها عند تقرير ما إذا كان سجل صرف العملات قديمًا أم لا. يكون هذا صالحًا عندما يكون "السماح بالمعدلات القديمة"**معطلاً**. لذلك ، إذا تم تعيين الأيام القديمة على أنها 10 ، فسيتم السماح بالمعدلات القديمة التي هي 10 أيام. إذا تم تمكين السماح بالمعدلات القديمة ، فلا يوجد حد زمني لأعمار الأسعار القديمة.

إذا تم تمكين الأسعار التي لا معنى لها ، فإن ترتيب الجلب هو:

* أحدث سعر من استمارة صرف العملات
* إذا لم يتم العثور على صرف العملات ، يتم جلب أحدث سعر حسب السوق تلقائيًا

إذا تم تعطيل الأسعار القديمة ، فسيكون ترتيب الجلب كما يلي:

* أحدث سعر من صرف العملات حتى عدد الأيام المحددة في "الأيام القديمة"
* إذا لم يتم العثور على صرف عملات ، فسيتم جلب آخر سعر حسب السوق تلقائيًا

## إعدادات التقرير

![إعدادات التقرير](https://docs.erpnext.com/files/Report٪20Settings.png)

### 1. استخدم تنسيق التدفق النقدي المخصص

يمكنك اختيار استخدام تنسيقات التدفقات النقدية المخصصة لتخصيص شكل تقرير التدفق النقدي. لمعرفة المزيد ، [تفضل بزيارة هذه الصفحة](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/articles/how-to-customise-cash-flow-report).