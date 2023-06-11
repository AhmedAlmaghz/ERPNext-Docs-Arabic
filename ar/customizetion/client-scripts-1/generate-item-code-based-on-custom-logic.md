---
description: generate item code based on custom logic
---

# إنشاء رمز العنصر على أساس منطق مخصص

أضف هذا البرنامج النصي المخصص في البرنامج النصي لـ**العنصر**، بحيث يتم إنشاء رمز العنصر الجديد قبل حفظ العنصر مباشرةً.

"" cur\_frm.cscript.custom\_validate = وظيفة (مستند) { // مسح item\_code (الاسم من item\_code) doc.item\_code = "" ؛

```
// أول حرفين على أساس item_group
التبديل (doc.item_group) {
    الحالة "الاختبار أ":
        doc.item_code = "TA" ؛
        استراحة؛
    الحالة "الاختبار ب":
        doc.item_code = "TB" ؛
        استراحة؛
    تقصير:
        doc.item_code = "XX" ؛
}

// أضف الحرفين التاليين بناءً على العلامة التجارية
مفتاح (doc.brand) {
    الحالة "العلامة التجارية أ":
        doc.item_code + = "BA" ؛
        استراحة؛
    الحالة "العلامة التجارية ب":
        doc.item_code + = "BB" ؛
        استراحة؛
    تقصير:
        doc.item_code + = "BX" ؛
}
```

} ""
