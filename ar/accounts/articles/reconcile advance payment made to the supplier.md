---
description: reconcile advance payment made to the supplier
---

# تسوية الدفعة المقدمة للمورد

**أثناء الترحيل من تطبيق **_**x**_** إلى ERPNext ، كيف يتم حجز حسابات الدفع مقدمًا والتسوية مع الفواتير المستقبلية؟**

**حجز حسابات الدفع المسبق:**

قم بإنشاء**إدخال دفتر اليومية**من النوع**فتح الإدخال**، قم بخصم \_ حساب الدائن\_ باختيار \_المورد \_ المطلوب وائتمان \_ حساب الفتح المؤقت \_.

قم بتوسيع صف الدائن وحدد**نعم**لـ _Is Advance._

\_ ارجع إلى ملف GIF الذي يوضح نفس الشيء: \_

![](https://docs.erpnext.com/files/CsMRH40.gif)

سيعكس تقديم إدخال دفتر اليومية رصيدًا سلبيًا في**ملخص الحسابات الدائنة**:![](https://docs.erpnext.com/files/FJeIj5k.png)**مطابقته مع فواتير الشراء:**

راجع تقرير**الحسابات الدائنة**\_ بعد\_ إنشاء فاتورة الشراء:

![](https://docs.erpnext.com/files/cxZArKd.png)

حاليًا ، لم يتم تسويتها ويتم إظهارها على أنها**اثنان\*\*\*\*إدخالات منفصلة**، استخدم أداة**تسوية المدفوعات**لتسوية هذين الإدخالين ، \_ ارجع إلى ملف GIF للخطوات: \_

![](https://docs.erpnext.com/files/jbj6LRc.gif)

راجع تقرير الحسابات الدائنة بعد التسوية ، فلن يعكس**إدخال دفتر اليومية**بعد الآن وسيعكس (\_ المبلغ المفوتر - المبلغ المقدم) \_:

![](https://docs.erpnext.com/files/vaXYQNc.png)
