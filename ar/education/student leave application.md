## طلب إجازة الطالب

**طلب إجازة الطالب هو وثيقة رسمية لتتبع الإجازات للطالب.**

للوصول إلى قائمة تطبيق إجازة الطالب ، انتقل إلى:

> الرئيسية> التعليم> الحضور> طلب إجازة الطالب

## 1 كيفية إنشاء طلب إجازة طالب

1. اذهب إلى قائمة تطبيق إجازة الطالب ، وانقر على جديد.
2. حدد الطالب.
3. قم بتعيين حقلي "من تاريخ" و "إلى تاريخ" لتحديد الفترة.
4. تحديد الحضور لطلب الإجازة يخضع لحقل "الحضور على أساس". في ERPNext ، يمكن تمييز حضور الطالب بطريقتين:
    
   ***الجدول الزمني للدورة التدريبية**: إذا تم تسجيل حضور لكل محاضرة (في الكليات / الجامعات) ، فيمكن إنشاء طلب الإجازة لشريحة جدول الدورة المحددة.
        
   ***مجموعة الطلاب**: إذا تم تسجيل الحضور ليوم كامل ، فسيتم استخدام مجموعة الطلاب (الفصل / القسم) لتمييز الحضور بحيث يتم احتساب الإجازة لليوم بأكمله
        
5. بناءً على حقل الحضور ، حدد مجموعة الطلاب أو جدول الدورة التدريبية. اختياريا أدخل السبب.
    
6. في حالة عدم حضور الطالب إلى المعهد للمشاركة أو تمثيل المعهد في أي حال ، يمكن تمييزه على أنه "موجود" من طلب الإجازة نفسه عن طريق تحديد _Mark as Present_.
7. حفظ. سيتم حساب "إجمالي أيام الإجازة" وتعيينها في المستند بعد استبعاد أيام العطل التي تعد جزءًا من [قائمة العطلات] الافتراضية الخاصة بك (https://docs.erpnext.com/docs/v13/user/manual/en/human -الموارد / قائمة العطلات).
    
    ![طلب إجازة الطالب](https://docs.erpnext.com/files/student-leave-application.png)
    

### 1.2 عند تقديم طلب إجازة الطالب

بمجرد تقديم طلب إجازة الطالب ، يتم إنشاء سجل حضور الطالب تلقائيًا بالحالة "غائب". إذا تم تحديد _Mark as Present_ ، فسيتم تعيين حالة سجل الحضور على "Present". طلب الإجازة مرتبط بوثيقة حضور الطالب هذه للرجوع إليها.

![حضور الطالب](https://docs.erpnext.com/files/leave-attendance-record.png)

إذا كان أي من التواريخ ضمن فترة الإجازة هو يوم عطلة ، فسيتم تخطي إنشاء سجل حضور الطالب لذلك التاريخ.

### 1.3 إلغاء طلب إجازة الطالب

عند إلغاء طلب إجازة الطالب ، يتم أيضًا إلغاء سجل حضور الطالب المرتبط تلقائيًا.

## 2. فيديو تعليمي لتطبيق إجازة الطالب

1. [حضور الطالب](https://docs.erpnext.com/docs/v13/user/manual/en/education/student-attendance).