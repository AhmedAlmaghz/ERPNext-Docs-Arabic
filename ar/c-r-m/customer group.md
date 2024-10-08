## مجموعة العملاء

**مجموعة العملاء عبارة عن مجموعة من العملاء المتشابهين بطريقة ما.**

تسمح لك مجموعات العملاء بتنظيم عملائك. عادةً ما يتم تجميع العملاء حسب قطاع السوق بناءً على المجال الذي تعمل فيه الشركة. يتم إنشاء مجموعات العملاء بطريقة هرمية في ERPNext. يمكنك إنشاء مجموعة عملاء رئيسية وإضافة مجموعات عملاء فرعية تحتها.

يمكنك تحديد قائمة الأسعار التي سيتم تطبيقها تلقائيًا على جميع العملاء المنتمين إلى تلك المجموعة. يمكنك أيضًا الحصول على تحليل الاتجاه لكل مجموعة. يتم إنشاء مجموعات العملاء الفردية والتجارية والحكومية بشكل افتراضي. يمكنك إضافة مجموعات العملاء الخاصة بك بناءً على متطلباتك مثل البيع بالتجزئة والبيع بالجملة وما إلى ذلك.

### 1. كيفية إنشاء مجموعة عملاء

1. انتقل إلى**CRM> الإعدادات> مجموعة العملاء**.
2. انقر فوق مجموعة العملاء الرئيسية مثل "جميع مجموعات العملاء".
3. انقر فوق "إضافة طفل".
4. أدخل "اسم مجموعة العملاء".
5. ضع علامة على "عقدة المجموعة" إذا كنت ترغب في إضافة مجموعات فرعية من العملاء تحت هذا.
6. انقر فوق "إنشاء جديد".

![مجموعة العملاء](https://docs.erpnext.com/files/customer-group.png)

> نصيحة: إذا كنت تعتقد أن كل هذا يتطلب الكثير من الجهد ، فيمكنك تركه في "مجموعة العملاء الافتراضية". لكن كل هذا الجهد سيؤتي ثماره عندما تبدأ في تلقي التقارير. فيما يلي مثال على نموذج تقرير:

![مجموعة عملاء تحليلات المبيعات](https://docs.erpnext.com/files/sales-analytics-customer-group.gif)

### 2. سمات

#### 2.1 تعيين حد الائتمان وقائمة الأسعار الافتراضية ونموذج شروط الدفع الافتراضية

يمكنك تعيين حد الائتمان و [قائمة الأسعار](https://docs.erpnext.com/docs/v13/user/manual/en/stock/price-lists) و [شروط الدفع](https: // docs .erpnext.com / docs / v13 / user / manual / en / accounts / payment-terms) وسيتم تطبيقها تلقائيًا عندما يتم تحديد عميل ينتمي إلى مجموعة العملاء في معاملات المبيعات مثل [أمر المبيعات](https: // docs.erpnext.com/docs/v13/user/manual/en/selling/sales-order) و [فاتورة المبيعات](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/ فاتورة المبيعات).

#### 2.2 حساب القبض الافتراضي

لا تحتاج إلى إنشاء دفتر أستاذ محاسبة منفصل لكل عميل في ERPNext. اقرأ [حساب القبض العام](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/articles/common-receivable-account) لمزيد من التفاصيل.

إذا كنت بحاجة إلى حساب مستحق منفصل للعميل ، فيمكنك إضافة نفس الحساب في قسم "حساب القبض الافتراضي".

1. [العميل](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/customer)
2. [قائمة الأسعار](https://docs.erpnext.com/docs/v13/user/manual/en/stock/price-lists)
3. [شروط الدفع](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/payment-terms)