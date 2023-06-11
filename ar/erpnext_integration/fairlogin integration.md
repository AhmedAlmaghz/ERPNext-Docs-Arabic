\n## إعداد نظام Fairlogin

Fairlogin هو مزود oAuth مدرك للائحة العامة لحماية البيانات من fairkom.eu.

لإعداد Fairlogin كموفر oAuth ، انتقل إلى:

> الصفحة الرئيسية> عمليات التكامل> مفتاح تسجيل الدخول الاجتماعي

## إعداد keycloak

يعتمد fairlogin على keycloak ، لذا قد تكون المعلمات متشابهة لأي إعداد oAuth مخصص يسهل keycloak.

هناك تقوم بإضافة عميل جديد ، وتحديد معرف مفتوح كبروتوكول عميل وإدخال عنوان مثيل ERPnext الخاص بك باعتباره عنوان URL الجذر وإعادة التوجيه والقاعدة.

إضافة خدمة ERNext كعميل يتم [تقديمها كخدمة من Fairkom] (https://erp.fairkom.net/cloud/fairlogin-client).

! [إعدادات keycloak ERPnext] (https://docs.erpnext.com/files/fairloginKeycloakERPnext.png)

## إعداد Fairlogin

لتمكين Fairlogin كخيار تسجيل دخول ERPNext ، تحتاج إلى تكوين المعلمات التالية:

* عنوان URL الأساسي https://id.fairkom.net/auth/realms/fairlogin/
* تخويل عنوان URL https://id.fairkom.net/auth/realms/fairlogin/protocol/openid-connect/auth
* إعادة توجيه URL /api/method/frappe.integrations.oauth2_logins.login_via\_fairlogin
* الوصول إلى عنوان URL لرمز الدخول https://id.fairkom.net/auth/realms/fairlogin/protocol/openid-connect/token
* نقطة نهاية واجهة برمجة التطبيقات https://id.fairkom.net/auth/realms/fairlogin/protocol/openid-connect/userinfo

! [إعدادات fairlogin ERPnext] (https://docs.erpnext.com/files/fairloginERPnextSettings.png)

عند تمكين الخدمة ، سيسمح النظام بتسجيل الدخول بأي حساب في Fairlogin.

الدور الافتراضي للمستخدم الجديد هو Blogger (حاليًا مشفر بشكل ثابت).