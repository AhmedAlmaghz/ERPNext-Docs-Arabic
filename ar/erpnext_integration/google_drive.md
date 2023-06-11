\n## جوجل درايف التكامل

يوفر ERPNext تكاملاً مع Google Drive حتى يتمكن جميع المستخدمين من نسخ بياناتهم احتياطيًا إلى Google Drive.

## كيفية إعداد Google Drive Integration

للسماح لـ ERPNext بتحميل النسخ الاحتياطية على Google Drive ، تحتاج إلى تفويض ERPNext لتحميل الملفات إلى Google Drive. تم إعداد Google Drive Integration من خلال الخطوات التالية:

* أنشئ بيانات اعتماد OAuth 2.0 عبر [إعدادات Google] (https://docs.erpnext.com/docs/v13/user/manual/en/erpnext_integration/google_settings).
* في قائمة Google Drive ، انقر فوق جديد. أدخل اسم مجلد النسخ الاحتياطي لحفظ النسخ الاحتياطية في Google Drive ، وتكرار النسخ الاحتياطي والبريد الإلكتروني للشخص الذي يتم إرسال البريد الإلكتروني إليه لإخطار حالة النسخ الاحتياطي ثم احفظه. انقر الآن على ** تخويل الوصول إلى Drive ** للسماح لـ ERPNext بدفع الملفات إلى Google Drive.
* بمجرد التفويض ، يمكنك حفظ النسخة الاحتياطية على Google Drive.

## كيفية استخدام Google Drive Integration

### تحميل نسخة احتياطية على Google Drive

* بمجرد نجاح Google Drive Integration ، يمكنك تحميل النسخة الاحتياطية للنظام وكذلك جميع ملفاتك العامة والخاصة إلى Google Drive.
* لنسخ البيانات احتياطيًا إلى Google Drive ، انقر فوق ** Take Backup **. ستعمل عملية النسخ الاحتياطي في الخلفية وسيتم إخطارك بحالة النسخ الاحتياطي. ! [] (https://docs.erpnext.com/files/google_drive.gif)

> ** ملاحظة **: إذا تجاوز حجم النسخ الاحتياطي المضغوط 1 جيجا بايت (جيجا بايت) ، فسيقوم النظام بتحميل أحدث نسخة احتياطية متوفرة على Google Drive بدلاً من إنشاء ملف نسخ احتياطي جديد.