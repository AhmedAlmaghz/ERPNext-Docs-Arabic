## إدخال دفتر اليومية بين الشركات

**يتم إدخال دفتر اليومية بين الشركات بين المؤسسات التي تنتمي إلى نفس المجموعة.**

يمكنك إنشاء إدخال دفتر يومية بين الشركات إذا كنت تجري معاملات مع شركات متعددة. يمكنك تحديد الحسابات التي ترغب في استخدامها في معاملات Inter Company. قد تكون حالة الاستخدام المحتملة شركة تشتري البضائع نيابة عن شركة أخرى.

يتم إنشاء إدخالات دفتر اليومية بين الشركات باستخدام نموذج إدخال دفتر اليومية في ERPNext. للوصول إلى قائمة إدخال دفتر اليومية ، انتقل إلى:

> الصفحة الرئيسية> المحاسبة> الشركة والحسابات> إدخال دفتر اليومية

## 1. المتطلبات الأساسية

قبل إنشاء إدخال دفتر يومية بين الشركات ، تحتاج إلى ما يلي:

* ما لا يقل عن شركتين [الشركات](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/company-setup)

## 2. كيفية إنشاء إدخال دفتر يومية بين الشركات

1. انتقل إلى قائمة إدخال دفتر اليومية ، وانقر فوق جديد.
2. حدد "نوع الإدخال" كـ "إدخال دفتر يومية بين الشركات".
3. تعيين الشركة التي تشتري السلع نيابة عن شركة أخرى.
4. أضف صفوفًا لإدخالات المحاسبة الفردية. يمكن جلب الحسابات بين الشركات فقط هنا.
5. في كل صف ، يجب تحديد:
    * الحساب الداخلي الذي سيتأثر.
    * المبلغ المدين أو الدائن.
    * مركز التكلفة (إذا كان دخلًا أو مصروفًا).
6. عند تقديم إدخال دفتر اليومية ، ستجد زرًا في الزاوية اليمنى العليا ،**Make Inter Company Journal Entry**.
    
    ![إدخال دفتر اليومية بين الشركات](https://docs.erpnext.com/files/inter-company-journal-entry.png)
    
7. انقر فوق الزر. الآن ، سيُطلب منك تحديد الشركة التي ترغب في إنشاء إدخال دفتر اليومية المرتبط مقابلها.
    
    ![مدير الشركة](https://docs.erpnext.com/files/select-company-in-inter-company-journal-entry.png)
    
8. عند تحديد الشركة ، سيتم توجيهك إلى إدخال دفتر يومية آخر حيث سيتم تعيين الحقول ذات الصلة ، أي الشركة ، ونوع القسيمة ، ومرجع إدخال دفتر اليومية بين الشركات وما إلى ذلك.
    
    ![إدخال دفتر اليومية الذي تم إنشاؤه تلقائيًا بين الشركات](https://docs.erpnext.com/files/auto-generated-intercompany-journal-entry.png)
    
9. حدد الحسابات الداخلية للشركة الثانية في الجدول.
    
10. إرسال إدخال دفتر اليومية.
11. تأكد من أن إجمالي مبالغ الخصم والائتمان مماثلة لإجمالي مبالغ الائتمان والخصم الخاصة بإدخال دفتر اليومية الذي تم إنشاؤه مسبقًا على التوالي ، ولكن ستكون عمليات الخصم والائتمان معاكسة.

**ملاحظة:**يجب أن تكون الحسابات في إدخال دفتر اليومية الثاني عكس ما فعلته في إدخال دفتر اليومية الأول. على سبيل المثال ، تشتري الشركة "أ" شيئًا من الشركة "ب". هكذا ستبدو دورة الدفع بين الشركتين باستخدام إدخال دفتر اليومية بين الشركات.

1. حساب مصرفي مدين بمقدار 500 وحساب مدين دائن للشركة B بمقدار 500.
2. الآن ، في إدخال دفتر اليومية بين الشركات ، حساب الدائنين المدين للشركة "أ" بمقدار 500 وحساب الائتمان المصرفي بمقدار 500.
3. تحتاج أيضًا إلى تحديد الأطراف لحساب الدائنين والمدينين قبل متابعة إدخال دفتر اليومية.

يمكنك أيضًا العثور على الرابط المرجعي في الأسفل ، والذي ستتم إضافته في كل من إدخالات دفتر اليومية المرتبطة وستتم إزالته إذا تم إلغاء أي من إدخالات دفتر اليومية.

1. [إدخال دفتر اليومية](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/journal-entry)
2. [فواتير بين الشركات](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/inter-company-invoices)