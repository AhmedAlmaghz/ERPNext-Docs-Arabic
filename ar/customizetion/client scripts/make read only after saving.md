\nاستخدم الطريقة `cur_frm.set_df_property` لتحديث عرض الحقل.

في هذا البرنامج النصي ، نستخدم أيضًا خاصية "__islocal" الخاصة بـ DocType للتحقق مما إذا كان المستند قد تم حفظه مرة واحدة على الأقل أو لم يتم حفظه مطلقًا. إذا كان "__islocal" يساوي "1" ، فهذا يعني أنه لم يتم حفظ المستند مطلقًا.

""
frappe.ui.form.on ("MyDocType"، "Refresh"، function (frm) {
    // استخدم طريقة is_new من frm للتحقق مما إذا كان المستند محفوظًا أم لا
    frm.set_df_property ("myfield"، "read_only"، frm.is_new ()؟ 0: 1)؛
}
""