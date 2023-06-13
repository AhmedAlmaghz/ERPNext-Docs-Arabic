---
description: erpnext shipping
---

# erpnext الشحن

### شحن ERPNext

> تم تقديمه في الإصدار 13

**يساعدك تطبيق ERPNext Shipping على مقارنة أسعار الشحن التي يقدمها العديد من مزودي الخدمة ، وإنشاء الملصقات ، وتتبع حالة الشحنات الخاصة بك.**

يتوفر التكامل مع مزودي الخدمة التاليين:

1. [Packlink](https://www.packlink.com/en-GB/)
2. [LetMeShip](https://www.letmeship.com/en/)
3. [SendCloud](https://www.sendcloud.com/)

> للاستفادة من هذه الميزات ، يجب تثبيت تطبيق**ERPNext Shipping**على موقعك. يمكنك الاستفادة من التطبيق [على GitHub](https://github.com/frappe/erpnext-shipping/tree/master) ، [على Frappe Cloud Marketplace](https://frappecloud.com/marketplace/apps/shipping) أو يمكنك الاتصال بمنصة الاستضافة الخاصة بك.

### 1. اعداد

لكي يعمل التطبيق بسلاسة ، سيتعين عليك إنشاء مفتاح API من**واحد على الأقل**من الأنظمة الأساسية المذكورة أعلاه. فيما يلي دليل لإعدادها:

#### 1.1 Packlink API

1. التسجيل في [Packlink PRO](https://auth.packlink.com/en-GB/pro/register%D8%9Fplatform=PRO\&platform\_country=UN).
2. اتبع [هذه الخطوات](https://support-pro.packlink.com/hc/en-gb/articles/213431749-How-to-generate-an-API-key-on-PRO) لإنشاء \* _مفتاح API_\*.
3. ابحث عن**Packlink**في الشريط الرائع.
4. أضف**API Key**إلى Packlink DocType ، حدد الحقل "ممكّن".
5. حفظ.

![Packlink API](https://docs.erpnext.com/files/packlink\_api.png)

#### 1.1 Sendcloud API

1. التسجيل على [Sendcloud](https://panel.sendcloud.sc/accounts/signup/).
2. اتبع [هذه الخطوات](https://support.sendcloud.com/hc/en-us/articles/360024967612-Service-points-for-API-Integrations#step-1-) لإنشاء**مفتاح عمومي**و**مفتاح سري**.
3. ابحث عن**SendCloud**في الشريط الرائع.
4. أضف**المفتاح العام**في حقل "مفتاح واجهة برمجة التطبيقات" و**المفتاح السري**في الحقل "سر واجهة برمجة التطبيقات" في SendCloud DocType.
5. حدد الحقل**ممكّن**.
6. حفظ.

![Sendcloud API](https://docs.erpnext.com/files/sendcloud\_api.png)

#### 1.1 واجهة برمجة تطبيقات LetMeShip

1. التسجيل في [LetMeShip](https://www.letmeship.com/en/).
2. اتبع [هذه الخطوات](https://www.letmeship.com/en-de/shipping-api/) لإنشاء**معرف API**و**كلمة مرور API**.
3. ابحث عن**LetMeShip**في الشريط الرائع.
4. أضف**معرف API**و**كلمة مرور API**إلى LetMeShip DocType. تحقق من حقل**ممكّن**.
5. حفظ.

![LetMeShip API](https://docs.erpnext.com/files/letmeship\_api.png)

### 2. سمات

#### 2.1 مقارنة أسعار الشحن

بمجرد إرسال [شحنة](https://docs.erpnext.com/docs/v13/user/manual/en/stock/shipment) ، إذا تم تثبيت التطبيق ، فسيظهر الزر**جلب أسعار الشحن**. عند النقر ، ستحصل على قائمة بالخدمات جنبًا إلى جنب مع مزودي الخدمة والأسعار.

![أسعار الجلب](https://docs.erpnext.com/files/fetch\_rates.png)

يمكنك أيضًا إضافة الخدمات المستخدمة بشكل متكرر إلى**الخدمات المفضلة**الخاصة بك باستخدام**نوع خدمة الطرود**:

1.  بافتراض أن الخدمة المميزة هي الخدمة التي نستخدمها كثيرًا ، فلنقم بإضافتها إلى**خدماتنا المفضلة**

    ![خدمة مميزة](https://docs.erpnext.com/files/service\_highlight.png)
2. انتقل إلى**نوع خدمة الطرد**>**جديد**. أنشئ**خدمة طرد**جديدة. في حالتنا ، إنه "TNT".
3. أضف**نوع خدمة طرد**. في حالتنا ، سيكون "الاقتصاد".
4. أضف "الاقتصاد" إلى جدول**الاسم المستعار لنوع خدمة الطرود**أيضًا.
5. أضف وصفًا (اختياري).
6. قم بتمكين الحقل**إظهار في قائمة الخدمات المفضلة**. يحفظ.

الآن عند النقر فوق الزر**جلب أسعار الشحن**، سترى دائمًا الخدمة المميزة مسبقًا ضمن**الخدمات المفضلة**.

![الخدمة المفضلة](https://docs.erpnext.com/files/preferred\_service.png)

#### 2.2 إنشاء الشحن

بعد مقارنة الأسعار ، يمكنك المتابعة مع أي خدمة من خلال النقر فوق**تحديد**مقابل صف الخدمة المناسب. عند النقر ، يتم إنشاء شحنة تلقائيًا على النظام الأساسي لمزود الخدمة الخاص بك.

ستلاحظ أن قسم**معلومات الشحن**يتم تحديثه تلقائيًا ، بناءً على الشحنة التي تم إنشاؤها.

![Shipment Creation](https://docs.erpnext.com/files/create\_shipment.gif)

يمكنك أيضًا البحث عن معاملتك على النظام الأساسي لمزود الخدمة باستخدام حقل**معرّف الشحنة**.

![شحنة Packlink](https://docs.erpnext.com/files/packlink\_shipment.png)

#### 2.3 طباعة الملصقات

للاستفادة من زر**Print Shipping Label**، يجب إنشاء**معرّف الشحنة**في السجل الحالي.

![زر طباعة الملصق](https://docs.erpnext.com/files/print\_label\_button.png)

يمكنك بعد ذلك النقر فوقه وإنشاء ملصق الشحن الخاص بك.

![ملصق شحن وهمي](https://docs.erpnext.com/files/dummy\_shipping\_label.png)

يمكنك أيضًا تتبع حالة شحنتك بالنقر فوق**عرض**>**تتبع الحالة**.

> **ملاحظة**: قد لا تخدم الأنظمة الأساسية المدمجة حاليًا منطقتك. يرجى زيارة الروابط المرفقة ضدهم لمعرفة المزيد.
