## إعدادات حجز المواعيد

يمكنك العثور على جميع الإعدادات المتعلقة بحجز المواعيد في إعدادات حجز المواعيد.

![إعدادات حجز المواعيد](https://docs.erpnext.com/files/appointment-booking-settings.png)

## 1. تفعيل جدولة الموعد

ستعمل خانة الاختيار هذه على تمكين جدولة المواعيد وأيضًا تمكين المسار `/ book_appointment` لمستخدمي موقع الويب (عملائك). سيرى عملاؤك طريقة عرض البوابة. لمعرفة المزيد ، قم بزيارة [صفحة الموعد](https://docs.erpnext.com/docs/v13/user/manual/en/CRM/appointment)

## 2. تفاصيل الوكيل

في هذا القسم ، يمكنك إضافة تفاصيل حول الوكلاء ، مثل ساعات عملهم وأجازاتهم.

### 2.1 توفر الفتحات

هنا يمكنك ضبط التوقيت الذي يكون فيه وكلائك متاحين لحضور موعد. يتم تعيين هذا لكل يوم من أيام الأسبوع. يمثل كل صف كتلة مستمرة من الوقت ، يمكن أن يكون لديك إدخالات متعددة لكل يوم من أيام الأسبوع.

على سبيل المثال ، إذا كان وكلاؤك يعملون من الاثنين إلى الجمعة ، من 9 صباحًا إلى 5 مساءً ولكن مع استراحة غداء في الساعة 1.30 لمدة نصف ساعة. سوف تحتاج إلى إنشاء إدخالين لكل يوم. واحد من 9 صباحًا إلى 1.30 مساءً والآخر من 2 مساءً إلى 5 مساءً.

### 2.2 الوكلاء

هذه قائمة الوكلاء التي سيتم**تعيينها تلقائيًا**في المواعيد. يعتمد عدد المواعيد التي يمكن أن توجد في فترة زمنية واحدة أيضًا على عدد الموظفين في هذه القائمة.

### 2.3 قائمة الأعياد

يمكنك ربط (قائمة العطلات) \ [https: //erpnext.com/docs/v13/user/manual/en/human-resources/holiday-list \] هنا للتقدم إلى جدول المواعيد. إذا كان اليوم عطلة ، فلن يُسمح بتحديد موعد في ذلك اليوم.

## 3. تفاصيل الموعد

يحتوي هذا القسم على تفاصيل حول الموعد نفسه.

### 3.1 مدة الموعد بالدقائق

مدة التعيين بالدقائق. يستخدم هذا لحساب المواعيد الزمنية لبوابة الويب. تغيير هذا لا يؤثر على المواعيد التي تم إنشاؤها قبل التغيير.

### 3.2 الإخطار عبر البريد الإلكتروني

سيؤدي تمكين مربع الاختيار هذا إلى إرسال بريد إلكتروني إلى المشاركين في المواعيد ، أي موظفك والعميل في يوم الموعد. لا يؤثر تغيير خانة الاختيار هذه على المواعيد التي تم إنشاؤها قبل التغيير.

### 3.3 عدد الأيام يمكن أن يكون الموعد محجوزًا مسبقًا

هذا هو عدد الأيام التي يمكن فيها حجز الموعد مسبقًا. إذا انتهت قائمة العطلات المقدمة أعلاه قبل التاريخ المحسوب باستخدام هذا الرقم ، فسيتم إيقاف جدولة الموعد في نهاية قائمة العطلات.

## 4. إعدادات النجاح

### 4.1 عنوان URL لإعادة توجيه النجاح

هذا هو عنوان URL حيث سيتم إعادة توجيه المستخدم عند إنشاء إنشاء موعد ناجح عبر بوابة الويب. لن تحدث إعادة التوجيه هذه عند إنشاء المواعيد من داخل Desk UI. اتركه فارغا للمنزل. هذا متعلق بعنوان URL للموقع ، على سبيل المثال "حول" سيعيد التوجيه إلى "https://yoursitename.com/about"