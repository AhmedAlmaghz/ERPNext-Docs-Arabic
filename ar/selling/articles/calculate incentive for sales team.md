\nيمكنك حساب الحوافز لفريق المبيعات باستخدام البرامج النصية المخصصة.

يمكن استخدامها في أي معاملة مبيعات مع جدول ** فريق المبيعات **:

""
cur_frm.cscript.custom_validate = وظيفة (مستند) {
    // حساب الحوافز لكل شخص في الصفقة
    total_incentive = 0
    $ .each (wn.model.get ("فريق المبيعات"، {parent: doc.name}) ، الوظيفة (i، d) {

        // حساب الحافز
        var stimive_percent = 2 ؛
        إذا (doc.grand_total> 400) حافز_بيرسينت = 4 ؛

        // الحافز الفعلي
        د - الحوافز = flt (doc.grand_total) * حافز_بيرسنت / 100 ؛
        total_incentive + = flt (حوافز د)
    }) ؛

    doc.total_incentive = total_incentive ؛
}
""