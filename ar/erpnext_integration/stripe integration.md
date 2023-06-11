\n## إعداد Stripe

لإعداد Stripe ، `Explore> Integrations> Stripe Settings`

#### شريط الإعداد

لتمكين خدمة دفع Stripe ، تحتاج إلى تكوين معلمات مثل Publishable Key، Secret Key! [إعدادات Razorpay] (https://docs.erpnext.com/files/stripe_setting.png)

عند تمكين الخدمة ، سيقوم النظام بإنشاء سجل بوابة الدفع ورئيس الحساب في مخطط الحساب مع نوع الحساب مثل البنك.

! [Stripe COA] (https://docs.erpnext.com/files/stripe_coa.png)

كما سيتم إنشاء إدخال حساب بوابة الدفع. حساب بوابة الدفع هو مركز التكوين من هذا يمكنك تعيين رئيس الحساب من COA الموجودة ، قالب نص البريد الإلكتروني الافتراضي لطلب الدفع.

! [حساب بوابة الدفع] (https://docs.erpnext.com/files/payment_gateway_account_stripe.png)

بعد تكوين حساب Payment Gateway ، يستطيع نظامك قبول المدفوعات عبر الإنترنت.

### إعداد خطط الاشتراكات

إذا كنت بحاجة إلى إصدار فاتورة بمبلغ متكرر بدلاً من دفع رسوم لمرة واحدة ، فيمكنك استخدام نظام اشتراك Stripe.

بمجرد إنشاء خطط الفوترة الخاصة بك في Stripe ، أضف واحدة أو عدة "خطة دفع" جديدة في Frappe.

! [خطة الدفع] (https://docs.erpnext.com/files/payment_plan.png)

بعد ذلك ، عند إنشاء طلب الدفع الخاص بك ، انقر فوق حقل الاختيار "هو اشتراك" وستقوم إضافة النظام بجلب خطط الاشتراك المقابلة من داخل الاشتراك المقابل.

! [طلب الدفع] (https://docs.erpnext.com/files/subscription_payment_request.png)

سيقوم ERPNext تلقائيًا بإنشاء اشتراك جديد لهذا العميل في Stripe.

#### دعم عملات المعاملات

""
"AED" ، "ALL" ، "ANG" ، "ARS" ، "AUD" ، "AWG" ، "BBD" ، "BDT" ، "BIF" ، "BMD" ، "BND" ،
"BOB" و "BRL" و "BSD" و "BWP" و "BZD" و "CAD" و "CHF" و "CLP" و "CNY" و "COP" و "CRC" و "CVE" و "CZK "،" DJF "،
"DKK" و "DOP" و "DZD" و "EGP" و "ETB" و "EUR" و "FJD" و "FKP" و "GBP" و "GIP" و "GMD" و "GNF" و "GTQ "،" GYD "،
"HKD" و "HNL" و "HRK" و "HTG" و "HUF" و "IDR" و "ILS" و "INR" و "ISK" و "JMD" و "JPY" و "KES" و "KHR "،" KMF "،
"KRW" و "KYD" و "KZT" و "LAK" و "LBP" و "LKR" و "LRD" و "MAD" و "MDL" و "MNT" و "MOP" و "MRO" و "MUR "،" MVR "،
"MWK" و "MXN" و "MYR" و "NAD" و "NGN" و "NIO" و "NOK" و "NPR" و "NZD" و "PAB" و "PEN" و "PGK" و "PHP "،" PKR "،
"PLN" ، "PYG" ، "QAR" ، "RUB" ، "SAR" ، "SBD" ، "SCR" ، "SEK" ، "SGD" ، "SHP" ، "SLL" ، "SOS" ، "STD "،" SVC "،
"SZL" و "THB" و "TOP" و "TTD" و "TWD" و "TZS" و "UAH" و "UGX" و "USD" و "UYU" و "UZS" و "VND" و "VUV "،" WST "،
"XAF" ، "XOF" ، "XPF" ، "YER" ، "ZAR"
""