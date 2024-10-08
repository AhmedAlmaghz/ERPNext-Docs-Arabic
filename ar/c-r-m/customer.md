## عميل

**العميل ، الذي يُعرف أحيانًا باسم العميل أو المشتري أو المشتري ، هو الشخص الذي يتلقى السلع أو الخدمات أو المنتجات أو الأفكار من البائع مقابل مقابل مالي.**

يحتاج كل عميل إلى تعيين معرف فريد. يمكن أن يكون اسم العميل نفسه هو المعرف أو يمكنك تعيين سلسلة تسمية للمعرفات التي سيتم إنشاؤها في [إعدادات البيع](https://docs.erpnext.com/docs/v13/user/manual/en/selling/selling-settings ).

للوصول إلى قائمة العملاء ، انتقل إلى:

> الصفحة الرئيسية> CRM> خط أنابيب المبيعات

أو

> الصفحة الرئيسية> البيع> العملاء

## 1. كيفية إنشاء عميل

1. اذهب إلى قائمة العملاء وانقر على جديد.
2. أدخل الاسم الكامل للعميل.
3. حدد فردًا إذا كان العميل يمثل فردًا أو شركة إذا كان العميل يمثل شركة في حقل النوع.
4. حدد [مجموعة عملاء](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/customer-group). الفردية والتجارية وغير الربحية والحكومية متاحة بشكل افتراضي. يمكنك إنشاء مجموعات إضافية إذا كنت بحاجة.
5. حدد الإقليم.
6. إذا كان يتم إنشاء العميل مقابل عميل متوقع ، فيمكنك تحديده في الحقل من العميل المتوقع.
7. حفظ.
    
    ![إنشاء عميل جديد](https://docs.erpnext.com/files/create-customer.gif)
    

يمكنك عدم السماح بأوامر المبيعات وفواتير المبيعات للعميل بالنقر فوق "معطل".

> نصيحة متقدمة: إذا كان العميل يمثل إحدى شركاتك الخاصة ، فحدد "عميل داخلي". تحقق من [Inter Company Invoices](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/inter-company-invoices) لمزيد من التفاصيل.

يمكنك أيضًا تحميل تفاصيل العميل عبر [أداة استيراد البيانات](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/data/data-import).

## 2. سمات

يكون التدفق العام للمعاملات للعميل على النحو التالي:

![مخطط تدفق المبيعات](https://docs.erpnext.com/files/customer-to٪20selling-flowchart.jpeg)

> ملاحظة: العملاء منفصلون عن جهات الاتصال والعناوين. يمكن للعميل أن يكون لديه جهات اتصال وعناوين متعددة.

### 2.1 جهات اتصال وعناوين متعددة

[جهات الاتصال](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/contact) و [العناوين](https://docs.erpnext.com/docs/v13/user/manual / en / CRM / address) بشكل منفصل بحيث يمكنك إرفاق عدة جهات اتصال أو عناوين للعميل.

### 2.2 السماح بإنشاء فاتورة مبيعات بدون أمر مبيعات ومذكرة تسليم

إذا تم تكوين الخيار "إشعار التسليم مطلوب" أو "أمر المبيعات مطلوب" على أنه "نعم" في [إعدادات البيع](https://docs.erpnext.com/docs/v13/user/manual/en/selling/selling- الإعدادات) ، يمكن تجاوزها لعميل معين عن طريق تمكين "السماح بإنشاء فاتورة المبيعات بدون طلب مبيعات" أو "السماح بإنشاء فاتورة المبيعات بدون إشعار التسليم" في العميل الرئيسي.

![الإعداد الإلزامي لأمر المبيعات](https://docs.erpnext.com/files/customer-so-dn-required.png)

### 2.3 تحديد فئة الاستقطاع الضريبي

يمكنك تعيين فئة الاستقطاع الضريبي لإعداد TCS ضد العملاء المؤهلين. لمزيد من المعلومات ، تفضل بزيارة صفحة [فئة الاستقطاع الضريبي](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/tax-withholding-category).

### 2.4 العملة الافتراضية وقائمة الأسعار

يدعم ERPNext [عدة عملات](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/multi-currency-accounting) و [قوائم الأسعار](https://docs.erpnext.com / docs / v13 / user / manual / en / stock / قوائم الأسعار).

يمكنك تعيين العملة الافتراضية لاستخدامها لهذا العميل في أوامر المبيعات وفواتير المبيعات عن طريق تحديد العملة المناسبة في "عملة الفوترة".

وبالمثل ، يمكنك تعيين قائمة الأسعار الافتراضية لاستخدامها لهذا العميل في أوامر المبيعات وفواتير المبيعات عن طريق تحديد العملة المناسبة في قائمة الأسعار الافتراضية.

### 2.5 التكامل مع الحسابات

على عكس العديد من برامج المحاسبة ، لا تحتاج إلى إنشاء دفتر أستاذ محاسبة منفصل لكل عميل. بشكل افتراضي ، يتم إنشاء دفتر أستاذ موحد يسمى**المدينون**.

ومع ذلك ، إذا كنت تحتاج على وجه التحديد إلى دفتر أستاذ منفصل للعميل ، فقم أولاً بإنشاء دفتر الأستاذ ضمن حسابات القبض في [مخطط الحسابات](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/chart -of-accounts.html) ثم قم بإضافتها في قسم المحاسبة الخاص بالعميل.

> نصيحة متقدمة: يدعم ERPNext [محاسبة الشركات المتعددة](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/inter-company-journal-entry). يمكنك استخدام نفس سجلات العملاء في العديد من الشركات. نظرًا لأن دفتر الأستاذ المحاسبي خاص بالشركة ، فأنت بحاجة إلى تحديد الشركة ودفتر الأستاذ المقابل في قسم المحاسبة إذا قررت أن يكون لديك دفتر أستاذ محاسبة منفصل للعميل.

### 2.6 حد الائتمان وشروط الدفع

يمكنك تعيين حد الائتمان عن طريق إدخال المبلغ في حقل "حد الائتمان". اقرأ [Credit Limit](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/credit-limit) لمزيد من التفاصيل.

يمكنك تحديد [شروط الدفع] الافتراضية (https://docs.erpnext.com/docs/v13/user/manual/en/accounts/payment-terms) ليتم تطبيقها في أوامر المبيعات وفواتير المبيعات في "شروط الدفع الافتراضية" النموذج.

### 2.7 فريق المبيعات وشريك المبيعات

إذا كان لديك واحد أو أكثر من [مندوب مبيعات](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/sales-person) لإدارة المبيعات للعميل ، فيمكنك إضافتهم في قسم فريق المبيعات. إذا كان هناك عدة مندوبين مبيعات مشتركين ، يمكنك تقسيم المساهمة بينهم. تأكد من أن مجموع مساهمة جميع مندوبي المبيعات يساوي 100٪.

تحقق من [مندوبي المبيعات في معاملة المبيعات](https://docs.erpnext.com/docs/v13/user/manual/en/selling/articles/sales-persons-in-the-sales-transactions) لمزيد من التفاصيل.

إن [شريك المبيعات](https://docs.erpnext.com/docs/v13/user/manual/en/selling/sales-partner) هو موزع / تاجر / وكيل بالعمولة / تابع / بائع يسهل منتجاتك / مبيعات الخدمات مقابل عمولة. إذا قمت ببيع منتجاتك / خدماتك للعميل من خلال أحد شركاء المبيعات ، يمكنك تعيينها في حقل "شريك المبيعات" وذكر "معدل العمولة" لحساب العمولة.

### 2.8 برنامج الولاء

إذا كنت ترغب في تقديم [برنامج الولاء](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/loyalty-program) إلى العميل ، فحدده في حقل برنامج الولاء.

### 2.9 عرض دفتر الأستاذ المحاسبي وحسابات القبض

اضغط على زر دفتر الأستاذ المحاسبي لعرض جميع المعاملات المحاسبية مع العميل.

انقر فوق زر "حسابات القبض" لعرض تفاصيل جميع الفواتير المستحقة.

### 2.10 قم بتعيين معرف العميل ومجموعة العملاء الافتراضية والإقليم وقائمة الأسعار

يمكنك تعيين كيفية إنشاء معرّف فريد لكل عميل في [إعدادات البيع](https://docs.erpnext.com/docs/v13/user/manual/en/selling/selling-settings).

***سلسلة التسمية**: إذا كنت ترغب في إنشاء معرّف فريد لكل عميل بناءً على سلسلة التسمية ، فحدد "سلسلة التسمية" في تسمية العميل.
    
***Customer Name**: إذا كان يجب استخدام اسم العميل نفسه كمعرف ، فحدد "اسم العميل" في "تسمية العميل بواسطة". في هذه الحالة ، إذا أنشأت عميلين بأسماء متطابقة ، فسيتم إضافة**\ - 1**للعميل الثاني.
    

![معرف العميل](https://docs.erpnext.com/files/customer-with-identical-names.png)

يمكنك تعيين مجموعة العملاء الافتراضية والإقليم وقائمة الأسعار في [إعدادات البيع](https://docs.erpnext.com/docs/v13/user/manual/en/selling/selling-settings).

يمكنك تخصيص نوع مستند العميل باستخدام أداة [Customize Form](https://docs.erpnext.com/docs/v13/user/manual/en/customize-erpnext/custom-field).

1. [مجموعة العملاء](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/customer-group)
2. [اقتباس](https://docs.erpnext.com/docs/v13/user/manual/en/selling/quotation)
3. [قائمة الأسعار](https://docs.erpnext.com/docs/v13/user/manual/en/stock/price-lists)
4. [جهة اتصال](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/contact)
5. [الفرق بين العميل المتوقع وجهة الاتصال والعميل](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/articles/difference_between_lead_contact_and_customer)