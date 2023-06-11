\n""
// تقييد مستودع معين على مدير المواد
cur_frm.cscript.custom_validate = وظيفة (مستند) {
    if (frappe.user_roles.indexOf ("مدير المواد") == - 1) {

        var limited_in_source = frappe.model.get_list ("تفاصيل إدخال المخزون" ،
            {الأصل: cur_frm.doc.name، s_warehouse: "Restricted"}) ؛

        var limited_in_target = frappe.model.get_list ("تفاصيل إدخال المخزون" ،
            {الأصل: cur_frm.doc.name، t_warehouse: "مقيد"})

        إذا (المقيدة_in_source.length || المقيدة_in_target.length) {
            frappe.msgprint (__ ("مدير المواد فقط يمكنه الدخول في المستودع المقيد")) ؛
            التحقق من صحتها = خطأ ؛
        }
    }
}
""