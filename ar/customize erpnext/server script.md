\n\n## البرنامج النصي للخادم

** يتيح لك البرنامج النصي للخادم تعريف Python Script ديناميكيًا الذي يتم تنفيذه على الخادم في حدث مستند أو واجهة برمجة تطبيقات **

> مقدمة في الإصدار 12

## 1 \. كيفية إنشاء برنامج نصي للخادم

لإنشاء برنامج نصي للخادم

1. إذا كان موقعك مستضافًا على [erpnext.com] (https://erpnext.com/) ، فاتصل بالدعم لتنشيط Server Script. في حالة الحسابات المستضافة ذاتيًا ، قم بتعيين "server_script_enabled" على أنه صحيح في site \ _config.json لموقعك.
2. لإضافة / تحرير البرنامج النصي للخادم ، تأكد من أن دورك هو مدير النظام.
3. أنشئ برنامجًا نصيًا جديدًا للخادم عبر "New Server Script" في شريط الأدوات.
4. حدد نوع البرنامج النصي للخادم: حدث المستند وواجهة برمجة التطبيقات واستعلام الأذونات.
5. قم بتعيين نوع المستند واسم الحدث أو اسم الطريقة والبرنامج النصي والحفظ.

## 2 \. سمات

### 2.1 تمكين البرنامج النصي للخادم

يجب تمكين البرنامج النصي للخادم عبر site \ _config.json

""
مقعد - site site1.local set-config server_script_enabled true
""

### 2.2 توثيق الأحداث

بالنسبة إلى البرامج النصية التي سيتم استدعاؤها عبر أحداث المستند ، يجب عليك تعيين نوع المستند المرجعي واسم الحدث لتعريف المشغل

* قبل الإدراج
* قبل الحفظ
* بعد الحفظ
* قبل الإرسال
* بعد الإرسال
* قبل الإلغاء
* بعد الإلغاء
* قبل الحذف
* بعد الحذف
* قبل الحفظ (المستند المقدم)
* بعد الحفظ (المستند المقدم)

### 2.3 البرامج النصية لواجهة برمجة التطبيقات

يمكنك إنشاء واجهة برمجة تطبيقات جديدة يمكن الوصول إليها عبر `api / method / [methodname]` بنوع البرنامج النصي "API"

إذا كنت تريد أن يصل المستخدم الضيف إلى واجهة برمجة التطبيقات ، فيجب عليك التحقق من "السماح للضيف"

يمكن ضبط الاستجابة عبر كائن `frappe.response [" message "]`

### 2.4 استعلام الإذن

يسمح لك هذا النوع من البرامج النصية بإضافة شروط مخصصة في عبارة أين لاستعلام قائمة DocType.

على سبيل المثال ، لنفترض أنك تريد إظهار قائمة سجلات ToDo للمستخدم فقط إذا قام بتعيين السجل أو تم تعيينه لهم. يمكن تنفيذ ذلك من خلال البرنامج النصي التالي:

""
الشروط = 'المالك = {مستخدم} أو تعيين_بي = {مستخدم}'. تنسيق (مستخدم = frappe.db.escape (مستخدم))
""

سيبدو طلب البحث "select" الناتج كما يلي:

""
حدد * من "tabToDo" حيث المالك = 'faris@erpnext.com' أو assign_by = 'faris@erpnext.com'
""

الآن ، سيعرض عرض قائمة ToDo السجلات المقيدة. سيؤدي هذا أيضًا إلى تقييد النتائج المعروضة في حقول الارتباط.

### 2.5 الأمن

يستخدم Frappe Framework مكتبة RestrictedPython لتقييد الوصول إلى الأساليب المتاحة لنصوص الخادم. تتوفر فقط الطرق الآمنة المذكورة أدناه في البرامج النصية للخادم

""
وحدة json # json
ديكت # ديكت داخلي
_ # طريقة المترجم
_dict # frappe._dict الأسلوب الداخلي
frappe.flags # أعلام عالمية

# تنسيق
frappe.format # frappe.format_value (value، dict (fieldtype = 'Currency'))
frappe.format_value # frappe.format_value (value، dict (fieldtype = 'Currency'))
frappe.date_format # تنسيق التاريخ الافتراضي
يعود تاريخ frappe.format_date # كـ "1st September 2019"

# حصة
frappe.form_dict # معلمات النموذج / الطلب
frappe.request # طلب كائن
frappe.response # كائن الاستجابة
frappe.session.user # المستخدم الحالي
frappe.session.csrf_token # رمز CSRF للدورة الحالية
frappe.user # المستخدم الحالي
frappe.get_fullname # الاسم الكامل للمستخدم الحالي
frappe.get_gravatar # frappe.utils.get_gravatar_url
frappe.full_name = # الاسم الكامل للمستخدم الحالي

# ORM
frappe.get_meta # get metadata object
frappe.get_doc
frappe.get_cached_doc
frappe.get_list
frappe.get_all
frappe.get_system_settings

# ديسيبل
frappe.db.get_list
frappe.db.get_all
frappe.db.get_value
frappe.db.get_single_value
frappe.db.get_default
frppe.db.escape
frppe.db
frappe.db.commit

# خدمات
frappe.msgprint # msgprint
frappe.get_hooks # خطافات التطبيق
frappe.utils # طرق في frappe.utils
frappe.render_template # frappe.render_template،
frappe.get_url # frappe.utils.get_url
frappe.sendmail # إرسال بريد إلكتروني عبر البرنامج النصي للخادم
frappe.get_print # الحصول على pdf لمستند
frappe.attach_print # إرفاق PDF برسالة بريد إلكتروني
منفذ socketio_port # للمقبس
style.border_color # '# d1d8dd'
get_next_link
تنظيف
guess_mimetype = mimetypes.guess_type ،
html2text = html2text ،
dev_server # صحيح إذا كان في وضع المطور
run_script # قم بتشغيل برنامج نصي آخر للخادم

# مخبأ
frappe.cache.set_value
frappe.cache.get_value
مجموعة فرابي
frappe.cache.hget
""

## 3 \. أمثلة

### 3.1 تغيير قيمة الخاصية قبل التغيير

نوع البرنامج النصي: قبل الحفظ

""
إذا كان "اختبار" في doc.description:
    doc.status = "مغلق"
""

### 3.2 التحقق المخصص

نوع البرنامج النصي: "قبل الحفظ"

""
إذا "تحقق" في doc.description:
    رفع frppe.ValidationError
""

### 3.3. إنشاء تلقائي للمهام

نوع البرنامج النصي: "بعد الحفظ"

""
إذا كان doc.allocated_to:
    frappe.get_doc (ديكت (
        DOCTYPE = 'ToDo'
        المالك = doc.allocated_to ،
        الوصف = doc.subject
    )).إدراج()
""

### 3.4 API

* نوع البرنامج النصي: API
* اسم الطريقة: `test_method`

""
frappe.response ['message'] = "مرحبًا"
""

الطلب: `/ api / method / test_method`