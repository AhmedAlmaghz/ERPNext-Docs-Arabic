---
description: role based permissions
---

# الصلاحيات القائمة على الدور

### الأذونات القائمة على الدور

**يمكن التحكم في الإذن بوثائق مختلفة باستخدام الأذونات المستندة إلى الدور.**

يحتوي ERPNext على نظام أذونات قائم على الأدوار. هذا يعني أنه يمكنك تعيين الأدوار للمستخدمين ، ويمكن تعيين الأذونات على الأدوار. يسمح لك مدير أذونات الدور بتعيين الأدوار التي يمكنها الوصول إلى المستندات والأذونات (القراءة والكتابة والإرسال وما إلى ذلك).

بمجرد تعيين الأدوار للمستخدم ، يمكن أن يقتصر وصولهم على مستندات معينة. تسمح لك بنية الأذونات بتحديد قواعد أذونات مختلفة لحقول مختلفة باستخدام مفهوم يسمى**مستوى الإذن**للحقل.

### 1. كيفية استخدام مدير أذونات الدور

لبدء استخدام مدير أذونات الدور ، انتقل إلى:

> الصفحة الرئيسية> المستخدمون والأذونات> مدير أذونات الدور

![إدارة القراءة والكتابة والإنشاء والإرسال وتعديل الوصول باستخدام مدير أذونات الدور](https://docs.erpnext.com/files/setting-up-permissions-leave-application.png)

يتم تطبيق الأذونات على مجموعة من:

\*\*\*الأدوار:\*\*كما رأينا سابقًا ، يتم تعيين الأدوار للمستخدمين ويتم تطبيق قواعد الأذونات على هذه الأدوار. على سبيل المثال ، قد يُمنح مستخدم المبيعات أدوار الموظف ومستخدم المبيعات.

```
تتضمن أمثلة الأدوار مدير الحسابات والموظف ومستخدم الموارد البشرية وما إلى ذلك.
```

\*\*\*أنواع المستندات:\*\*لكل نوع من أنواع المستندات ، الرئيسية أو المعاملات ، قائمة منفصلة من الأذونات المستندة إلى الأدوار كما هو موضح في لقطة الشاشة السابقة.

```
أمثلة على أنواع المستندات هي فاتورة المبيعات ، طلب الإجازة ، إدخال المخزون ، إلخ.
```

\*\*\*مستويات الإذن:\*\*في كل مستند ، يمكنك تجميع الحقول حسب "المستويات". يتم الإشارة إلى كل مجموعة من الحقول برقم فريد (من 0 إلى 9). يمكن تطبيق مجموعة منفصلة من قواعد الأذونات على كل مجموعة حقول. بشكل افتراضي ، تكون جميع الحقول من المستوى 0.

```
يربط إذن "المستوى" الحقول بالمستوى X بقاعدة إذن بالمستوى X. لمعرفة المزيد ، انقر [هنا](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/articles / إدارة بيرم المستوى).
```

\*\*\*مراحل المستند:\*\*يتم تطبيق الأذونات على كل مرحلة من مراحل المستند مثل الإنشاء والحفظ والتقديم والإلغاء والتعديل. يمكن السماح للدور بطباعة البيانات أو إرسالها بالبريد الإلكتروني أو استيرادها أو تصديرها أو الوصول إلى التقارير أو تحديد أذونات المستخدم.

\*\*\*أذونات المستخدم:\*\*باستخدام أذونات المستخدم في ERPNext ، يمكن تقييد المستخدم للوصول إلى مستندات محددة فقط لنوع المستند هذا. على سبيل المثال: منطقة واحدة فقط من جميع الأقاليم. يتم أيضًا تطبيق أذونات المستخدم المحددة لأنواع المستندات الأخرى إذا كانت مرتبطة بنوع المستند الحالي من خلال حقول الارتباط.

```
على سبيل المثال ، العميل هو حقل ارتباط في طلب المبيعات أو عرض الأسعار. في مدير أذونات الدور ، يمكن تعيين أذونات المستخدم باستخدام الزر "تعيين أذونات المستخدم".

لتعيين أذونات المستخدم بناءً على المستندات / الحقول ، انتقل إلى:

> الصفحة الرئيسية> المستخدمون والأذونات> الأذونات> [أذونات المستخدم](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/users-and-permissions/user-permissions)
```

\***إضافة قاعدة جديدة**: في مدير أذونات الدور ، لإضافة قاعدة جديدة ، انقر فوق الزر**إضافة قاعدة جديدة**وسيطلب منك مربع منبثق تحديد دور وإذن مستوى. بمجرد تحديد هذا والنقر فوق "إضافة" ، سيؤدي ذلك إلى إضافة صف جديد إلى جدول القواعد الخاص بك.

### 2. كيف تعمل الأذونات المستندة إلى الدور

تطبيق الإجازة هو مثال جيد يشمل جميع مجالات نظام الأذونات.

*   يجب أن يتم إنشاؤه من قبل الموظف. لهذا ، يجب إعطاء دور الموظف أذونات القراءة والكتابة وإنشاء.

    ![إعطاء أذونات القراءة والكتابة وإنشاء الموظف لتقديم طلب المغادرة](https://docs.erpnext.com/files/setting-up-permissions-employee-role.png)
*   يجب أن يكون**الموظف**قادرًا فقط على الوصول إلى طلب الإجازة الخاص به. ومن ثم ، يجب إنشاء سجل أذونات المستخدم لكل مجموعة بين المستخدم والموظف.

    ![تقييد الوصول إلى تطبيقات المغادرة لمستخدم لديه دور موظف عبر مدير أذونات المستخدم](https://docs.erpnext.com/files/setting-up-permissions-employee-user-permissions.png)
*   إذا كنت تريد أن يقوم**الموظف**بتحديد مستند فقط في مستند آخر وليس لديه حق الوصول للقراءة إلى هذا المستند ككل ، فامنح إذن تحديد فقط للدور ، الموظف.

    ![تقييد الوصول إلى تطبيقات المغادرة لمستخدم لديه دور موظف عبر مدير أذونات المستخدم](https://docs.erpnext.com/files/setting-up-select-permissions-employee.png)

\***يجب أن يكون مدير الموارد البشرية**قادرًا على رؤية جميع طلبات الإجازة. أنشئ قاعدة إذن لمدير الموارد البشرية في المستوى 0 ، مع أذونات القراءة. يجب تعطيل تطبيق أذونات المستخدم.

```
![إعطاء أذونات إرسال وإلغاء لمدير الموارد البشرية لتطبيقات الإجازة. تم إلغاء تحديد "تطبيق أذونات المستخدم" لمنح الوصول الكامل.](https://docs.erpnext.com/files/setting-up-permissions-hr-manager-role.png)
```

\***يجب أن يكون**مسؤول الإجازة\*\*قادرًا على رؤية وتحديث طلبات الإجازات للموظفين تحت إشرافه. يُمنح مسؤول الإجازة حق الوصول للقراءة والكتابة في المستوى 0. يجب إدراج مستندات الموظف ذات الصلة في أذونات المستخدم الخاصة بالموافقين على الإجازات. (يتم تقليل هذا الجهد للموافقين على الإجازات المذكورة في مستندات الموظف ، عن طريق إنشاء سجلات أذونات المستخدم برمجيًا).

```
![إعطاء أذونات القراءة والكتابة وإرسالها للموافق على المغادرة لتطبيقات المغادرة. تم تحديد "تطبيق أذونات المستخدم" لتقييد الوصول استنادًا إلى الموظف.](https://docs.erpnext.com/files/setting-up-permissions- ترك-approver-role.png)
```

*   يجب أن يتم الموافقة / الرفض فقط من قبل مستخدم الموارد البشرية أو الموافقة على الإجازة. يتم تعيين حقل الحالة لتطبيق الإجازة في المستوى 1. يتم منح مستخدم الموارد البشرية والموافق على الإجازة أذونات القراءة والكتابة للمستوى 0 ، بينما يتم منح الجميع (الكل) إذن قراءة للمستوى 1.

    ![تقييد الوصول للقراءة لمجموعة من الحقول إلى أدوار معينة](https://docs.erpnext.com/files/setting-up-permissions-level-1.png)

\***مستخدم الموارد البشرية**يجب أن يكون قادرًا على تفويض طلبات الإجازة إلى مرؤوسيه. يُمنح مستخدم الموارد البشرية الحق في تعيين أذونات المستخدم. يمكن للمستخدم الذي يتمتع بدور مستخدم الموارد البشرية تحديد أذونات المستخدم في تطبيق الإجازة للمستخدمين الآخرين.

```
![اسمح لمستخدم الموارد البشرية بتفويض الوصول إلى مغادرة التطبيقات عن طريق تحديد "تعيين أذونات المستخدم". سيسمح هذا لمستخدم الموارد البشرية بالوصول إلى مدير أذونات المستخدم لـ "ترك التطبيق"](https://docs.erpnext.com/files/setting-up-permissions-hr-user-role.png)
```

في حالة تعيين الأدوار بشكل صحيح ولكن لا تزال تواجه أخطاء عند الوصول إلى المستندات ، فراجع \[هذه الصفحة]\(https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/articles / تقرير إذن خطأ).

1. [الأذونات المستندة إلى الدور](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/users-and-permissions/role-based-permissions)
2. [أذونات المستخدم](https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/users-and-permissions/user-permissions)
3. \[إذن الدور للصفحة والتقرير]\(https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/users-and-permissions/role-permission-for-page-and -تقرير)
