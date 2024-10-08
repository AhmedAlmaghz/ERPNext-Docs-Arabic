---
description: copy pasting multiple records from excel
---

# نسخ ولصق عدة حقول من إكسل

**إذا كان لديك تسلسل من السجلات المحفوظة في ورقة Excel ، والتي تحتاج إلى تعيينها في جدول فرعي في ERPNext ، فيمكن القيام بالشيء نفسه باستخدام هذه الميزة.**

لنفترض أن لديك قائمة بالعناصر المحفوظة في ورقة Excel ، وتحتاج إلى نسخها إلى الجدول الفرعي "العناصر" في طلب المبيعات.

**خطوات لنسخ ولصق السجلات من Excel**

*   تحضير البيانات المصدر في Excel أو محرر نصوص مع فصل كل عمود بعلامة تبويب.

    ![نسخ لصق](https://docs.erpnext.com/files/using-copy-paste-1.png)
*   اسحب لتحديد السجلات ، وانقر فوق زر قائمة النسخ أو عن طريق Ctrl + C (Cmd + C) من أجل

    الحالة 1. يجب أن يكون العمود الأول من ورقة Excel هو رأس العمود والمحتويات الموجودة فيه.

    الحالة 2. عندما لا يكون هناك رأس عمود محدد ، سيتم تعيين البيانات إلى الأعمدة المرئية.

    ![نسخ لصق](https://docs.erpnext.com/files/using-copy-paste-4.png)
*   ضع المؤشر على حقل الإدخال الهدف للجدول الفرعي ، والصقه. على عكس ميزة الاستيراد عبر تحميل الملف ، ستؤدي ميزة النسخ واللصق هذه إلى تشغيل أحداث تغيير الحقل تلقائيًا.

    ![نسخ لصق](https://docs.erpnext.com/files/using-copy-paste-3.gif)

للنظر في الأداء ، يجب فقط لصق أقل من أو يساوي 100 سجل في المرة الواحدة.
