## التعاقد من الباطن

**في التعاقد من الباطن ، توظف طرفًا خارجيًا لتنفيذ مهام لمؤسستك ، وخاصة التصنيع.**

التعاقد من الباطن هو نوع من عقود العمل الذي يسعى إلى الاستعانة بمصادر خارجية لأنواع معينة من العمل لشركات أخرى. يسمح بالعمل على أكثر من مرحلة واحدة من المشروع ليتم إنجازها في وقت واحد ، مما يؤدي في كثير من الأحيان إلى إنجاز أسرع.

يمارس التعاقد من الباطن من قبل مختلف الصناعات. على سبيل المثال ، يقوم المصنعون الذين يصنعون عدة منتجات من مكونات معقدة بالتعاقد من الباطن على مكونات معينة وتعبئتها في منشآتهم.

إذا كان عملك ينطوي على إسناد عمليات معينة إلى مورد خارجي حيث تقوم بتوريد المواد الخام ويقوم الطرف الثالث بالعمل / الإنتاج ، فيمكنك تتبع ذلك باستخدام ميزة التعاقد من الباطن الخاصة بـ ERPNext.

## 1. كيفية إعداد التعاقد من الباطن

1. إنشاء عنصر خدمة (عنصر غير مخزون). يمثل تكلفة الخدمة للعملية المتعاقد عليها من الباطن.
    
    ![service itemb2929d](https://docs.erpnext.com/files/service-itemb2929d.png)
    
2. إنشاء عناصر منفصلة للمنتج غير المعالج والمنتج المعالج. على سبيل المثال ، إذا قدمت X غير مصبوغ إلى المورد الخاص بك وأعاد المورد لك X ، فيمكنك إنشاء عنصرين: "X-unpainted" و "X".
    
3. قم بإنشاء مستودع للمورد الخاص بك حتى تتمكن من تتبع العناصر الموردة. (يمكنك توفير عناصر بقيمة شهر دفعة واحدة).
    
4. بالنسبة للبند الذي تمت معالجته ، في مدير السلعة ، قم بتمكين "توريد المواد الخام للشراء".
    
    ![fg item](https://docs.erpnext.com/files/fg-item.png)
    

### 1.1 إنشاء قائمة مكونات الصنف

قم بعمل [فاتورة المواد](https://docs.erpnext.com/docs/v13/user/manual/en/manufacturing/bill-of-materials) للعنصر المعالج ، مع العناصر غير المعالجة كعناصر فرعية. لنفكر في مثال بسيط ، حيث تصنع قلمًا. سيتم تسمية القلم المعالج تحت قائمة المواد (BOM) ، بينما سيتم تصنيف المنقار والبلاستيك والحبر وما إلى ذلك كعناصر فرعية.

سيكون BOM هذا بدون عمليات إذا تم تنفيذ جميع أعمال الإنتاج بواسطة جهة خارجية. دعنا نرى مع مثال بسيط لتجميع وحدة المعالجة المركزية:

![bom items](https://docs.erpnext.com/files/bom-items.png)

### 1.2 إنشاء طلب شراء

قم بعمل طلب شراء تعاقد من الباطن لعنصر الخدمة وحدد العنصر النهائي الجيد ، الذي قمت بإنشاء قائمة مكونات الصنف من أجله.

1. قم بتمكين "متعاقد من الباطن" لأن أمر الشراء هذا مخصص للتعاقد من الباطن.
    
    ![po is subcontracted](https://docs.erpnext.com/files/po-is-subcontracted.png)
    
2. هنا ستكون قيمة حقل السعر لجدول السلع في طلب الشراء هي تكلفة الخدمة التي اتفقت عليها مع الطرف الثالث أو المورد.
    
    ![po items](https://docs.erpnext.com/files/po-items.png)
    
3. بعد ملء التفاصيل ، احفظ وأرسل [طلب الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/buying/purchase-order#35-raw-materials-supplied) .
    

### 1.3 إنشاء أمر تعاقد من الباطن

قم بعمل أمر تعاقد من الباطن لأمر الشراء بالنقر فوق إنشاء> أمر التعاقد من الباطن. عند "حفظ" ، في "المواد الخام الموردة" ، سيتم تحديث جميع العناصر غير المعالجة بناءً على فاتورة المواد الخاصة بك. يمكنك أيضًا تحديد المستودع حيث سيتم حجز المواد الخام للتعاقد من الباطن ضمن احتياطي المستودع.

![إنشاء sco من po](https://docs.erpnext.com/files/create-sco-from-po.gif)

1. يجب تسجيل التكاليف المتضمنة في عملية التعاقد من الباطن في حقل السعر في جدول البنود في أمر التعاقد من الباطن الموضح على النحو التالي:
    
    ![sco all item table](https://docs.erpnext.com/files/sco-all-item-tables.png)
    
2. في الصورة السابقة ، نزود المقاول من الباطن بالعناصر التالية:
    
    * 8 اللوحات الأم
    * 8 معالجات
    * 16 رام
    * 8 أقراص صلبة
    * 8 خزائن
    
    تبلغ تكلفة وحدة المعالجة المركزية الواحدة بما في ذلك المواد الخام وتكاليف الخدمة 1،02،994 والتكلفة الإجمالية لجميع وحدات المعالجة المركزية هي 8،23،952
    
    ![sco items row qty rate](https://docs.erpnext.com/files/sco-items-row-qty-rate.png)
    
3. من أمر تعاقد من الباطن ، حدد المواد الخام المراد نقلها إلى المقاول من الباطن:
    
    ![أرسل إلى المقاول من الباطن](https://docs.erpnext.com/files/se-send-to-subcontractor.gif)
    
4. بمجرد تقديم طلب التعاقد من الباطن ، يمكنك عرض الكمية المحجوزة للصنف من لوحة معلومات الصنف أيضًا.
    
    ![لوحة تحكم العنصر](https://docs.erpnext.com/files/item-dashboard.png)
    

### 1.4 إنشاء إدخال مخزون لنقل المواد الخام

الآن بعد أن تم حجز المواد الخام ، قم بعمل إدخال للمخزون وقم بتسليم عناصر المواد الخام إلى المورد الخاص بك.

في أمر التعاقد من الباطن ، انقر فوق نقل> مادة إلى المورد. تعيين المصدر والمستودعات المستهدفة. سيكون إدخال المخزون من النوع "إرسال إلى المقاول من الباطن" حيث تقوم بالتحويل من مستودع إلى آخر. ضع علامة على "من BOM" ، حدد BOM ، أدخل الكمية ، وانقر على زر الحصول على العناصر.

![تم تقديمه](https://docs.erpnext.com/files/se-submitted.png)

### 1.5 إنشاء إيصال تعاقد من الباطن لاستلام العناصر المنتهية

استلم العناصر من المورد الخاص بك باستخدام إيصال التعاقد من الباطن. تحتاج إلى دخول مستودع الموردين حيث سيتم أخذ المواد الخام واستلام البضائع النهائية في المستودع المقبول. ضع في اعتبارك هذا مثل رد فعل خلفي للتعاقد من الباطن.

انقر فوق إنشاء> إيصال التعاقد من الباطن من أمر التعاقد من الباطن. قم بتعيين المستودعات المقبولة والموردين. تأكد من مراجعة "الكمية المستهلكة" في جدول "المواد الخام" حتى يتم الاحتفاظ بالمخزون الصحيح في نهاية المورد. تحتاج إلى تحديد مستودع المورد حيث ستتلقى البضائع النهائية.

![scr المستهلكات](https://docs.erpnext.com/files/scr-consumed-items.png)

### 1.6 إنشاء إيصال شراء

العودة إلى أمر الشراء ، انقر فوق إنشاء> إيصال الشراء. لن يكون هناك أي تأثير على دفتر الأستاذ ودفتر الأستاذ المحاسبي حيث يتم تحديث كل من دفتر الأستاذ والمحاسبة عند إرسال إيصال التعاقد من الباطن. في حالة وجود "ضرائب ورسوم شراء" ، فسيتم تحديث دفتر الأستاذ المحاسبي وفقًا لذلك.

### 1.7 المواد الخام من مصادر المورد

أثناء إنشاء BOM للتعاقد من الباطن ، قد يكون هناك القليل من المواد الخام مثل الصواميل والمسامير التي سيتعين على الموردين شراؤها بأنفسهم.

أثناء إنشاء إدخال مخزون لـ "التحويل" من أمر التعاقد من الباطن ، يمكن استبعاد هذه العناصر واحدًا تلو الآخر ، ولكن من المستحيل القيام بذلك إذا كان لديك أكثر من 100 عنصر.

إذا تم الحصول على بعض المواد الخام من قبل المورد مباشرة ، فيجب تضمين هذه المواد الخام في قائمة المواد.

* سيكون لها قيمة صفرية في قائمة مكونات الصنف
* في أمر التعاقد من الباطن ، لن تظهر هذه المادة الخام في العناصر الموردة نظرًا لعدم توفيرها
* أيضًا ، أثناء إنشاء "تحويل" ، سيتم استبعاد هذه العناصر من إدخال المخزون
    
    ![صف عناصر bom مصدره المورد](https://docs.erpnext.com/files/bom-items-row-sourced-by-supplier.png)
    

ومع ذلك ، قد يختار المورد تضمين العناصر التي يقدمها المورد في طلب المبيعات المرسل إليك.

## 2. ملحوظات

* تأكد من أن "سعر" السلعة المعالجة هو تكلفة المعالجة / الخدمة (باستثناء تكلفة المواد الخام).
    
* سيضيف ERPNext تلقائيًا معدل المواد الخام لغرض التقييم الخاص بك عندما تتلقى العنصر النهائي في مخزونك.
    
* سيقوم ERPNext تلقائيًا "مخزن الاحتياطي" افتراضيًا في أمر التعاقد من الباطن من BOM. إذا لم يتم العثور عليه في BOM ، فسيتم تعيينه افتراضيًا من المستودع الافتراضي المعين في العنصر. يمكنك تعيين مستودع الاحتياطي الافتراضي لجميع العناصر الموجودة في أمر التعاقد من الباطن من حقل "مخزن الاحتياطي" في قسم المواد الخام الموردة.
    

1. [أمر الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/buying/purchase-order)
2. [إيصال الشراء](https://docs.erpnext.com/docs/v13/user/manual/en/stock/purchase-receipt)