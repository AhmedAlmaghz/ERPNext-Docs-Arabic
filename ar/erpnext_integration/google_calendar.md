\n## تكامل تقويم Google

يوفر ERPNext تكاملاً مع تقويم Google حتى يتمكن جميع المستخدمين من مزامنة أحداث تقويم Google الخاصة بهم مع ERPNext.

## كيفية إعداد Google Calendar Integration

للسماح بالمزامنة مع تقويم Google ، تحتاج إلى تفويض ERPNext للحصول على بيانات أحداث التقويم من Google. تم إعداد تكامل تقويم Google بالخطوات التالية:

* أنشئ بيانات اعتماد OAuth 2.0 عبر [إعدادات Google] (https://docs.erpnext.com/docs/v13/user/manual/en/erpnext_integration/google_settings).
* في قائمة تقويم Google ، انقر فوق جديد. أدخل اسم التقويم والمستخدم الذي تريد المزامنة له ثم احفظه.
* بناءً على البيانات التي تريد مزامنتها ، يمكنك تحديد ما يلي
    * سحب من تقويم Google - مزامنة كل الأحداث من تقويم Google إلى ERPNext.
    * الدفع إلى تقويم Google - مزامنة كل الأحداث من ERPNext إلى تقويم Google.
* انقر الآن على ** تخويل الوصول إلى التقويم ** لتفويض ERPNext للحصول على بيانات أحداث التقويم من Google.
* بمجرد التفويض ، يمكنك مزامنة حدث تقويم Google يدويًا أو السماح لـ ERPNext بمزامنة جهات اتصال Google يوميًا.

## كيفية استخدام Google Calendar Integration

### إنشاء حدث في ERPNext

### مزامنة الأحداث من تقويم Google

* بمجرد نجاح دمج تقويم Google ، ستتم مزامنة جميع الأحداث في تقويم Google إذا تم تحديد "سحب من تقويم Google".
* مزامنة الأحداث من تقويم Google إلى ERPNext! [] (https://docs.erpnext.com/files/gc-sync.gif)