\nفي طلب المبيعات المقدم ، يمكنك رؤية خيارات متعددة ضمن خيار "إنشاء":

![برنامج نصي مخصص](https://docs.erpnext.com/files/customize-button-all.png)

يمكنك استخدام هذا البرنامج النصي المخصص لإعادة تسمية الأزرار:

""
frappe.ui.form.on ("طلب المبيعات" ، {
    on_submit: الوظيفة (frm) {
    // console.log ('reloaded doc on submit')
        location.Reload ()
    } ،
    onload_post_render: الوظيفة (frm) {
        var bt = ["التسليم" ، "طلب العمل" ، "الفاتورة" ، "طلب المواد" ، "طلب المواد الخام" ، "طلب الشراء" ، "طلب الدفع" ، "الدفع" ، "المشروع" ، "الاشتراك" ]
        bt.forEach (الوظيفة (bt) {
            frm.page.remove_inner_button (bt، "إنشاء")
            }) ؛
        frm.page.add_inner_button ("طلب المواد الأولية" ، () => cur_frm.cscript.make_raw_material_request () ، "إنشاء")
        }
    }
) ؛
""

باستخدام هذا البرنامج النصي ، قمنا بإزالة / إخفاء الأزرار غير المرغوب فيها ، ثم أعدنا تسمية واحدة:

![برنامج نصي مخصص](https://docs.erpnext.com/files/customize-button-rename.png)

**ملاحظة:**لمعرفة المزيد حول واجهات برمجة تطبيقات JS ، تفضل بزيارة [وثائق frappe](https://frappe.io/docs/v13/user/en/api/form).

للتحقق من الطريقة التي تم استدعاؤها ، ستحتاج إلى التحقق من ملف JS لهذا النوع من المستندات. في هذا المثال ، لإعادة تسمية "طلب المواد الأولية" ، فإننا نشير إلى [هذا السطر](https://github.com/frappe/erpnext/blob/782f45ae5f272173b5daadb493d40cf7ccf131b4/erpnext/selling/doctype/sales_order/sales_order.js L167).