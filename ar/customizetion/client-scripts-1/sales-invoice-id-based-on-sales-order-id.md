---
description: sales invoice id based on sales order id
---

# رقم تسلسل فاتورة المبيعات إعتماداً على رقم تسلسل طلب المبيعات

يسمح لك البرنامج النصي الوارد أدناه بتطبيق سلسلة التسمية على فاتورة المبيعات ، مثل تلك الخاصة بأمر المبيعات المقابل. تستخدم فاتورة المبيعات البادئة M- لكن الرقم يكرر نفسه من اسم أمر المبيعات.

مثال: إذا كان معرف طلب المبيعات هو SO-12345 ، فسيتم تعيين معرف فاتورة المبيعات المقابل كـ M-12345.

"" frappe.ui.form.on ("فاتورة المبيعات" ، "التحديث" ، الوظيفة (frm) { var sales\_order = frm.doc.items \[0] .sales\_order.replace ("M"، "M-") ؛ إذا (! frm.is\_new () && sales\_order && frm.doc.name! == sales\_order) { frappe.call ({ الطريقة: 'frappe.model.rename\_doc.rename\_doc' ، أرغس: { DOCTYPE: frm.doctype ، قديم: frm.docname ، "جديد": sales\_order، "دمج": خطأ } ، }) ؛ } }) ؛ ""
