## طلب عرض أسعار

**طلب عرض الأسعار هو مستند ترسله منظمة إلى مورد واحد أو أكثر يطلب عرض أسعار للعناصر.**

![Buying Flow](https://docs.erpnext.com/files/buying_flow_rfq.png)

للوصول إلى طلب عرض الأسعار ، انتقل إلى:

> الصفحة الرئيسية> الشراء> الشراء> طلب عرض أسعار

## 1. المتطلبات الأساسية

قبل إنشاء طلب تسعير واستخدامه ، يُنصح بإنشاء ما يلي أولاً:

* [المورد](https://docs.erpnext.com/docs/v13/user/manual/en/buying/supplier)
* [عنصر](https://docs.erpnext.com/docs/v13/user/manual/en/stock/item)

## 2. كيفية إنشاء طلب تسعير

1. انتقل إلى قائمة "طلب عرض الأسعار" ، وانقر فوق "جديد".
2. أدخل التاريخ.
3. اختر المورد الذي سيتم إرسال طلب عرض الأسعار إليه.
4. في الجدول التالي ، أدخل العناصر والكمية والمستودع المستهدف حيث سترسل العناصر.
5. يمكن ترك المستودع فارغًا إذا لم يتم تحديد "صيانة المخزون" للعنصر.
6. حفظ وتقديم.

![إنشاء RFQ](https://docs.erpnext.com/files/rfq-create.png)

يمكن أيضًا إنشاء طلب عرض أسعار (RFQ) من طلب مادة مقدم. بمجرد إنشاء RFQ ، يمكنك طباعة وإرسال ملف PDF إلى الموردين والذي سيحتوي على جميع التفاصيل التي أدخلتها ذات الصلة بـ RFQ. يمكنك أيضًا الحصول على ردهم (عرض أسعار المورد) في ERPNext نفسها ، راجع القسم [4.1 عرض أسعار المورد من قبل المستخدم](# 41-عرض أسعار المورد من قبل المستخدم). ومع ذلك ، بالنسبة لعدد كبير من العناصر ، قد يكون المورد الخاص بك أكثر راحة مع ورقة Excel ، وما إلى ذلك.

## 3. سمات

### 3.1 احصل على عناصر من

يمكن جلب العناصر الموجودة في جدول العناصر من مستندات أخرى. الخيارات هي: طلب المواد والفرصة والمورد المحتمل.

***طلب المواد**: سيتم جلب العناصر من طلب المواد المقدم الذي تحدده. يمكن البحث في طلب المواد ببعض الكلمات المتطابقة ويمكن أيضًا تحديد نطاق تاريخ لتصفية طلبات المواد.
    
***الفرصة**: سيتم جلب العناصر من فرصة محفوظة. يمكن تحديد نطاق التاريخ هنا أيضًا.
    
***مورد محتمل**: حدد موردًا محتملاً. ثم إذا كان لديك أي طلبات مواد مقدمة ضد هذا المورد ، فيمكن جلب العناصر من ذلك.
    

![RFQ الحصول على العناصر](https://docs.erpnext.com/files/rfq-get-items.png)

### 3.2 احصل على الموردين

بدلاً من إدخال الموردين يدويًا في الجدول ، يمكنك أيضًا جلبهم باستخدام زر "الحصول على الموردين". عند النقر فوق**أدوات> الحصول على الموردين**، سترى الحقل "الحصول على الموردين بواسطة". يوجد خياران لجلب الموردين: حسب العلامة أو حسب المجموعة.

***بالعلامة**: انتقل إلى "فئة العلامة" من خلال البحث من شريط البحث. يجب أن تكون قد أنشأت علامات هنا أولاً وقمت بتعيينها لمورد في وحدة الشراء. ثم يمكنك تحديد "حسب العلامة". عند النقر فوق إضافة "جميع الموردين" ، سيتم جلب الموردين الذين لديهم علامات مطابقة.
    
***حسب المجموعة**: حدد "مجموعة الموردين" واختر مجموعة الموردين التي تريد إضافة الموردين منها. على سبيل المثال ، إذا حددت الأجهزة ، فسيتم إضافة جميع موردي الأجهزة لديك بحيث يمكنك الحصول على عرض أسعار منهم جميعًا.
    

![RFQ الحصول على موردين](https://docs.erpnext.com/files/rfq-get-suppliers.png)

في جدول المورد ، عند توسيع صف باستخدام المثلث المقلوب ، سترى خيار "تنزيل ملف PDF" والذي سيفتح ملف PDF من طلب عرض الأسعار.

### 3.3 رابط طلبات المواد:

عندما تنقر على**أدوات> رابط لطلبات المواد**، فإنها تربط طلب عرض الأسعار بطلبات المواد المتاحة. يجب أن تكون العناصر هي نفسها في طلب عرض الأسعار وطلب المواد.

![رابط طلب المواد](https://docs.erpnext.com/files/link-to-material-request.png)

الآن ، عندما يتم حفظ طلب عرض الأسعار ، يمكنك أن ترى في لوحة المعلومات أنه مرتبط بطلب المواد. إذا كانت هناك طلبات مواد متعددة بنفس العناصر ، فسيتم إنشاء الرابط بأحدث طلب مادة.

### 3.4 معاينة البريد الإلكتروني

في قسم "تفاصيل البريد الإلكتروني" ، من مسودة طلب عرض الأسعار ، هناك شرط لإنشاء ومعاينة بريدك الإلكتروني لإرساله إلى المورد. ![قسم تفاصيل البريد الإلكتروني](https://docs.erpnext.com/files/email-details-section.png)

أدخل أي رسائل إضافية للمورد في حقل "رسالة للمورد". يمكن ملء هذا الحقل تلقائيًا باستخدام حقل "نموذج البريد الإلكتروني".

يمكن إضافة تحية ويمكن تغيير حقل "الموضوع" أيضًا. بمجرد الانتهاء من ذلك ، يمكنك النقر فوق الزر "معاينة البريد الإلكتروني" ومشاهدة معاينة للبريد الإلكتروني الذي سيتم إرساله. ![معاينة البريد الإلكتروني](https://docs.erpnext.com/files/email-preview.png)

### 3.5 الشروط والأحكام

في معاملات البيع / الشراء ، قد تكون هناك شروط وأحكام معينة بناءً عليها يقدم المورد السلع أو الخدمات للعميل. يمكنك تطبيق الشروط والأحكام على المعاملات وستظهر عند طباعة المستند. للتعرف على الشروط والأحكام ، [انقر هنا](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/terms-and-conditions)

### 3.6 إعدادات الطباعة

#### ورقة ذات رأسية

يمكنك طباعة طلبك للحصول على عرض أسعار / أمر شراء على ترويسة الشركة الخاصة بك. تعرف على المزيد [هنا](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/letter-head).

ستجمع "تجميع العناصر نفسها" نفس العناصر المضافة عدة مرات في جدول العناصر. يمكن ملاحظة ذلك عند طباعته.

#### طباعة العناوين

يمكن تغيير عناوين المستندات الخاصة بك. تعرف على المزيد [هنا](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-headings).

## 4. إنشاء عرض أسعار للمورد بعد RFQ

بعد إنشاء طلب عرض الأسعار ، هناك طريقتان لإنشاء عرض أسعار للمورد من طلب عرض الأسعار.

### 4.1 تسعير المورد من قبل المستخدم

1. افتح طلب عرض أسعار وانقر على**عرض أسعار للمورد> إنشاء**.
    
    ![عرض أسعار المورد من RFQ](https://docs.erpnext.com/files/make-supplier-quotation-from-rfq.png)
    
2. حدد المورد ، انقر فوق المورد مرة أخرى. في هذه الصفحة ، انقر فوق + بجوار "عرض أسعار المورد". سيتم فتح صفحة جديدة لعرض أسعار الموردين ، يتعين على المستخدم إدخال الكمية والسعر وإرسالها.
    
    ![عرض أسعار المورد من المورد](https://docs.erpnext.com/files/supplier-quotation-from-sup.png)
    

### 4.2 عرض أسعار المورد من المورد

1. إذا تم إنشاء [جهة اتصال](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/contact) للمورد وكان عنوان البريد الإلكتروني مرتبطًا بجهة الاتصال ، تفاصيل جهة الاتصال وسيتم جلب عنوان البريد الإلكتروني عند اختيار المورد. قم بإنشاء جهة اتصال وعنوان بريد إلكتروني إذا لم يكن موجودًا بالفعل.
    
2. انقر فوق**أدوات> إرسال رسائل بريد إلكتروني إلى الموردين**.
    
  **في حالة عدم وجود حساب المورد**: سيقوم النظام بإنشاء حساب المورد وإرسال التفاصيل إلى المورد. سيحتاج المورد إلى النقر فوق الرابط (تحديث كلمة المرور) الموجود في البريد الإلكتروني. بعد تحديث كلمة المرور ، يمكن للمورد الوصول إلى بوابتهم باستخدام نموذج "طلب عرض الأسعار". سيتم إنشاء المورد كمستخدم موقع الويب.
    
    ![البريد الإلكتروني للمورد إذا لم يكن الحساب موجودًا](https://docs.erpnext.com/files/supplier-email-with-update-password.png)
    
  **في حالة وجود حساب المورد**: سيرسل النظام رابط طلب عرض الأسعار إلى المورد. يجب على المورد تسجيل الدخول باستخدام بيانات اعتماده لعرض نموذج طلب عرض الأسعار على البوابة الإلكترونية.
    
    ![البريد الإلكتروني للمورد إذا كان الحساب موجودًا](https://docs.erpnext.com/files/supplier-email-normal.png)
    
3. في كلتا الحالتين ، عندما يقوم المورد بتسجيل الدخول ، ستظهر الشاشة التالية لهم. من هنا يمكنهم إرسال عرض أسعار إليك:
    
    ![شاشة عرض أسعار المورد](https://docs.erpnext.com/files/rfq-supplier-quotation.png)
    
    يتعين على المورد إدخال المبلغ والملاحظات (شروط الدفع) في النموذج والنقر فوق إرسال. في قسم عروض الأسعار ، ستكون الاقتباسات السابقة مرئية.
    
4. عند التقديم ، ستنشئ ERPNext عرض أسعار للمورد (وضع المسودة) مقابل المورد. يجب على المستخدم مراجعة عرض أسعار المورد وإرساله. عندما يتم اقتباس جميع العناصر من طلب عرض الأسعار من قبل المورد ، يتم تحديث حالة عرض الأسعار إلى "تم الاستلام" في جدول "الموردين" في طلب عرض الأسعار.
    
    ![حالة RFQ بعد عرض أسعار المورد](https://docs.erpnext.com/files/rfq-supplier-quoted.png)
    

اقرأ [عرض أسعار المورد](https://docs.erpnext.com/docs/v13/user/manual/en/buying/supplier-quotation) لمعرفة المزيد.

## 5. فيديو

1. [أمر الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/buying/purchase-order)
2. [المورد](https://docs.erpnext.com/docs/v13/user/manual/en/buying/supplier)
3. [عرض أسعار المورد](https://docs.erpnext.com/docs/v13/user/manual/en/buying/supplier-quotation)
4. [اقتباس](https://docs.erpnext.com/docs/v13/user/manual/en/selling/quotation)
5. [طلب المواد](https://docs.erpnext.com/docs/v13/user/manual/en/stock/material-request)