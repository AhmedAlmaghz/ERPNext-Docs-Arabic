## ضمان القرض غير ملزم

> مقدمة في الإصدار 13

**بمجرد سداد كامل مبلغ القرض ، يتم إنشاء "إلغاء تعهد ضمان القرض" لإلغاء التعهد بالأوراق المالية.**

![اجعل تأمين القرض غير ملزم](https://docs.erpnext.com/files/loan-security-unpledge-flow.png)

للوصول إلى قائمة Loan Security Unpledge ، انتقل إلى:

> الصفحة الرئيسية> إدارة القروض> ضمان القرض> إلغاء التعهد بضمان القرض

## 1. المتطلبات الأساسية

قبل إنشاء Loan Security Unpledge ، يجب عليك إنشاء ما يلي أولاً:

* [نوع ضمان القرض](https://docs.erpnext.com/docs/v13/user/manual/en/loan-management/loan-security-type)
* [قرض الضمان](https://docs.erpnext.com/docs/v13/user/manual/en/loan-management/loan-security)
* [قرض](https://docs.erpnext.com/docs/v13/user/manual/en/loan-management/loan)

## 2. كيفية إنشاء سند ضمان القرض

1. انتقل إلى Loan Security Unpledge List ، وانقر فوق New.
2. حدد القرض الذي لم يتم التعهد للأوراق المالية مقابله.
3. حدد مقدم الطلب.
4. حدد الشركة
5. في جدول الأوراق المالية ، أدخل ضمان القرض وكميته التي سيتم إلغاء التعهد بها. أدخل أيضًا [تعهد ضمان القرض](https://docs.erpnext.com/docs/v13/user/manual/en/loan-management/loan-security-pledge) الذي يجب أن تكون الأوراق المالية غير مرتبط بها.
6. انقر فوق "حفظ" لحفظ مسودة "إلغاء تعهد ضمان القرض".
7. انقر فوق "إرسال" لفصل سندات القرض المالية

![طلب قرض](https://docs.erpnext.com/files/loan-security-unpledge.png)

### 2.1. طرق أخرى لإنشاء Unpledge ضمان القرض

يمكنك أيضًا إنشاء "إلغاء تأمين القرض" من القرض الذي يُطلب من خلاله إغلاق القرض عبر الزر**إنشاء**في أعلى اليمين

![طلب قرض](https://docs.erpnext.com/files/create-loan-security-unpledge.png)

## 3. سمات

### 3.1 الموافقة على طلب إلغاء تعهد ضمان القرض

عند الموافقة على Loan Security Unpledge ، سيتم تلقائيًا تحديث الكمية والحالة في [تعهد ضمان القرض] المقابل (https://docs.erpnext.com/docs/v13/user/manual/en/loan-management/loan- تعهد أمني). في حالة إلغاء التعهد بالكامل ، فإن الحالة في تعهد ضمان القرض الذي يتم تقديم طلب إلغاء التعهد مقابله سيتم تعيينها على أنها "غير متعهد" وإلا فسيتم تعيينها على أنها "مرهون جزئيًا". في حالة إلغاء الرهن بالكامل ، سيتم أيضًا إغلاق القرض الذي يتم تقديم طلب غير مؤكد مقابله تلقائيًا.