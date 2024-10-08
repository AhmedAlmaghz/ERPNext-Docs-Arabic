## ميعاد

**الموعد هو اجتماع تم الترتيب له مسبقًا بين عميل ~~~~متوقع وموظف في شركتك.**

يمكن استخدام نوع مستند الموعد لجدولة وإدارة التفاعل مع [العميل المحتمل](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/lead) أو [فرصة](https: / /docs.erpnext.com/docs/v13/user/manual/en/CRM/opportunity).

للوصول إلى قائمة المواعيد ، انتقل إلى:

> الصفحة الرئيسية> CRM> خط أنابيب المبيعات> موعد

## 1. المتطلبات الأساسية

1. [إعدادات حجز المواعيد](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/appointment-booking-settings)
2. [قائمة العطلات](https://docs.erpnext.com/docs/v13/user/manual/en/human-resources/holiday-list)
3. [الموظف](https://docs.erpnext.com/docs/v13/user/manual/en/human-resources/employee)
4. [الرصاص](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/lead)
5. [بريد إلكتروني](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/email/email-account)

## 2. كيفية إنشاء موعد

1. اذهب إلى قائمة المواعيد ، وانقر على جديد
2. حدد الوقت المجدول للموعد
3. أدخل تفاصيل العميل
4. في المستندات المرتبطة ، إذا كنت قد قمت بالفعل بإنشاء عميل متوقع للعميل ، يمكنك تعيينه هنا. وإلا فسيقوم النظام تلقائيًا بإنشاء عميل متوقع جديد بتفاصيل العميل من الخطوة السابقة.
5. حفظ. ![موعد جديد](https://docs.erpnext.com/files/new-appointment.png)

### 2.1 إنشاء المواعيد عبر الموقع الإلكتروني

يمكن لعملائك / العملاء المتوقعين إنشاء موعد باستخدام صفحة الويب `yoursitename.com / book_appointment`.

يحتاجون أولاً إلى تحديد التاريخ والوقت. ![نموذج ويب موعد](https://docs.erpnext.com/files/appointment-webform.png)

ثم أضف المزيد من التفاصيل:![تفاصيل الموعد](https://docs.erpnext.com/files/appointment-details.png)

سيتطابق مع البريد الإلكتروني للعميل مع العملاء المتوقعين في النظام وإذا تم العثور على واحد ، فسيتم ربطه بالمستند. إذا لم يتم العثور على عميل متوقع ، فسيتم تمييز الموعد على أنه "لم يتم التحقق منه" ويتم إرسال بريد إلكتروني إلى العميل لتأكيد بريده الإلكتروني

## 3. سمات

### 3.1 تعيين تلقائي

يتم تعيين المواعيد تلقائيًا للموظفين وفقًا لقائمة "الوكلاء" في [إعدادات حجز المواعيد](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/appointment-booking-settings). يتم تعيين الوكيل الذي لديه أقل عدد من التعيينات في يوم الموعد والذي يكون مجانيًا في الوقت المحدد للموعد.

### 3.2 تأكيد البريد الإلكتروني

إذا لم يكن هناك عميل متوقع مطابق في نظامك ، فسيتم إرسال بريد إلكتروني إلى عنوان البريد الإلكتروني في الموعد لتأكيد ما إذا كان عنوان البريد الإلكتروني صالحًا أم لا. عند التأكيد ، سيتم أيضًا إنشاء عميل متوقع جديد في النظام جنبًا إلى جنب مع الموعد.