## تكامل Amazon SP-API

يسحب Amazon Connector طلبات المنتجات والمبيعات من سوق Amazon. تتم مزامنة المنتجات وأوامر المبيعات بشكل تسلسلي. يجب عليك مزامنة المنتجات قبل مزامنة أوامر المبيعات.

## كيفية إعداد موصل Amazon SP-API؟

تم نقل Amazon Connector من ERPNext ومتاحًا من خلال تطبيق Frappe على [Frappe Cloud Marketplace](https://frappe Cloud Marketplace](https://frappecloud.com/marketplace/apps/ecommerce_integrations)

### تثبيت التطبيق

* إذا كنت تستضيف موقع ERPNext الخاص بك على Frappe Cloud ، فيمكنك تثبيت التطبيق بسرعة من خلال الانتقال إلى لوحة التحكم في موقعك. التطبيق متاح في [Frappe Cloud Marketplace](https://frappecloud.com/marketplace/apps/ecommerce_integrations)
* إذا كان موقعك مستضافًا بواسطة Frappe ، فيرجى رفع تذكرة دعم لتثبيت التطبيق على موقعك.
* إذا كنت تستضيف ERPNext بنفسك ، يمكنك تثبيت التطبيق باستخدام مقعد Frappe. راجع [وثائق مقاعد البدلاء](https://frappeframework.com/docs/user/en/bench/frappe-commands#app-installation) لتثبيت تطبيقات Frappe. "التجارة الإلكترونية_تكامل get-app - الفرع الرئيسي"

يتم استضافة مستودع التطبيق على GitHub: [http://github.com/frappe/ecommerce\_integrations/](http://github.com/frappe/ecommerce_integrations/)

### إعداد بيانات الاعتماد في ERPNext

يمكنك طلب بيانات اعتماد المطور من Amazon SP بمجرد أن تصبح بائعًا مسجلاً على موقعه على الويب. لمزيد من التفاصيل حول ذلك ، انقر [هنا](https://developer.amazonservices.com/).

#### 1. إعداد بيانات اعتماد SP-API

أدخل IAM ARN و Refresh Token و Client ID و Client Secret و AWS Access Key و AWS Secret Key و Country. ![بيانات اعتماد الإعداد](https://docs.erpnext.com/files/amazon_sp_api_settings_1..png)

#### 2. قم بإعداد تفاصيل الطلب

قم بإعداد الشركة والمستودع ومجموعة العناصر الأصلية وقائمة الأسعار ومجموعة العملاء والإقليم ونوع العميل ومجموعة الحسابات. تُستخدم مجموعة الحساب في الاحتفاظ بالعمولة والضرائب وما إلى ذلك التي تفرضها أمازون. ![تكوينات ERPNext](https://docs.erpnext.com/files/amazon_sp_api_settings_2..png)

#### 3. إعداد تكوينات المزامنة

باستخدام تاريخ ما بعد ، يمكنك مزامنة المنتجات والأوامر التي تم إنشاؤها بعد تاريخ معين. في حالة استيراد الكثير من البيانات التاريخية ، يُقترح أن تبدأ بالترتيب الزمني العكسي للتاريخ التالي واستيراد البيانات في أجزاء صغيرة. ![تكوينات المزامنة](https://docs.erpnext.com/files/amazon_sp_api_settings_3..png) بعد إعداد جميع التكوينات ، انقر فوق "تمكين أمازون" واحفظ الإعدادات. أنت الآن جاهز لاستخدام التكامل.

#### 4. منتجات المزامنة

انقر فوق هذا الزر لمزامنة المنتجات. بمجرد نجاح ذلك ، يجب أن ترى منتجات Amazon الخاصة بك كعناصر في ERPNext.

![تكوينات المزامنة](https://docs.erpnext.com/files/amazon_mws_settings_4.png)![تكوينات المزامنة](https://docs.erpnext.com/files/amazon_mws_settings_5.png)

#### 5. أوامر المزامنة

انقر فوق هذا الزر لمزامنة أوامر المبيعات. بمجرد نجاح ذلك ، يجب أن ترى طلبات Amazon الخاصة بك كأوامر مبيعات في ERPNext. يمكنك أيضًا إعداد برنامج جدولة لمزامنة الطلبات تلقائيًا.

> في حالة عدم قدرة حساب المطور الخاص بك على الوصول إلى معلومات التعريف الشخصية. سيتم تخزين اسم العميل كمجموعة من اسم المشتري + <معرف الطلب>.

![تكوينات المزامنة](https://docs.erpnext.com/files/amazon_mws_settings_6.png)

### ملحوظة

لن يتعامل الموصل مع إلغاء الطلب. إذا قمت بإلغاء أي طلب في Amazon ، فعليك يدويًا إلغاء طلب المبيعات المعني والمستندات الأخرى في ERPNext.