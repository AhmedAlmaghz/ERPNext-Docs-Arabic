## هيكلية الرواتب

**هيكل الرواتب هو تفاصيل الراتب المقدم للموظف ، من حيث تفكك المكونات المختلفة التي تشكل التعويض.**

أي تغييرات في هيكل الرواتب ، أي بين المكونات ، يمكن أن يكون لها تأثير كبير على ما يفعله الموظف ، مثل نوع الإعفاءات الضريبية المطالب بها.

يتيح لك Frappe HR تحديد الأرباح والخصومات لهيكل الرواتب وتكرار الرواتب ووضع الدفع من بين ميزات أخرى.

للوصول إلى هيكل الرواتب ، انتقل إلى:

> الرئيسية> الموارد البشرية> كشوف المرتبات> هيكل الرواتب

## 1. المتطلبات الأساسية

قبل إنشاء هيكل الرواتب ، من المستحسن أن يكون لديك ما يلي:

* [مكون الراتب](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/salary-component)
    

## 2. كيفية إنشاء هيكل الرواتب

1. اذهب إلى قائمة هيكل الرواتب ، وانقر على جديد.
    
2. أدخل اسم هيكل الرواتب.
    
3. حدد اسم الشركة وتكرار الرواتب.
    
4. حفظ وإرسال.
    

## 2. سمات

### 2.1 الأرباح والخصومات

تحدد الأرباح مكونات الراتب التي يحصل عليها الموظف. تتضمن هذه المكونات عادةً الأساسيات والبدلات والمكافآت والحوافز التي تتم إضافتها إلى إجمالي الراتب للموظف. من ناحية أخرى ، تحدد الاستقطاعات مكونات الراتب التي يتم خصمها من إجمالي الراتب للموظف. وتشمل هذه عادة الضرائب.

>**ملاحظة:**سيتم عرض مكونات الراتب المعينة على أنها "أرباح" فقط في جدول الأرباح والمكونات التي تم تعيينها على أنها "خصومات" ستظهر في جدول الخصومات.

لإنشاء الأرباح والخصومات ، حدد مكون الراتب في عمود المكون. أدخل الصيغة / الشرط إذا لم يتم تحديده مسبقًا أثناء إنشاء [مكون الراتب](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/salary-component). بالإضافة إلى ذلك ، يمكنك أيضًا إدخال مبلغ محدد مسبقًا في عمود المبلغ.

![هيكل الرواتب](https://docs.erpnext.com/files/salary-structure.png)

>**ملاحظة:**تأكد من النقر فوق السهم المتجه لأسفل وتمكين مربع الاختيار "المبلغ بناءً على الصيغة" في حالة حساب مكون الراتب باستخدام صيغة.

### 2.2 الحساب

في هذا القسم ، [طريقة الدفع](https://docs.erpnext.com/docs/v14/user/manual/en/accounts/articles/mode_of_payment) و [حساب الدفع](https: // docs. يمكن تحديد erpnext.com/docs/v14/user/manual/en/accounts/chart-of-accounts) المستخدم لدفع الراتب.

### 2.3 هيكل الرواتب للراتب على أساس جداول الدوام

في Frappe HR ، يمكنك أيضًا تحديد هيكل الرواتب لقسيمة الرواتب استنادًا إلى سجل الدوام ، والذي يسمح للشركة بدفع أجور الموظف هناك حسب ساعات العمل.

خطوات إنشاء هيكل الرواتب بناءً على الدوام:

1. اذهب إلى قائمة هيكل الرواتب ، وانقر على جديد.
    
2. حدد مربع الاختيار**قسيمة الراتب على أساس الجدول الزمني**.
    
3. حدد مكون الراتب.
    
4. أدخل سعر الساعة. بناءً على السعر الذي تم إدخاله ، سيتم حساب مبلغ ساعات العمل لمكون الراتب المحدد وفقًا لذلك.
    
5. حفظ وإرسال.
    
    ![أنشئ قسيمة راتب بناءً على الجداول الزمنية](https://docs.erpnext.com/files/salary-structure-for-salary-based-on-timesheets.png)
    

### 2.4 مبلغ الإجازة المصروف في اليوم

في حالة وجود إجازات قابلة للتحصيل للموظف ، يمكنك تحديد مبلغ صرف الإجازة يوميًا في هذا الحقل لهيكل الرواتب المحدد هذا. استنادًا إلى "مكون الربح" المحدد في [نوع الإجازة](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/leave-type) والمبلغ اليومي ، سيتم احتساب قيمة مكون الراتب وفقًا لذلك في قسيمة الراتب.

### 2.5 الحد الأقصى للفوائد (المبلغ)

في هذا الحقل ، يمكن تحديد الحد الأقصى لمبلغ المزايا لهيكل الرواتب. إذا تم ملء هذا الحقل ، فتأكد من أن هيكل الرواتب يحتوي على [مكون الراتب](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/salary-component) مع "هل فحص المنافع المرنة "، وسيتم دفع هذا المبلغ مقابله.

بمجرد حفظ جميع المعلومات وإرسالها ، يمكنك تعيين هيكل المرتبات للموظف إما من خلال زر**تعيين هيكل الراتب**أو عن طريق إنشاء [تعيين هيكل الراتب] جديد (https://docs.erpnext.com/ docs / v14 / user / manual / en / human-resources / راتب-هيكل-تعيين) من خلال لوحة القيادة.

يمكنك أيضًا تعيين هيكل الرواتب الذي تم إنشاؤه للعديد من الموظفين بناءً على [درجة الموظف](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/employee-grade) ، [القسم ](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/department) ، [التعيين](https://docs.erpnext.com/docs/v14/user/manual / en / human-resources / designation) ، وما إلى ذلك من خلال زر "تعيين للموظفين". بالإضافة إلى ذلك ، يمكن أيضًا إنشاء قسيمة الراتب مباشرة من خلال لوحة القيادة.

## 3. مواضيع ذات صلة

1. [مكون الراتب](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/salary-component)
    
2. [تعيين هيكل الراتب](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/salary-structure-assignment)
    
3. [إدخال كشوف المرتبات](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/payroll-entry)