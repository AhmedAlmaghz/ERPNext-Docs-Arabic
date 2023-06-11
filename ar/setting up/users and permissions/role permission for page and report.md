** يمكن التحكم في الوصول إلى صفحات وتقارير مختلفة في إذن الدور للصفحة والتقرير. **

أنواع المستندات هي أمر المبيعات ، والعميل ، والمورد ، وما إلى ذلك ، وهي ** نوع مستند ** مما يعني أنها يمكن أن تحتوي على مستندات متعددة من هذا النوع. الصفحة هي صفحة واحدة مثل [إعدادات البيع] (https://docs.erpnext.com/docs/v13/user/manual/en/selling/selling-settings). لا يمكنك إنشاء عدة إعدادات بيع ، ولكن يمكنك إنشاء أوامر مبيعات متعددة.

في ERPNext ، يمكن للمستخدم إنشاء واجهة مستخدم مخصصة باستخدام صفحة وتقرير مخصص باستخدام [Report Builder] (https://docs.erpnext.com/docs/v13/user/videos/learn/report-builder.html) أو [ تقرير الاستعلام] (https://frappe.io/docs/v13/user/en/guides/reports-and-printing/how-to-make-query-report). يحتوي ERPNext على [نظام أذونات قائم على الدور] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/users-and-permissions/role-based-permissions) حيث يمكنك تعيين الأدوار للمستخدم. يمكن تعيين نفس الدور للصفحة والتقرير للوصول إليها.

إذا قام المستخدم بتمكين وضع المطور ، فيمكنه إضافة الأدوار مباشرة في الصفحة وسجل التقرير. في هذه الحالة ، ستنعكس الأذونات أيضًا في ملف JSON للصفحة / التقرير. ضع في اعتبارك أنك تريد تقييد الأدوار التي يمكنها الوصول إلى صفحات وتقارير معينة في ERPNext ، يمكن القيام بذلك عبر إذن الدور للصفحة والتقرير.

للوصول إلى إذن الدور للصفحة والتقرير ، انتقل إلى:

> الصفحة الرئيسية> المستخدمون والأذونات> إذن الدور للصفحة والتقرير

## 1 \. كيفية استخدام إذن الدور للصفحة وأداة التقرير

إذا تم تعطيل وضع المطور ، يمكن للمستخدم تعيين الأدوار للصفحة والتقرير ، باستخدام صفحة "إذن الدور للصفحة والتقرير".

! [أدوات لتعيين أدوار مخصصة للصفحة] (https://docs.erpnext.com/files/role-permission-for-page-and-report.png)

### 1.1 إعادة التعيين إلى الإعدادات الافتراضية

باستخدام زر "إعادة التعيين إلى الإعدادات الافتراضية" ، يمكن للمستخدم إزالة الأذونات المخصصة المطبقة على صفحة أو تقرير. ثم ستكون الأذونات الافتراضية قابلة للتطبيق على تلك الصفحة أو التقرير.

! [إعادة تعيين الأدوار الافتراضية] (https://docs.erpnext.com/files/reset-roles-permission-for-page-report.png)

### أذونات الدور للصفحة

1. انتقل إلى: الصفحة الرئيسية> المطور> الصفحة.
2. أضف صفًا وحدد الأدوار الأخرى التي يمكنها الوصول إلى الصفحة.
    
    ! [تعيين الأدوار إلى الصفحة] (https://docs.erpnext.com/files/roles-for-page.png)
    

### أذونات الدور للتقرير

1. انتقل إلى: الصفحة الرئيسية> المطور> تقرير.
2. أضف صفوفًا بأدوار يمكنها الوصول إلى التقرير.
    
    ! [تعيين الأدوار للتقرير] (https://docs.erpnext.com/files/roles-for-report.png)
    

1. [ملف تعريف الدور والدور] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/users-and-permissions/role-and-role-profile)
2. [الأذونات المستندة إلى الدور] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/users-and-permissions/role-based-permissions)
3. [أذونات المستخدم] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/users-and-permissions/user-permissions)