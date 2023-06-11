\n\n## إعداد النسخ الاحتياطية لـ Dropbox

نوصي العملاء دائمًا بالاحتفاظ بنسخة احتياطية من بياناتهم في ERPNext. يتم تنزيل النسخة الاحتياطية لقاعدة البيانات في شكل ملف SQL. إذا لزم الأمر ، يمكن استعادة ملف SQL للنسخ الاحتياطي هذا في حساب ERPNext آخر أيضًا.

يمكنك أتمتة تنزيل نسخة احتياطية لقاعدة البيانات لحساب ERPNext الخاص بك في حساب Dropbox الخاص بك.

لإعداد Dropbox Backup ،

> الصفحة الرئيسية> عمليات التكامل> إعدادات Dropbox

## تختلف الخطوات بالنسبة للإصدارات المدارة من ERPnext والإصدارات مفتوحة المصدر

### تعليمات الإصدار المُدار من ERPnext

#### الخطوة 1: ضبط التردد

قم بتعيين التردد لتنزيل نسخة احتياطية في حساب Dropbox الخاص بك.

! [ضبط التردد] (https://docs.erpnext.com/files/setup-backup-frequency.png)

#### الخطوة 2: السماح بالوصول إلى Dropbox

بعد تحديد التردد وتحديث التفاصيل الأخرى ، انقر فوق "السماح بوصول Dropbox". عند النقر فوق هذا الزر ، سيتم فتح صفحة تسجيل الدخول إلى Dropbox في علامة التبويب الجديدة. قد يتطلب ذلك منك السماح بالانبثاق المنبثق لحساب ERPNext الخاص بك.

#### الخطوة الثالثة: تسجيل الدخول إلى Dropbox

قم بتسجيل الدخول إلى حساب Dropbox الخاص بك عن طريق إدخال بيانات اعتماد تسجيل الدخول.

! [تسجيل الدخول] (https://docs.erpnext.com/files/dropbox-2.png)

#### الخطوة 4: السماح

عند تسجيل الدخول بنجاح ، ستجد رسالة تأكيد على النحو التالي. انقر فوق "السماح" للسماح لحساب ERPNext الخاص بك بالوصول إلى حساب Dropbox الخاص بك.

! [سماح] (https://docs.erpnext.com/files/dropbox-3.png)

باستخدام هذا ، سيتم إنشاء مجلد يسمى "ERPNext" في حساب Dropbox الخاص بك ، وسيبدأ التنزيل التلقائي لقاعدة البيانات فيه.

## تعليمات إصدار مفتوح المصدر

#### الخطوة 1: تسجيل الدخول إلى منطقة Dropbox Developer

[https://www.dropbox.com/developers/apps](https://www.dropbox.com/developers/apps)

#### الخطوة الثانية: إنشاء تطبيق Dropbox جديد

! [إنشاء جديد] (https://docs.erpnext.com/files/dropbox-open-3.png)

#### الخطوة 3: املأ التفاصيل الخاصة بتطبيقك الجديد

! [اختر Dropbox API واكتب كمجلد APP] (https://docs.erpnext.com/files/dropbox-open-1.png) -! [Setup APP Name] (https://docs.erpnext.com/ files / dropbox-open-2.png)

#### الخطوة 4: أدخل نطاقك الخاص Redirect URI

`https: // {yourwebsite.com} / api / method / frappe.integrations.doctype.dropbox_settings.dropbox_settings.dropbox_auth_finish`! [تعيين عنوان URL لإعادة التوجيه] (https://docs.erpnext.com/files/dropbox_redirect_uri.png)

#### الخطوة 5: في نافذة جديدة ، افتح صفحة إعدادات Dropbox في تثبيت ERPnext

#### الخطوة 6: ضبط تردد النسخ الاحتياطي والبريد الإلكتروني

قم بتعيين التردد لتنزيل النسخ الاحتياطية لموقعك على حساب Dropbox الخاص بك. ! [ضبط التردد] (https://docs.erpnext.com/files/setup-backup-frequency.png)

#### الخطوة 7: مفاتيح الإدخال من نافذة تطبيق Dropbox

من صفحة تطبيق Dropbox ، أدخل مفتاح التطبيق وسر التطبيق (غير المخفي) في صفحة إعدادات ERPnext Dropbox.

بدلاً من ذلك ، يمكنك إدخاله يدويًا في `sites / {sitename} / site_config.json` على النحو التالي ،

        "{" db_name ":" demo "،" db_password ":" DZ1Idd55xJ9qvkHvUH "،" dropbox_access_key ":" ACCESSKEY "،" dropbox_secret_key ":" SECRECTKEY "}`
        
    

#### الخطوة 8: انقر فوق "حفظ" قبل المتابعة !!!

#### الخطوة التاسعة: بعد الحفظ ، انقر على "السماح بوصول Dropbox"

سيتم فتح صفحة تسجيل الدخول إلى Dropbox في علامة التبويب الجديدة. قد يتطلب ذلك منك السماح بالانبثاق المنبثق لحساب ERPNext الخاص بك.

#### الخطوة 11: السماح بالوصول إلى Dropbox

عند تسجيل الدخول بنجاح ، ستجد رسالة تأكيد على النحو التالي. انقر فوق "السماح" للسماح لحساب ERPNext الخاص بك بالوصول إلى حساب Dropbox الخاص بك. ! [سماح] (https://docs.erpnext.com/files/dropbox-3.png)

#### الخطوة 12: تأكيد عمل النسخ الاحتياطية

من صفحة ERPnext Dropbox ، انقر فوق "Take Backup Now" ثم انتقل إلى عرض ملفات Dropbox. من المفترض أن ترى مجلدًا جديدًا في Dropbox باسم "Apps" وداخله مجلد {New App}. يجب أن يكون داخلها مجلدات نسخ احتياطي لكل من الملفات وقاعدة البيانات. لذلك بالنسبة لتطبيق يسمى "erpnext" ، فيما يلي مواقع المجلدات:

""
ملفات قاعدة البيانات: / Apps / erpnext / database
الملفات العامة: / Apps / erpnext / files
الملفات الخاصة: / Apps / erpnext / private / files
""

> ** ملاحظة **: إذا تجاوز حجم النسخ الاحتياطي المضغوط 1 جيجا بايت (جيجا بايت) ، فسيقوم النظام بتحميل أحدث نسخة احتياطية متاحة إلى Dropbox بدلاً من إنشاء ملف نسخ احتياطي جديد.