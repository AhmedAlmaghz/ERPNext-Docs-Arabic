\nفي البيانات الرئيسية للعنصر ، قد تشهد تجميد القيم في الحقول التالية.

1. الحفاظ على المخزون
2. لديها رقم الدفعة.
3. لديه الرقم التسلسلي.

![تم تجميد حقل العنصر](https://docs.erpnext.com/files/maintain-stock-1.png)

بالنسبة إلى عنصر ما ، بمجرد إنشاء إدخال دفتر أستاذ المخزون ، سيتم تجميد القيم الموجودة في هذه الحقول. هذا لمنع المستخدم من تغيير القيمة التي يمكن أن تؤدي إلى تطابق خاطئ للمخزون الفعلي ومستوى المخزون في نظام أحد العناصر.

بالنسبة إلى العنصر المتسلسل ، نظرًا لأنه يتم حساب مستوى المخزون الخاص به بناءً على عدد الأرقام التسلسلية المتاحة ، فإن تعيين العنصر على أنه غير متسلسل في منتصف الطريق سيؤدي إلى تعطيل المزامنة ، ولن يكون مستوى مخزون العنصر الموضح في التقرير دقيقًا ، وبالتالي فقد تم تجميد حقل الرقم التسلسلي.

لجعل هذه الحقول قابلة للتحرير مرة أخرى ، يجب عليك حذف جميع معاملات المخزون التي تم إجراؤها لهذا العنصر. بالنسبة للعنصر المسلسل والعنصر الدفعي ، يجب عليك أيضًا حذف الرقم المسلسل وسجل رقم الدُفعة لهذا العنصر.