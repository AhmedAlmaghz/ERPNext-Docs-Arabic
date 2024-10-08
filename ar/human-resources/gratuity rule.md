\n\> تم تقديم هذه الميزة في الإصدار 13 ، والتي ستكون جزءًا من وحدة كشوف المرتبات المنفصلة.

**قاعدة الإكراميات هي مجموعة من القواعد التي يحددها المركز أو الولاية المستخدمة أثناء حساب مبلغ المكافأة**

في Frappe HR ، يمكنك تحديد قواعد إكرامية مختلفة بناءً على منطقة مختلفة.

للوصول إلى قاعدة الإكراميات ، انتقل إلى:

\> الصفحة الرئيسية> كشوف المرتبات> قاعدة الإكراميات

## 1. المتطلبات الأساسية

قبل إنشاء قاعدة المكافأة ، يُنصح بإنشاء ما يلي:

1. [موظف](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/employee)
2. [مكون الراتب](https://docs.erpnext.com/docs/v14/user/manual/en/human-resources/salary-component)

## 2. كيفية إنشاء قاعدة الإكراميات

1. حصلت على قاعدة الإكراميات> جديد
2. حدد المكونات القابلة للتطبيق. تساهم مكونات الراتب هذه أثناء احتساب المكافأة.
3. حدد "حساب مبلغ المكافأة على أساس"
4. تحديد قاعدة المكافأة
5. حفظ

![قاعدة الإكراميات](https://docs.erpnext.com/files/gratuity-rule.png)

## 3. خصائص إضافية

يتم تحديد بعض السمات الإضافية المستخدمة أثناء احتساب المكافأة أدناه.

### 3.1 طريقة حساب الخبرة في العمل:

توفر Frappe HR طريقتين مختلفتين لحساب خبرة العمل.

1. تقريب طريقة خبرة العمل قرب تجربتك الحالية. على سبيل المثال ، إذا كان الموظف لديه خبرة إجمالية مدتها 3 سنوات و 6 أشهر ، فسيتم التعامل معه على أنه خبرة 4 سنوات.
2. خذ السنة المكتملة بالضبط.

### 3.2 احسب مبلغ الإكرامية بناءً على:

دعنا نفكر في المثال التالي لفهم العملية الحسابية.

![gratuity-rule-example](https://docs.erpnext.com/files/gratuity-rule-example.png)

1.**الشريحة الحالية:**إذا كان حساب مبلغ المكافأة يعتمد على الشريحة الحالية ، فسيكون المبلغ ناتجًا عن خبرة العمل (بالسنوات) ، وجزء من الأرباح المطبقة ، وتجميع مكونات الأرباح المطبقة. بناءً على قواعد / لوح الإكراميات أعلاه ، إذا كان الموظف لديه خبرة 5 سنوات ، فإنه يقع في الشريحة الثالثة. سيكون حساب مبلغ المكافأة على النحو التالي:

\> مبلغ الإكرامية = 5 \ * 0.467 \ * (متأخر + أساسي)

2.**مجموع كل الألواح السابقة:**إذا كان حساب مبلغ المكافأة يعتمد على مجموع كل الألواح السابقة ، فسيكون المبلغ هو مجموع منتج الألواح الفردية حتى سنة الخبرة وتجميع مكون الأرباح المطبق. بناءً على قواعد / لوح المكافأة أعلاه ، إذا كان الموظف لديه خبرة 5 سنوات ، فسيكون حساب مبلغ المكافأة على النحو التالي:

\> مبلغ الإكرامية = \ [(1 \ * 0) + (2 \ * 0.233) + (2 \ * 0.467) \] \ * (متأخر + أساسي)