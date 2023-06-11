### نموذج نص برمجي لجلب تاريخ انتهاء الصلاحية \ _حقل التاريخ من نوع مستند الدُفعة إلى جدول عنصر فاتورة المبيعات

الخطوة 1: إنشاء برنامج نصي مخصص لنوع _**فاتورة المبيعات**_ (الأصل)

الخطوة 2: نص على النحو التالي وحفظ

""
frappe.ui.form.on ("عنصر فاتورة المبيعات"، "batch_no"، function (frm، cdt، cdn) {
    var d = locals [cdt] [cdn] ؛
        frappe.db.get_value ("Batch"، {"name": d.batch_no}، "expiry_date"، الوظيفة (القيمة) {
            d.expiry_date = value.expiry_date ؛
        }) ؛
}) ؛
""