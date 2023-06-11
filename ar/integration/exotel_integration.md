## تكامل Exotel

يتيح لك هذا التكامل دمج Exotel في حساب ERPNext الخاص بك. يمكن حفظ العملاء المتوقعين وأرقام هواتفهم التي تم التقاطها عبر Exotel مباشرةً في ERPNext الخاص بك.

## 1. سمات

* تتبع المكالمات الواردة في حساب ERPNext الخاص بك.
* يُظهر نافذة منبثقة لمعلومات العميل / العميل المتوقع للموظفين عند تلقي مكالمة واردة.

## 2. كيفيه التنصيب

### 2.1 قم بإعداد حساب Exotel الخاص بك

* قم بتسجيل الدخول إلى حساب Exotel الخاص بك وانتقل إلى App Bazar.
* إنشاء تطبيق جديد لتدفق جديد.
* قم بإعداد التدفق كما يحلو لك.
* في واجهة برمجة تطبيقات الاتصال الخاصة بك ضمن "إنشاء نافذة منبثقة ..." والصق عنوان URL التالي: `https: // <your-site> / api / method / erpnext.erpnext_integrations.exotel_integration.handle_incoming_call`

![Connect Applet](https://docs.erpnext.com/files/connect_applet.png)![قسم الاتصال المنبثق](https://docs.erpnext.com/files/create_popup_section.png)

>**ملاحظة:**استبدل "<your-site>` في عنوان URL باسم موقعك. على سبيل المثال ، إذا كان اسم الموقع هو**frappe.erpnext.com**، فسيكون عنوان URL: `https: // frappe.erpnext.com / api / method / erpnext.erpnext_integrations.exotel_integration.handle_incoming_call`

* بعد ذلك ، أضف تطبيق Passthru الصغير ضمن "بعد انتهاء محادثة المكالمة" والصق عنوان URL التالي: `https: // <your-site> / api / method / erpnext.erpnext_integrations.exotel_integration.handle_end_call`

![قسم نهاية المحادثة](https://docs.erpnext.com/files/after_conversation_ends_section.png)

![قسم بعد انتهاء المكالمة](https://docs.erpnext.com/files/passthru_end_call.png)

>**ملاحظة:**تأكد من تحديد "Make Passthru Async".

* على نحو مماثل ، أضف تطبيقًا صغيرًا ممرًا ضمن قسم "إذا لم يجيب أحد ..." والصق عنوان URL التالي: `https: // <your-site> / api / method / erpnext.erpnext_integrations.exotel_integration.handle_missed_call`

![قسم بلا رد](https://docs.erpnext.com/files/no_response.png)

![قسم بعد انتهاء المكالمة](https://docs.erpnext.com/files/passthru_missed_call.png)

>**ملاحظة:**تأكد من تحديد "Make Passthru Async".

* حفظ التدفق.
* الآن قم بتعيين هذا التطبيق الذي تم إنشاؤه حديثًا إلى ExoPhone الخاص بك والذي تتلقى منه مكالمات عملك.

### 2.2 الإعداد في ERPNext

* من شريط رائع ، انتقل إلى "إعدادات Exotel".
* اضبط "Exotel SID" و "Exotel Token". يمكنك العثور على مفتاح Exotel API والرمز المميز على [Exotel Dashboard](https://my.exotel.com/apisettings/site#api-credentials).
* انتقل إلى وسيلة الاتصال.
* أضف ExoPhone الخاص بك وجدول هذا الرقم. بناءً على هذا الجدول الزمني ، سيتلقى الموظفون النافذة المنبثقة.