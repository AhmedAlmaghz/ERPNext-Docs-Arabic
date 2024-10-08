---
description: using custom domain on erpnext
---

# استخدام الدومين المخصص في ERPNext

إذا كنت قد اشتركت في أي من الخطط علي  HisabCloud.com ، فيمكنك جعلنا نخدم موقعك على نطاقك المخصص (على سبيل المثال على http://example.com). يمكّن هذا موقع الويب الخاص بك من أن يتم تقديمه في مجال مخصص.

لتمكين هذه الميزة ، سيتعين عليك أولاً تعديل إعدادات DNS الخاصة بنطاقك على النحو التالي.

* أنشئ سجل CNAME لنطاق فرعي (www في معظم الحالات) إلى {youraccountname} .hiabcloud.com
* إذا كنت تريد خدمة موقع الويب على نطاق مجرد (مثل http://example.com) ، فعيِّن إعادة توجيه عنوان URL إلى http://www.example.com وليس سجل CNAME. قد يؤدي إنشاء سجل CNAME في هذه الحالة إلى عواقب غير متوقعة بما في ذلك عدم قدرتك على تلقي رسائل البريد الإلكتروني بعد الآن.

بعد إعداد سجلات DNS ، سيتعين عليك رفع تذكرة دعم عن طريق إرسال بريد إلكتروني إلى support@hisabcloud.com وسنأخذها من هناك.

**ملاحظة**: نحن لا ندعم HTTPS في المجالات المخصصة. يتيح HTTPS التشفير من طرف إلى طرف (من متصفحك إلى خادمنا). على الرغم من أنه ليس مهمًا لموقع الويب ، إلا أننا نوصي بشدة بعدم استخدام تطبيق ERPNext عبر بروتوكول غير مشفر. لتكون آمنًا ، استخدم دائمًا ERP على عنوان erpnext.com الخاص بك.
