## إعادة تقييم سعر الصرف

في ERPNext ، يمكنك عمل إدخالات محاسبية بعملات متعددة. على سبيل المثال ، إذا كان لديك حساب مصرفي بعملة أجنبية ، فيمكنك إجراء معاملات بهذه العملة وسيظهر النظام رصيدًا مصرفيًا بتلك العملة المحددة.

الغرض من سيد إعادة تقييم سعر الصرف هو ضبط الرصيد في حسابات دفتر الأستاذ العام وفقًا لأية تغييرات في أسعار صرف العملات. يكون هذا مفيدًا عندما تغلق دفاتر حساباتك وترغب في تحديث حسابات GL الخاصة بشركتك عن طريق جلب الأموال من حسابات العملات الأخرى.

**_ ملاحظة: من الإصدار 14 من ERPNext ، يمكن لإعادة تقييم سعر الصرف التعامل مع حسابات العملات الأجنبية التي تحتوي على رصيد "0" إما بعملة الأساس أو عملة الحساب. سيتم إنشاء دفتر يومية منفصل من نوع "مكاسب / خسارة التبادل" في حالة المسودة لهم. _**

للوصول إلى قائمة إعادة تقييم سعر الصرف ، انتقل إلى:

> الرئيسية> المحاسبة> العملات المتعددة> إعادة تقييم سعر الصرف

## 1. كيفية إعداد العملة في الحساب

1. للبدء في المحاسبة متعددة العملات ، تحتاج إلى تعيين عملة المحاسبة في سجل الحساب.
2. يمكنك تحديد العملة من مخطط الحسابات أثناء إنشاء حساب.
    
    ![العملة في دفتر الأستاذ](https://docs.erpnext.com/files/currency-in-ledger.png)
    
3. يمكنك أيضًا تعيين / تعديل العملة للحسابات الحالية عن طريق فتح سجل الحساب المحدد.
    
4. انقر فوق الحساب وانقر فوق تحرير.
    
    ![تعيين عملة الحساب](https://docs.erpnext.com/files/update-currency-in-ledger.png)
    

## 2. كيفية تمكين إعادة تقييم سعر الصرف

ميزة إعادة تقييم سعر الصرف مخصصة للتعامل مع الموقف عندما يكون لديك حسابات بعملات مختلفة في مخطط حسابات شركة واحدة.

1. انتقل إلى:**الإعداد> الشركة> _ اختر الشركة _**.
2. قم بتعيين حقل "حساب مكاسب / خسارة Exchange غير المحقق" في نوع مستند الشركة. هذا الحساب لموازنة الفرق بين إجمالي الائتمان والخصم الإجمالي.
    
    ![دفتر أستاذ مكاسب / خسارة غير محقق في الشركة](https://docs.erpnext.com/files/unrealized-exchange-gain-loss-ledger-in-company.png)
    
3. انتقل إلى**المحاسبة> الإعداد> إعادة تقييم سعر الصرف> جديد**.
    
4. حدد الشركة.
5. انقر فوق الزر "الحصول على إدخالات". ستجلب الحسابات التي لها عملات مختلفة عن "العملة الافتراضية" المحددة في الشركة.
6. سيؤدي هذا إلى جلب سعر الصرف الجديد تلقائيًا إذا لم يتم تعيينه في Currency Exchange DocType لتلك العملة وإلا فسيتم جلب "سعر الصرف" المحدد في [Currency Exchange](https://docs.erpnext.com/docs/v13 / user / manual / en / accounts / currency-exchange) DocType. ![إعادة تقييم سعر الصرف](https://docs.erpnext.com/files/exchange-rate-revaluation.png)
    
7. عند التقديم ، سيظهر زر**Create Journal Entry**. ![خيار إدخال دفتر اليومية بعد الإرسال](https://docs.erpnext.com/files/exchange-rate-revaluation-submit.png)
    
8. سيؤدي النقر فوق هذا الزر إلى إنشاء إدخال دفتر يومية لإعادة تقييم سعر الصرف. ![إدخال دفتر اليومية لإعادة تقييم سعر الصرف](https://docs.erpnext.com/files/exchange-rate-revaluation-journal-entry.png)
    
9. عند إرسال إدخال دفتر اليومية ، يتأثر دفتر الأستاذ العام على النحو التالي:![Exchange Rate Revaluation GL](https://docs.erpnext.com/files/exchange-rate-revaluation-gl.png)
    

1. [إدخال دفتر اليومية بين الشركات](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/inter-company-journal-entry)
2. [فواتير بين الشركات](https://docs.erpnext.com/docs/v13/user/manual/en/accounts/inter-company-invoices)