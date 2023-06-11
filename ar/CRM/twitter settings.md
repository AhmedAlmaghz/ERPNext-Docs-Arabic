## إعدادات Twitter

يمكن هنا تكوين الإعدادات المتعلقة بتويتر مثل OAuth. يحتاج ERPNext إلى الوصول إلى واجهة برمجة التطبيقات التي يتم من خلالها مشاركة المنشور وتحقيقه باستخدام بروتوكول مصادقة OAuth 2.0.

## 1. كيفية إعداد تطبيق تويتر

يجب أن يكون لديك تطبيق Twitter لشركتك. يتفاعل ERPNext مع هذا التطبيق لمشاركة التغريدات.

### 1.1 إنشاء تطبيق Twitter Developer

أنشئ تطبيقًا عن طريق الرابط `` https: // developer.twitter.com / 'وتحقق من أن التطبيق لديه**قراءة وكتابة**إذن وصول. ![إذن تطبيق Twitter](https://docs.erpnext.com/files/twitter-app-permission.png)

### 1.2. تكوين عنوان URL لمعاودة الاتصال

1. حدد التطبيق الخاص بك وانتقل إلى**تفاصيل التطبيق**.
2. ثم انتقل إلى**تعديل**وانقر على**تعديل التفاصيل**.
3. أضف عنوان URL لموقع الويب الخاص بك في**عناوين URL لمعاودة الاتصال**مثل: `https: // {yoursite} / api / method / erpnext.crm.doctype.twitter_settings.twitter_settings.callback`
4. انقر فوق**حفظ**لإجراء التغييرات.

![عنوان URL لمعاودة الاتصال لتطبيق Twitter](https://docs.erpnext.com/files/twitter-callback-url.png)

## 2. كيفية ضبط إعدادات تويتر

للوصول إلى إعدادات Twitter ، انتقل إلى:

> الصفحة الرئيسية> CRM> الإعدادات> إعدادات Twitter

![إعدادات Twitter](https://docs.erpnext.com/files/twitter-settings.png)

### 2.1 مفتاح واجهة برمجة التطبيقات وسر واجهة برمجة التطبيقات

يمكنك الحصول على**مفتاح API**و**سر واجهة برمجة التطبيقات**من حساب Twitter Developer الخاص بك ، انتقل إلى:

> `https: // developer.twitter.com /`> تطبيقاتي> `{Your App}`> المفاتيح والرموز المميزة

![رموز مفاتيح Twitter](https://docs.erpnext.com/files/twitter-key-token.png)

بمجرد حفظ المستند عن طريق ملء**API Key**و**API Key Secret**، سيتم إعادة التوجيه إلى صفحة تسجيل الدخول إلى Twitter من خلال تقديم بيانات اعتماد Twitter صالحة والنقر على**Authorize app**، يوافق العضو على طلب التطبيق الخاص بك للوصول إلى بيانات الأعضاء والتفاعل مع Twitter. ![Twitter Authorize App](https://docs.erpnext.com/files/twitter-authorize-app.png)