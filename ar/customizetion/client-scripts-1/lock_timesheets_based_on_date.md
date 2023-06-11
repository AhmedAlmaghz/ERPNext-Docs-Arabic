---
description: lock timesheets based on date
---

# قفل ورقة تسجيل الحضور بناءاً على تاريخ

لنفترض أنك تريد أن يملأ جميع الموظفين جداول المواعيد بحلول يوم الجمعة من كل أسبوع. واسمح فقط للمستخدمين الذين لديهم دور "مدير المشاريع" بتعديل أو إضافة جداول زمنية للأيام السابقة لآخر جمعة. سينفذ البرنامج النصي المخصص أدناه هذه الميزة.

"" frappe.ui.form.on ("Timesheet"، "validate"، function (frm) { if (frappe.user\_roles.indexOf ("مدير المشاريع") == -1) { const t = new Date (). getDate () + (6 - new Date (). getDay () - 1) - 7 ؛ const lastFriday = تاريخ جديد () ؛ lastFriday.setDate (ر) ،

```
    دعونا dd = lastFriday.getDate () ،
    دع مم = lastFriday.getMonth () + 1 ؛
    دع yyyy = lastFriday.getFullYear () ،

    frm.doc.time_logs.forEach (تسجيل => {
        إذا (تاريخ جديد (log.from_time) <= lastFriday) {
            frappe.throw ("لا يمكنك إضافة جدول زمني للتواريخ قبل الجمعة الماضية" + dd + "/" + mm + "/" + yyyy + ". يرجى الاتصال بمدير المشروع.")؛
        }
    })
}
```

}) ""
