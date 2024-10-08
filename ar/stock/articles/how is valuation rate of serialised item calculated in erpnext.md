\nفي ERPNext ، يتم تحديث مخزون العنصر**معدل التقييم**عند إنشاء المعاملة التالية:

1. إيصال الشراء
2. إدخال المخزون من نوع استلام المواد
3. إجراء تسوية المخزون لتحديث رصيد فتح المخزون

يدعم ERPNext نوعين من التقييم: FIFO والمتوسط ​​المتحرك.

يمكنك تحديد طريقة التقييم بناءً على قيمة العنصر التي سيتم حسابها. يمكن ضبطه حسب العنصر الفردي وكذلك عالميًا لجميع العناصر من إعدادات المخزون.

![](https://docs.erpnext.com/files/Ecw7uZV.png)

يتم احتساب معدلات تقييم الأصناف وفقًا لطريقة التقييم المحددة لها. ومع ذلك ، في حالة**العنصر المتسلسل**، يتم _ Signored_ هذه الإعدادات. العنصر أدناه ، "Macbook Pro" عبارة عن سلعة متسلسلة ولا يتم جلب معدل تقييمها من مدير السلعة. بدلاً من ذلك ، يتم تحديث معدل التقييم من _سعر إدخال المخزون الوارد الأول_ ، RS 199.80. وبالتالي ، يتم تحديثه وفقًا للمعاملات الأخرى التي يتم إجراؤها على هذا العنصر.

سيد البند:

![](https://docs.erpnext.com/files/SD7TwWD.png)

![](https://docs.erpnext.com/files/yhdnL5S.png)

الأستاذ الأسهم:

![](https://docs.erpnext.com/files/cXFcuOu.png)

لمعرفة المزيد حول وحدة ERPNext Stocks ، انقر [هنا](https://erpnext.com/docs/user/manual/en/stock)