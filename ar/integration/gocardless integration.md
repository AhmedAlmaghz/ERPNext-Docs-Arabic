## إعداد GoCardless

لإعداد GoCardless ، انتقل إلى "استكشاف> عمليات التكامل> إعدادات GoCardless"

## إعداد GoCardless

لتمكين GoCardless في حساب ERPNext الخاص بك ، تحتاج إلى تكوين المعلمات التالية و Access Token واختيارياً (لكن يوصى به بشدة) ، مفتاح Webhooks Secret.

يمكنك إعداد عدة بوابات دفع GoCardless إذا لزم الأمر. سيحدد اختيار حساب بوابة الدفع حساب GoCardless المستخدم للدفع.

![إعدادات GoCardless](https://docs.erpnext.com/files/gocardless_account.png)

عند تمكين الخدمة ، سيقوم النظام بإنشاء سجل بوابة الدفع ورئيس الحساب في مخطط الحساب مع نوع الحساب مثل البنك.

![GoCardless COA](https://docs.erpnext.com/files/gocardless_coa.png)

سيتم أيضًا إنشاء حساب بوابة دفع. يمكنك تغيير الحساب المصرفي الافتراضي إذا لزم الأمر وإنشاء نموذج لطلب الدفع.

![حساب بوابة الدفع](https://docs.erpnext.com/files/payment_gateway_account_gocardless.png)

بعد تكوين حساب Payment Gateway ، يمكن لنظامك قبول المدفوعات عبر الإنترنت من خلال GoCardless.

## تدفق مدفوعات SEPA

عند بدء عملية دفع SEPA جديدة ، يُطلب من العميل إدخال رقم IBAN الخاص به (أو رقم الحساب المحلي) والتحقق من صحة تفويض SEPA.

عند التحقق من التفويض ، يتم إرسال طلب الدفع إلى GoCardless ومعالجته.

إذا كان العميل لديه بالفعل تفويض صالح من منطقة الدفعات المالية الموحدة باليورو SEPA ، فعندما يتم إرسال طلب الدفع مباشرة إلى GoCardless دون الحاجة إلى التحقق من صحته بدلاً من إرسال طلب الدفع إلى العميل. سيتلقى العميل فقط رسالة تأكيد بالبريد الإلكتروني من GoCardless لإعلامه بأنه تمت معالجة الدفع.

## إلغاء الانتداب

يمكنك إعداد Webhook في GoCardless لتعطيل التفويضات الملغاة أو منتهية الصلاحية تلقائيًا في ERPNext.

يجب أن يكون عنوان URL لنقطة النهاية للخطاف التلقائي على الويب:

`https: // yoursite.com / api / method / erpnext.erpnext_integrations.doctype.gocardless_settings.webhooks`

في هذه الحالة ، لا تنس تكوين Webhooks Secret Key في إعدادات حساب GoCardless في ERPNext.

## عملات المعاملات المدعومة

""
"EUR" ، "DKK" ، "GBP" ، "SEK"
""