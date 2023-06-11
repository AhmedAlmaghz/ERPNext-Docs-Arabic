---
description: hide buttons in form view
---

# اخفاء أزرار في عرض النموذج

في طلب المبيعات المقدم ، يمكنك رؤية أزرار مثل **تحديث العناصر** ،**الحالة**. هناك أيضًا العديد من الخيارات تحت الزر "إنشاء".

![برنامج نصي مخصص](https://docs.erpnext.com/files/sales\_order\_buttons.png)

يمكنك كتابة برنامج نصي مخصص كما هو موضح أدناه لإخفاء هذه الأزرار.

"" frappe.ui.form.on ("طلب المبيعات" ، { تحديث (frm) { setTimeout (() => { frm.remove\_custom\_button ("تحديث العناصر") ؛ frm.remove\_custom\_button ("إغلاق"، "الحالة") ؛ frm.remove\_custom\_button ("طلب العمل" ، "صنع") ؛ } ، 10) ؛ } }) ""
