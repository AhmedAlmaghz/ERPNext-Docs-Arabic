\nفي طلب المبيعات المقدم ، يمكنك رؤية أزرار مثل ** تحديث العناصر ** ، ** الحالة **. هناك أيضًا العديد من الخيارات تحت الزر "إنشاء".

! [برنامج نصي مخصص] (https://docs.erpnext.com/files/sales_order_buttons.png)

يمكنك كتابة برنامج نصي مخصص كما هو موضح أدناه لإخفاء هذه الأزرار.

""
frappe.ui.form.on ("طلب المبيعات" ، {
    تحديث (frm) {
    setTimeout (() => {
        frm.remove_custom_button ("تحديث العناصر") ؛
        frm.remove_custom_button ("إغلاق"، "الحالة") ؛
        frm.remove_custom_button ("طلب العمل" ، "صنع") ؛
        } ، 10) ؛
    }
})
""