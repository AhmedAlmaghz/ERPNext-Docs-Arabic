## تنسيق الطباعة

** باستخدام تنسيق الطباعة ، يمكنك تعيين كيف تبدو أنواع المستندات عند الطباعة. **

كل معاملة لها تنسيق طباعة افتراضي يسمى "قياسي". يمكنك تغيير تنسيقات الطباعة من خلال:

* باستخدام نموذج تنسيق الطباعة
* استخدام البرمجة النصية Jinja / JS ضمن تنسيق الطباعة
* استخدام [Print Format Builder] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-format-builder) لإنشاء تنسيقات طباعة باستخدام واجهة المستخدم
* استخدام نموذج التخصيص لإخفاء / إظهار الحقول

للوصول إلى تنسيق الطباعة ، انتقل إلى:

> الصفحة الرئيسية> الإعدادات> تنسيق الطباعة

## 1 \. كيفية إنشاء تنسيق طباعة

1. انتقل إلى Print Format List ، وانقر فوق New.
2. أدخل اسمًا وحدد نوع المستند الذي سيتم استخدام تنسيق الطباعة له.
3. سيتم اختيار الوحدة النمطية التي يجب أن تنطبق عليها تلقائيًا.
    
    ! [قائمة تنسيق الطباعة] (https://docs.erpnext.com/files/print-format-menu.png)
    
4. حفظ.
    

ضمن إعدادات النمط ، توجد خيارات لتغيير خيارات التصميم. باستخدام هذه الخيارات ، يمكنك تغيير الخط ، ومحاذاة التسميات معًا على اليسار أو اليمين ، وإضافة عناوين للأقسام ، وما إلى ذلك.

لتصميم تنسيق الطباعة باستخدام Jinja / JS المخصص ، انقر فوق تنسيق مخصص. إذا حددت هذا الخيار ، فسيكون هناك مربع اختيار للطباعة الأولية. لمعرفة المزيد عن الطباعة الأولية ، [انقر هنا] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/raw-printing).

إذا تم تمكين وضع المطور ، فيمكنك تحديد قياسي كنعم للمساهمة بتنسيق طباعة كتنسيق طباعة قياسي (محدد مسبقًا) في النظام.

## 1.1 استخدام نموذج التخصيص لتغيير عناصر تنسيق الطباعة

يمكن إخفاء / إظهار الحقول في المعاملات والجداول الفرعية الخاصة بهم باستخدام Customize Form. على سبيل المثال ، إذا كنت تريد إخفاء "رمز العنصر" عند طباعة عرض أسعار ، فانقر فوق رمز الطباعة للدخول إلى شاشة الطباعة.

اذهب إلى القائمة> تخصيص ، حدد عنصر عرض الأسعار في حقل "إدخال نوع النموذج". ! [تخصيص تنسيق الطباعة] (https://docs.erpnext.com/files/print-format-customize1.png)

لمعرفة المزيد ، تفضل بزيارة صفحة [تخصيص تنسيق الطباعة] (https://docs.erpnext.com/docs/v13/user/manual/en/customize-erpnext/print-format).

في جدول الحقول ، وسّع صف "رمز العنصر" ، ثم مرر لأسفل وحدد مربع الاختيار "طباعة إخفاء". ! [Print Format Print Hide] (https://docs.erpnext.com/files/print-format-customize2.png)

يمكن تحديد تنسيق طباعة تم إنشاؤه حديثًا على شاشة الطباعة الخاصة بالمعاملة. من هناك يمكنك أن ترى كيف يبدو والمضي قدما في الطباعة. ! [تحديد تنسيق طباعة] (https://docs.erpnext.com/files/print-format-selection.png)

## 2 \. فيديو

1. [نمط الطباعة] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-style)
2. [عناوين الطباعة] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/print-headings)
3. [Letter Head] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/letter-head)
4. [نموذج طباعة الشيك] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/print/cheque-print-template)
5. [تعطيل فواصل الأسطر في أقسام تنسيق الطباعة] (https://docs.erpnext.com/docs/v13/user/manual/en/setting-up/articles/print-format-sections)