## الاحتفاظ بعينة المخزون

**مخزون العينة عبارة عن دفعة من أي عناصر مخزنة للتحليل إذا دعت الحاجة لاحقًا.**

يمكن أن يكون العنصر الذي يتم تخزين مخزون العينة له مادة خام أو مادة تعبئة أو منتج نهائي.

## 1. المتطلبات الأساسية

قبل استخدام الاحتفاظ بالعينة ، يُنصح بإنشاء ما يلي أولاً:

* [عنصر](https://docs.erpnext.com/docs/v13/user/manual/en/stock/item)
* [دفعة](https://docs.erpnext.com/docs/v13/user/manual/en/stock/batch)
* [المستودع](https://docs.erpnext.com/docs/v13/user/manual/en/stock/warehouse)

## 1. كيفية تعيين مستودع الاحتفاظ بالعينة في إعدادات المخزون

يُنصح بإنشاء مستودع جديد بشكل منفصل للاحتفاظ بالعينات وعدم استخدامها في الإنتاج.

![نموذج مستودع الاحتفاظ](https://docs.erpnext.com/files/sample-warehouse.png)

### 1.2 تمكين الاحتفاظ بالعينة في مدير العنصر

يعتمد الاحتفاظ بالعينة على الدُفعة ومن ثم يجب تمكين "لديه دفعة لا" أولاً. تحقق من الاحتفاظ بالعينة وقم بتعيين الحد الأقصى للعينات المسموح بها للدُفعة.

![الاحتفاظ بالعينة](https://docs.erpnext.com/files/retain-sample.png)

### 1.3 إدخال المخزون

* عندما يتم إنشاء [إدخال مخزون](https://docs.erpnext.com/docs/v13/user/manual/en/stock/stock-entry) لغرض استلام المواد ، للعناصر التي تم تمكين الاحتفاظ بنموذج ، يمكن تعيين كمية العينة أثناء إدخال المخزون هذا. تحتاج إلى تحديد رقم الدُفعة للعنصر / العناصر. لا يمكن أن تزيد كمية العينة عن الحد الأقصى لكمية العينة المحددة في "سجل السلعة".
    
    ![الاحتفاظ بالعينة](https://docs.erpnext.com/files/material-receipt-sample.png)
    
* عند تقديم إدخال المخزون هذا ، سيكون الزر "إنشاء إدخال مخزون الاحتفاظ" متاحًا لإجراء إدخال مخزون آخر لنقل عناصر العينة من الدُفعة المذكورة إلى مستودع الاحتفاظ المحدد في إعدادات المخزون.
    
    ![زر الاحتفاظ بالعينة](https://docs.erpnext.com/files/sample-retention-button.png)
    
* سيؤدي النقر فوق هذا الزر إلى توجيهك إلى إدخال مخزون جديد من النوع "نقل المواد". يقوم هذا الإدخال بنقل الاحتفاظ بالعينات الخاصة بك من المستودع الهدف (المتاجر) إلى مستودع نماذج الاحتفاظ. سيحتوي على جميع المعلومات ، تحقق وانقر فوق إرسال.
    
    ![الاحتفاظ بالعينة](https://docs.erpnext.com/files/material-transfer-sample.png)
    

1. [المستودع](https://docs.erpnext.com/docs/v13/user/manual/en/stock/warehouse)