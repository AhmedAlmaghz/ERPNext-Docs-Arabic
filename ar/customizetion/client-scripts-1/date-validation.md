## التحقق من صحة التاريخ

""
    frappe.ui.form.on ("المهمة" ، "التحقق من الصحة" ، الوظيفة (frm) {
        إذا (frm.doc.from_date <get_today ()) {
            frappe.msgprint (__ ("لا يمكنك تحديد التاريخ الماضي في من تاريخ")) ؛
            frappe.validated = خطأ ؛
        }
    }) ؛
""