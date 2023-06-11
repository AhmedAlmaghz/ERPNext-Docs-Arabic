## طلب الدفع

**يتم استخدام طلب الدفع لطلب الدفع من العميل لأمر مبيعات أو فاتورة.**

يتم إرسال طلب الدفع عبر البريد الإلكتروني وسيحتوي على ارتباط إلى بوابة الدفع في حالة الإعداد. يمكنك إنشاء طلب دفع عبر أمر مبيعات أو فاتورة مبيعات. يمكن أيضًا إعداد طلب الدفع مقابل طلب الشراء أو فاتورة الشراء للسجلات الداخلية. بعد ذلك ، يمكن معالجة المدفوعات دفعة واحدة باستخدام [أمر الدفع](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/payment-order).

للوصول إلى طلب الدفع ، انتقل إلى:

> الصفحة الرئيسية> المحاسبة> حسابات القبض> طلب الدفع

## 1. المتطلبات الأساسية

قبل إنشاء واستخدام طلب الدفع ، يُنصح بإنشاء ما يلي أولاً:

1. [فاتورة المبيعات](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/sales-invoice)
2. [فاتورة الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/purchase-invoice)
3. [أمر المبيعات](https://docs.erpnext.com/docs/v13/user/manual/en/selling/sales-order)
4. [أمر الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/buying/purchase-order)

## 2. كيفية إنشاء طلب الدفع

لا يمكن إنشاء طلب الدفع يدويًا ، بل يتم إنشاؤه من أمر مبيعات / شراء أو فاتورة.

### 2.1 إنشاء طلب الدفع عن طريق طلب المبيعات

في طلب المبيعات ، انقر فوق إنشاء ثم انقر فوق الدفع لإجراء دفعة مقدمة. لمعرفة المزيد حول الدفعة المقدمة ، تفضل بزيارة صفحة [إدخال الدفع المسبق](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/advance-payment-entry).

![طلب الدفع من طلب المبيعات](https://docs.erpnext.com/files/payment-request-from-sales-order.png)

### 2.2 إنشاء طلب الدفع عبر فاتورة المبيعات

في فاتورة المبيعات ، انقر فوق إنشاء ثم انقر فوق الدفع لإجراء الدفع مقابل الفاتورة.

![طلب الدفع من فاتورة المبيعات](https://docs.erpnext.com/files/payment-request-from-sales-invoice.png)

حدد حساب بوابة الدفع المناسب عند طلب الدفع لترحيل الحسابات. سيتم اعتبار رئيس الحساب المحدد في بوابة الدفع لإنشاء إدخال دفتر اليومية.

> ملاحظة: يجب أن تكون عملة الفاتورة / الطلب وعملة "حساب بوابة الدفع" هي نفسها.

![تفاصيل طلب الدفع](https://docs.erpnext.com/files/payment-request-details.png)

### 2.3 إخطار العميل

يمكنك إخطار العميل من طلب الدفع باستخدام [تنسيق الطباعة](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-format). إذا تم تعيين البريد الإلكتروني للاتصال بالعميل ، فسيتم جلبه تلقائيًا. إذا لم يكن الأمر كذلك ، يمكنك تعيين عنوان بريد إلكتروني في طلب الدفع.

![تفاصيل طلب الدفع](https://docs.erpnext.com/files/payment-request-recipient-details.png)

### 2.4 طلب البريد

هنا مثال لطلب البريد الإلكتروني. يتم إنشاء عنوان URL تلقائيًا إذا قمت بإعداد تكامل الدفع المعني. لمعرفة المزيد حول عمليات الدمج ، [تفضل بزيارة هذه الصفحة](https://docs.erpnext.com/docs/v13/user/manual/en/erpnext_integration).

![طلب الدفع](https://docs.erpnext.com/files/pr-email.png)

### 2.5 طلب الدفع بدون استخدام أي بوابة

في حالة عدم رغبتك في استخدام أي تكامل أو بوابة دفع وتريد فقط إرسال إشعار ، ما عليك سوى تعيين الحساب المصرفي. سيتعين عليك إنشاء الرسالة وفقًا للتفاصيل المصرفية. يمكن للطرف بعد ذلك تحويل المبلغ إلى الحساب المصرفي المذكور.

1. [إدخال الدفع](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/payment-entry)
2. [شروط الدفع](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/payment-terms)
3. [فاتورة المبيعات](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/sales-invoice)
4. [فاتورة الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/purchase-invoice)