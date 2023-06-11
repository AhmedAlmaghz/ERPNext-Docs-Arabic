## إعدادات LinkedIn

يمكن هنا تكوين الإعدادات ذات الصلة بـ LinkedIn مثل OAuth. يحتاج ERPNext إلى الوصول إلى واجهة برمجة التطبيقات التي يتم من خلالها مشاركة المنشور وتحقيقه باستخدام بروتوكول مصادقة OAuth 2.0.

## 1. كيفية إعداد LinkedIn Developer App

يجب أن يكون لديك تطبيق LinkedIn Developer لشركتك. يتفاعل ERPNext مع هذا التطبيق لمشاركة المنشور.

### 1.1 إنشاء تطبيق LinkedIn Developer

قم بإنشاء التطبيق بالرابط `https: // www.linkedin.com / developer` قم بتعبئة جميع التفاصيل وتحقق منها. وهذا التطبيق يحتوي على المنتجات التالية.

1. شارك على LinkedIn
2. تسجيل الدخول مع LinkedIn
3. منصة مطوري التسويق![منتج تطبيق LinkedIn Developer](https://docs.erpnext.com/files/linkedin-dev-products.png)

### 1.2 تكوين عناوين URL لإعادة التوجيه:

1. انتقل إلى تطبيق LinkedIn Developers ثم علامة التبويب**Auth**.
2. في قسم**إعدادات OAuth 2.0**أضف**عناوين URL لإعادة التوجيه**: `https: // {yoursite} / api / method / erpnext.crm.doctype.linkedin_settings.linkedin_settings.callback`
3. انقر فوق**تحديث**لإجراء التغييرات. ![عنوان URL لإعادة توجيه LinkedIn](https://docs.erpnext.com/files/linkedin-redirect-urls.png)

## 2. كيفية إعداد إعدادات LinkedIn

للوصول إلى إعدادات LinkedIn ، انتقل إلى:

> الصفحة الرئيسية> CRM> الإعدادات> إعدادات LinkedIn

![إعدادات LinkedIn](https://docs.erpnext.com/files/linkedin-settings.png)

### هوية الشركة

تحصل على معرّف الشركة من عنوان URL الخاص بشركتك على LinkedIn. ![معرف شركة LinkedIn](https://docs.erpnext.com/files/linkedin-company-id.png)

### مفتاح المستهلك وسر المستهلك

تحصل على**مفتاح المستهلك**و**سر المستهلك**من حساب مطور LinkedIn الخاص بك ، انتقل إلى:

> `https: // www.linkedin.com / developer /`> تطبيقاتي> `{Your App}`> Auth

![عميل LinkedIn](https://docs.erpnext.com/files/linkedin-client.png)

بمجرد حفظ المستند عن طريق ملء**معرّف الشركة**و**مفتاح المستهلك**و**سر المستهلك**، ستتم إعادة التوجيه إلى صفحة تسجيل الدخول على LinkedIn من خلال تقديم بيانات اعتماد LinkedIn صالحة والنقر فوق السماح ، يوافق العضو على طلب التطبيق للوصول إلى بيانات الأعضاء والتفاعل مع LinkedIn نيابة عنهم. ![تخويل LinkedIn](https://docs.erpnext.com/files/authorize-linkedin.jpg)