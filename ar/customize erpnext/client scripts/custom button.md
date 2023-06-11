\n## إضافة زر مخصص

""
frappe.ui.form.on ("الحدث" ، "التحديث" ، الوظيفة (frm) {
    frm.add_custom_button (__ ("Do Something") ، الوظيفة () {
        // عند النقر فوق هذا الزر ، قم بذلك

        var subject = frm.doc.subject ؛
        var event_type = frm.doc.event_type ؛

        // افعل شيئًا بهذه القيم ، مثل طلب أياكس
        / / أو استدعاء وظيفة فرابيه جانب الخادم باستخدام frappe.call
        .ajax $ ({
            url: "http://example.com/just-do-it"،
            بيانات: {
                "الموضوع الموضوع،
                "event_type": نوع الحدث
            }

            // اقرأ المزيد عن صيغة $ .ajax على http://api.jquery.com/jquery.ajax/

        }) ؛
    }) ؛
}) ؛
""