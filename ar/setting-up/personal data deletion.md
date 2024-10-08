---
description: personal data deletion
---

# حذف البيانات الشخصية

### حذف البيانات الشخصية

كجزء من الامتثال للائحة العامة لحماية البيانات (GDPR) ، لدى ERPNext ميزة حذف البيانات الشخصية.

تمكّن أداة حذف البيانات الشخصية المستخدم من حذف حسابه وإخفاء هوية جميع بيانات التعريف الشخصية التي أنشأها المستخدم أثناء استخدام ERPNext. وهذا يعني أن معلومات التعريف الشخصية ستكون عشوائية. يتضمن ذلك بيانات التعريف الشخصية من حساب المستخدم الخاص بك مثل: اسم المستخدم ، والاسم الكامل ، وتاريخ الميلاد ، وأرقام الهواتف ، وأرقام الهواتف المحمولة ، والموقع ، والاهتمامات ، والسيرة الذاتية ، وتوقيع البريد الإلكتروني ، والبريد الإلكتروني ، والاتصال ، والعنوان ، والاتصال ، وما إلى ذلك ، ويتضمن أيضًا بيانات من العملاء المتوقعين والفرص ، التفاصيل التي قمت بحفظها مثل أرقام الهواتف وأرقام الهواتف المحمولة والفاكس والموقع الإلكتروني والاسم.

ومع ذلك ، فإن هذا يستثني البيانات التي يتطلب القانون أن تحتفظ بها الشركة.

### 1. كيفية طلب حذف الحساب

1. لبدء حذف حساب المستخدمين وبيانات التعريف الشخصية ، يلزمك زيارة \ \[host-name ] / request-for-account-deletion (على سبيل المثال ، example.erpnext.com/request-for-account-deletion) في عنوان URL مجال.

![طلب حذف الحساب](https://docs.erpnext.com/files/Screenshot%D9%AA202021-12-01%D9%AA20at%D9%AA208.53.14%D9%AA20PM.png)

2.  أدخل البريد الإلكتروني المرتبط بحساب ERPNext الخاص بك. بعد تقديم طلبك ، ستتلقى ردًا ناجحًا.

    ![نجح طلب الحذف](https://docs.erpnext.com/files/deletion-request-success.png)
3.  سيؤدي هذا إلى إرسال بريد إلكتروني به رابط تحقق لحذف البيانات إلى عنوان البريد الإلكتروني المرتبط بالمستخدم.

    ![رسالة التحقق](https://docs.erpnext.com/files/verification-email.png)
4. بمجرد أن ينقر المستخدم على رابط التحقق. سيتم عرض رسالة تأكيد. ![تأكيد التحقق](https://docs.erpnext.com/files/confirmed-verification.png)

### 2. كيف يتم حذف البيانات الشخصية للمستخدم

يتم تسجيل طلب حذف البيانات في نوع المستند "طلب حذف البيانات الشخصية".

![Doctype طلب تنزيل البيانات الشخصية](https://docs.erpnext.com/files/personal-data-deletion-request-doctype.png)

يحتفظ هذا المستند بثلاث حالات للحالة لإكمال عملية إزالة بيانات المستخدم.

#### 2.1 في انتظار التحقق

تشير هذه الحالة إلى أن المستخدم قد طلب حذف البيانات عبر نموذج الويب. ومع ذلك ، لا يزال التحقق من هذا الطلب معلقًا. ابحث عن طلب حذف البيانات الشخصية من شريط البحث.

![في انتظار التحقق](https://docs.erpnext.com/files/pending-verification.png)

#### 2.2 الموافقة المعلقة

يشير هذا إلى أن المستخدم قد تحقق من الطلب عبر البريد الإلكتروني. يتيح ذلك خيار "حذف البيانات" لمديري النظام.

![الموافقة المعلقة](https://docs.erpnext.com/files/pending-approval.png)

#### 2.3 محذوف

يشير هذا إلى أن مدير النظام قد نقر على زر "حذف البيانات". هذا يعني أن بيانات التعريف الشخصية للمستخدم مجهولة المصدر.

![مستخدم محذوف](https://docs.erpnext.com/files/deleted-user.png)

#### 3. إعداد اتفاقية مستوى الخدمة لطلب حذف البيانات الشخصية.

يمكنك أيضًا تعيين اتفاقية مستوى الخدمة (SLA) لطلب حذف البيانات الشخصية من خلال إعدادات موقع الويب. سيظهر هذا في وصف نموذج الويب.

* اذهب إلى إعدادات الموقع
* قم بالتمرير إلى القسم المسمى إعدادات حذف الحساب
* في الحقل**حذف الحساب اتفاقية مستوى الخدمة (أيام)**، حدد عدد الأيام التي سيتم خلالها تلبية طلب المستخدمين لحذف الحساب.
* إذا قمت بتمكين**إظهار رابط حذف الحساب في صفحة حسابي**، فسيكون رابط النموذج مرئيًا للمستخدمين في صفحة حسابي على موقع الويب

![إعدادات حذف الحساب](https://docs.erpnext.com/files/Screenshot%D9%AA202021-12-01%D9%AA20at%D9%AA208.50.39%D9%AA20PM.png)

1. [تنزيل البيانات الشخصية](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/personal-data-download)
