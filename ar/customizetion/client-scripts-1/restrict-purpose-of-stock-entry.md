---
description: restrict purpose of stock entry
---

# تقييد الغرض من قيد المخزون

"" frappe.ui.form.on ("طلب المواد" ، "التحقق من صحة" ، الوظيفة (frm) { if (frappe.user == "user1@example.com" && frm.doc.purpose! = "استلام المواد") { frappe.msgprint ("مسموح لك فقط باستلام المواد") ؛ frappe.throw (\_\_ ("غير مسموح به")) ؛ } } ""
