---
description: update date field based on value in other date field
---

# تحديث حقل التاريخ بالإعتماد على قيمة حقل تاريخ آخر

يقوم البرنامج النصي الموضح أدناه بتعيين القيمة تلقائيًا لحقل التاريخ ، بناءً على القيمة الموجودة في حقل تاريخ آخر.

مثال: يجب تحديد تاريخ استحقاق الإنتاج ليومين قبل تاريخ التسليم. لنفترض أن تاريخ التسليم للمشروع قد تم تحديده بالفعل ، وهناك حقل "تاريخ استحقاق الإنتاج" كنوع حقل "تاريخ" موجود بالفعل في النموذج. يجب أن يضمن تطبيق النص التالي تحديث تاريخ استحقاق الإنتاج تلقائيًا إلى يومين قبل تاريخ التسليم.

"" cur\_frm.cscript.custom\_delivery\_date = function (doc، cdt، cd) { cur\_frm.set\_value ("production\_due\_date"، frappe.datetime.add\_days (doc.delivery\_date، -2)) ؛ } ""
