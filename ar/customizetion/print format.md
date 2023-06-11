## تخصيص تنسيق الطباعة

**تنسيقات الطباعة هي التخطيطات التي يتم إنشاؤها عندما تريد طباعة معاملة أو إرسالها بالبريد الإلكتروني.**

هذه الميزة مفيدة لجميع المعاملات في ERPNext مثل جميع معاملات البيع والشراء ووثائق الموارد البشرية وغير ذلك الكثير.

في ERPNext ، هناك ثلاثة أنواع من تنسيقات الطباعة ، وهي تنسيق الطباعة القياسي وتنسيق الطباعة المخصص وتنسيق طباعة HTML.

## تنسيق الطباعة القياسي

سيكون لكل نوع مستند قابل للطباعة في ERPNext تنسيق طباعة قياسي خاص به يتم إنشاؤه بواسطة Frappe Framework. يعتمد وضع الحقل في تنسيقات الطباعة القياسية على موضع الحقول المعنية في المستند.

![تنسيق الطباعة القياسي](https://docs.erpnext.com/files/customize-standard-print-format.png)

أي تغييرات يتم إجراؤها على تنسيق الطباعة القياسي يجب أن تتم باستخدام نموذج التخصيص. يمكنك أيضًا التحقق من [إضافة الحقول في Print Formats](https://docs.erpnext.com/docs/v13/user/manual/en/customize-erpnext/articles/making-fields-visible-in-print-format) .

## تنسيق الطباعة المخصص

يمكنك أيضًا إنشاء تنسيقات الطباعة المخصصة الخاصة بك باستخدام أداة تسمى [Print Format Builder](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-format- باني). ستساعدك هذه الأداة في إنشاء تنسيق طباعة مخصص بسيط عن طريق سحب وإفلات الحقول بتنسيق حسب تفضيلاتك.

![تخصيص تنسيق الطباعة](https://docs.erpnext.com/files/customize-print-format.gif)

لإنشاء تنسيقات طباعة مخصصة ، يأتي ERPNext مع العديد من القوالب المحددة مسبقًا بثلاثة أنماط ، وهي Modern و Monochrome و Classic.

لإنشاء إصداراتك ، افتح نموذجًا موجودًا من:

> إنشاء> طرق عرض> تنسيق الطباعة

## إعدادات الطباعة

لتعديل / تحديث إعدادات الطباعة و PDF ، انتقل إلى:

> الإعدادات> إعدادات الطباعة

![إعدادات الطباعة](https://docs.erpnext.com/files/print-settings.png)

## تنسيق طباعة HTML

لإنشاء تنسيق طباعة HTML ، قد تحتاج إلى بعض المعرفة بـ HTML و CSS و Python. فيما يلي مثال على كيفية تصميم تنسيق الطباعة الذي يحتوي على تنسيق محدد للغاية.

![تنسيق طباعة HTML](https://docs.erpnext.com/files/customize-custom-print-format-1.png)

يتم توفير تنسيقات الطباعة على جانب الخادم باستخدام [Jinja Templating Language](https://jinja.palletsprojects.com/en/3.0.x/templates/). جميع النماذج لها حق الوصول إلى كائن المستند الذي يحتوي على معلومات حول المستند الذي يتم تنسيقه. يمكنك أيضًا الوصول إلى المرافق العامة عبر وحدة فرابي. للاستفادة من الدعم عند إنشاء تنسيق طباعة مستند إلى HTML ، يمكنك الرجوع إلى [منتدى مجتمع ERPNext](https://discuss.erpnext.com/) ، أو بدء منشور جديد لاستعلامك.

للتصميم ، يتم توفير [Bootstrap CSS Framework](http://getbootstrap.com/) ويمكنك الاستمتاع بمجموعة كاملة من الفئات.

#### مراجع

1. [لغة قالب Jinja: المرجع](https://jinja.palletsprojects.com/en/3.0.x/templates/)
2. [Bootstrap CSS Framework](http://getbootstrap.com/)

#### مثال

""
    {٪ raw٪} <h3> {{doc.select_print_heading or "Invoice"}} </h3>
    <div class = "row">
        <div class = "col-md-3 text-right"> اسم العميل </ div>
        <div class = "col-md-9"> {{doc.customer_name}} </div>
    </div>
    <div class = "row">
        <div class = "col-md-3 text-right"> التاريخ </ div>
        <div class = "col-md-9"> {{doc.get_formatted ("invoice_date")}} </div>
    </div>

            {٪ - للصف في doc.items -٪}

            {٪ - endfor -٪}
        <table class = "table table-bordered">
        <tbody>
            <tr>
                <th> الأب </th>
                <th> اسم العنصر </th>
                <th> الوصف </th>
                <th class = "text-right"> الكمية </th>
                <th class = "text-right"> معدل </th>
                <th class = "text-right"> المبلغ </ th>
            </tr> <tr>
                <td style = "width: 3٪؛"> {{row.idx}} </td>
                <td style = "width: 20٪؛">
                    {{row.item_name}}
                    {٪ if row.item_code! = row.item_name -٪}
                    <br> كود الصنف: {{row.item_code}}
                    {٪- إنهاء إذا ٪}
                </td>
                <td style = "width: 37٪؛">
                    <div style = "border: 0px؛"> {{row.description}} </div> </td>
                <td style = "width: 10٪؛ text-align: right؛"> {{row.qty}} {{row.uom or row.stock_uom}} </td>
                <td style = "width: 15٪؛ text-align: right؛"> {{
                    row.get_formatted ("rate"، doc)}} </td>
                <td style = "width: 15٪؛ text-align: right؛"> {{
                    row.get_formatted ("amount"، doc)}} </td>
            </tr> </tbody>
    </table> {٪ endraw٪}
""

## ملحوظات

1. للحصول على القيم المنسقة للتاريخ والعملة ، استخدم ، `doc.get_formatted (" اسم الحقل ")`
2. بالنسبة إلى السلاسل القابلة للترجمة ، استخدم `{{'{{_ (" تمت ترجمة هذه السلسلة ")}}'}}`