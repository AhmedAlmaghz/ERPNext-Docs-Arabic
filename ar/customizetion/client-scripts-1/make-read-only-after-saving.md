---
description: make read only after saving
---

# جعله للقراءة فقط بعد الحفظ

استخدم الطريقة `cur_frm.set_df_property` لتحديث عرض الحقل.

في هذا البرنامج النصي ، نستخدم أيضًا خاصية "\_\_islocal" الخاصة بـ DocType للتحقق مما إذا كان المستند قد تم حفظه مرة واحدة على الأقل أو لم يتم حفظه مطلقًا. إذا كان "\_\_islocal" يساوي "1" ، فهذا يعني أنه لم يتم حفظ المستند مطلقًا.

"" frappe.ui.form.on ("MyDocType"، "Refresh"، function (frm) { // استخدم طريقة is\_new من frm للتحقق مما إذا كان المستند محفوظًا أم لا frm.set\_df\_property ("myfield"، "read\_only"، frm.is\_new ()؟ 0: 1)؛ } ""
