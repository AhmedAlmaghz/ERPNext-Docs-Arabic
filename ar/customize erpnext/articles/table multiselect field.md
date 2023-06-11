\n## جدول MultiSelect الحقل

حقل الجدول MultiSelect يشبه إلى حد بعيد حقل الارتباط. الاختلاف الرئيسي هو أن حقل الجدول MultiSelect يسمح لك بتحديد قيم متعددة.

دعونا نفكر في مثال لفهم الشيء نفسه. لنفترض أنك تريد تعيين ToDo لعدة مستخدمين ، كما هو موضح أدناه:

! [Table MultiSelect Field] (https://docs.erpnext.com/files/table-multiselect-field.png)

يمكنك إضافة حقل التحديد المتعدد للجدول باستخدام الخطوات التالية:

## الخطوة 1: إنشاء نوع DocType تابع.

قم بإنشاء DocType جديد ، وقم بتمكين مربعي الاختيار "Is Child Table" و "Editable Grid" وإضافة حقل بنوع "Link" كما هو موضح أدناه.

قم بتعيين حقل الارتباط على أنه إلزامي. تأكد من أن الحقل الموجود في الجدول الفرعي قد تم وضع علامة عليه "في عرض القائمة".

! [DocType for Table MultiSelect] (https://docs.erpnext.com/files/doctype-for-table-multi-select.png)

## الخطوة 2: إضافة حقل من النوع "Table MultiSelect".

قم بإنشاء حقل من النوع "Table MultiSelect" وأضف نوع DocType الذي تم إنشاؤه في الخطوة الأولى في "الخيارات".

! [حقل بنوع Table MultiSelect] (https://docs.erpnext.com/files/multi-select-field.png)

يمكنك إزالة أي قيمة محددة عن طريق النقر فوق علامة التقاطع بجوار القيمة المحددة أو بوضع المؤشر بجوار القيمة والضغط على Backspace.

يسمح هذا الحقل بتحديد قيمة واحدة مرة واحدة فقط.

> ملاحظة: لا يمكن إضافة حقول الجدول MultiSelect في DocTypes الفرعية.