---
description: restrict user based on child record
---

# تقييد المستخدم على أساس سجل الجدول الفرعي (الابن)

"" // تقييد مستودع معين على مدير المواد cur\_frm.cscript.custom\_validate = وظيفة (مستند) { if (frappe.user\_roles.indexOf ("مدير المواد") == - 1) {

```
    var limited_in_source = frappe.model.get_list ("تفاصيل إدخال المخزون" ،
        {الأصل: cur_frm.doc.name، s_warehouse: "Restricted"}) ؛

    var limited_in_target = frappe.model.get_list ("تفاصيل إدخال المخزون" ،
        {الأصل: cur_frm.doc.name، t_warehouse: "مقيد"})

    إذا (المقيدة_in_source.length || المقيدة_in_target.length) {
        frappe.msgprint (__ ("مدير المواد فقط يمكنه الدخول في المستودع المقيد")) ؛
        التحقق من صحتها = خطأ ؛
    }
}
```

} ""
