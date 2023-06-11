\nيسمح لك البرنامج النصي الوارد أدناه بتطبيق سلسلة التسمية على فاتورة المبيعات ، مثل تلك الخاصة بأمر المبيعات المقابل. تستخدم فاتورة المبيعات البادئة M- لكن الرقم يكرر نفسه من اسم أمر المبيعات.

مثال: إذا كان معرف طلب المبيعات هو SO-12345 ، فسيتم تعيين معرف فاتورة المبيعات المقابل كـ M-12345.

""
frappe.ui.form.on ("فاتورة المبيعات" ، "التحديث" ، الوظيفة (frm) {
    var sales_order = frm.doc.items [0] .sales_order.replace ("M"، "M-") ؛
    إذا (! frm.is_new () && sales_order && frm.doc.name! == sales_order) {
        frappe.call ({
        الطريقة: 'frappe.model.rename_doc.rename_doc' ،
        أرغس: {
            DOCTYPE: frm.doctype ،
            قديم: frm.docname ،
            "جديد": sales_order،
            "دمج": خطأ
        } ،
    }) ؛
    }
}) ؛
""