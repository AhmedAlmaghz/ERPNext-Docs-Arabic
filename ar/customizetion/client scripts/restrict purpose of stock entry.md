\n""
frappe.ui.form.on ("طلب المواد" ، "التحقق من صحة" ، الوظيفة (frm) {
    if (frappe.user == "user1@example.com" && frm.doc.purpose! = "استلام المواد") {
        frappe.msgprint ("مسموح لك فقط باستلام المواد") ؛
        frappe.throw (__ ("غير مسموح به")) ؛
    }
}
""