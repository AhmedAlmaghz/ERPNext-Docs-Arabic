\nيمكن استخدام قالب Jinja للإشارة إلى أي حقل في أي نوع DocType في ERPNext. يمكن القيام بذلك ببساطة عن طريق استدعاء {{doc.field \ _name}} على تنسيق طباعة ، حيث "doc.name" هو اسم متغير لحقل معين.

ومع ذلك ، لا يعمل هذا الأسلوب للجداول التابعة داخل DocType. ستساعدك هذه المقالة في اجتياز جميع الصفوف المتعلقة بجدول فرعي وعرضها داخل أي DocType.

**المتطلبات المسبقة**

سنطلب اسم متغير للجدول الفرعي في DocType المقابل. يمكن الاطلاع على هذا من قسم "تخصيص النموذج" لنوع DocType المطلوب. نفس الشيء موضح أدناه

![](https://docs.erpnext.com/files/f7Xxz1S.png)

سنطلب أيضًا أسماء المتغيرات لجميع الحقول الموجودة داخل الجدول الفرعي والتي يجب الرجوع إليها. يمكن الحصول على هذا من قسم "تخصيص النموذج" في الجدول الفرعي المقابل كما هو موضح أدناه

![](https://docs.erpnext.com/files/tzloEh2.png)

![](https://docs.erpnext.com/files/wPB82f0.png)

![](https://docs.erpnext.com/files/AV0308f.png)

![](https://docs.erpnext.com/files/CW0oEUo.png)

**الطريقة الأولى: عرض صفوف جدول فرعي في قائمة غير مرتبة**

{٪ for row in doc.items٪} * رمز الصنف: {{row.get \\\ _ formatted ("item \\\ _ code"، doc)}} الكمية: {{row.get \\\ _ formatted ("qty "، doc)}} المعدل: {{row.get \\\ _ formatted (" rate "، doc)}} المبلغ: {{row.get \\\ _ formatted (" amount "، doc)}}
{٪ endfor٪}

سيكون الإخراج على تنسيق الطباعة على النحو التالي

![](https://docs.erpnext.com/files/lgLjE7u.png)

**الطريقة الثانية: عرض صفوف الجدول الفرعي كجدول**



{٪ للعنصر في doc.items٪} {٪ endfor٪}

| كود الصنف | الكمية | معدل | المبلغ |
| --- | --- | --- | --- |
| {{item.item \\\ _ code}} | {{item.qty}} | {{item.rate}} | {{item.amount}} |

سيكون الإخراج على تنسيق الطباعة على النحو التالي

![](https://docs.erpnext.com/files/GS00WlC.png)

يمكن استخدام هذا النموذج كمرجع. يمكن جلب أي حقول إضافية في حقل الجدول الفرعي بطريقة مماثلة ، عن طريق تعديل قالب Jinja.