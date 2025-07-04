---
title: "الحقول"
sidebar_position: 3
---

# الحقول 
هي الوحدات الأساسية التي تحمل البيانات في كل سجل أو كيان. تصف الحقول البيانات التي يتم تخزينها في كل مدخل أو سجل داخل النظام. تتميز الحقول بخصائص مختلفة تسهل تنظيم وإدارة البيانات.



## خصائص الحقل العامة	
### أنماط البيانات
1. تاريخ:
الغرض: تمثيل التواريخ بتنسيق اليوم/الشهر/السنة.
2. قيمة منطقية:
الغرض: إشارة إلى القيمة صحيحة أو خاطئة.
3. تاريخ/وقت:
الغرض: تمثيل الطوابع الزمنية بتنسيق اليوم/الشهر/السنة والساعة/الدقيقة.
4. أيقونة:
الغرض: اختيار وعرض أيقونة.
5. نص:
الغرض: تمثيل النصوص القصيرة والوصف والمحتوى النصي.
7. رقم:
الغرض: تمثيل القيم الرقمية بما في ذلك الأعداد الصحيحة والكسور.
8. وقت:
الغرض: تمثيل الوقت بتنسيق الساعة/الدقيقة.

### الحقل الإلزامي	
يُعرف هذا النوع من الحقول بأنه حقل يجب ملؤه عندما يتم إنشاء أو تحديث مدخل في النظام. يساهم في ضمان أن تحتوي كل مدخلات البيانات على المعلومات الأساسية المطلوبة. على سبيل المثال، حقل "اسم المستخدم" في سجل المستخدمين قد يكون حقلًا إلزاميًا لأنه يجب أن يحتوي على معلومات تعريفية فريدة لكل مستخدم.
### الحقل الفريد    
هذا النوع من الحقول يتطلب أن تكون القيم المخزنة فيه فريدة وغير مكررة في كل مدخلات. يُستخدم هذا النوع من الحقول لضمان عدم تكرار بعض البيانات الرئيسية في النظام. على سبيل المثال، حقل "البريد الإلكتروني" كحقل فريد يضمن عدم وجود عناوين بريد إلكتروني متكررة بين المستخدمين.  
### القيمة الافتراضية	
تعني هذه الخاصية تحديد قيمة افتراضية للحقل. عند إنشاء مدخل جديد وعدم إدخال قيمة محددة، يتم استخدام القيمة الافتراضية كبديل. هذا يُسهل عملية ملء الحقول ويضمن وجود قيمة للحقل حتى إذا لم يقم المستخدم بتحديدها. على سبيل المثال، تاريخ الإنشاء الافتراضي لسجل جديد يمكن أن يكون تاريخ اليوم.
### التكرار	
هذه الخاصية تسمح بإمكانية إضافة نفس الحقل بقيم مختلفة داخل نفس السجل أو المدخل. عند تفعيل هذه الخاصية، يُمكن للمستخدم إضافة مجموعة من القيم لنفس الحقل في سجل واحد. فمثلاً، في حقل "الملاحظات"، يُمكن تفعيل خاصية التكرار ليتمكن المستخدم من إضافة مجموعة متنوعة من الملاحظات في نفس السجل.
### الظهور والخفاء	
هذه الخاصية تتيح التحكم في رؤية الحقول بناءً على شروط معينة. بالتالي، يمكن إظهار أو إخفاء الحقول استنادًا إلى متطلبات محددة أو حالات معينة. مثلاً، يمكن أن يتم إظهار حقل إضافي إذا تم تحديد "نوع معين" للسجل.
### الحقل  المُقفل     
هذا النوع من الحقول يمنع التعديل أو التغيير على القيمة المخزنة فيه. يُستخدم هذا الحقل لحماية البيانات الحساسة أو البيانات التي لا يجب تغييرها يدويًا. على سبيل المثال، تاريخ إنشاء يمكن أن يكون محقلاً مقفلاً لمنع تغييره.
### تعدد القيم	
عند تفعيل هذه الخاصية، يُمكن للمستخدم اختيار أكثر من قيمة من بين الخيارات المتاحة في الحقل. فعلى سبيل المثال، في حقل "الألوان المُفضلة"، يُمكن تفعيل تعدد القيم ليسمح للمستخدم باختيار أكثر من لون واحد كمفضل لديه.


## مهم أن تعرف 
### ما هي الكتلة	
حقل الكتلة هو حقل يسمح بتجميع مجموعة من الحقول تحت تسمية واحدة داخل إطار موحد. يُستخدم لتنظيم وتجميع مجموعة من الحقول ضمن هيكل واحد. يتيح للمستخدم تنظيم العرض النهائي للبيانات، سواء عبر عرض المحتوى داخل تبويب خاص للحقل الكتلة أو ضمن العرض الرئيسي للمدخل. توفر هذه الميزة مرونة أكبر في التعامل مع البيانات، خاصة عندما يكون هناك عدد كبير من الحقول في الكيان.

إذا تم تكوين حقل الكتلة على أنه قابل للتكرار، فهذا يسهل تكرار البيانات دون الحاجة إلى إنشاء مدخل جديد بالكامل، مما يُسهّل عملية تنظيم وإدخال البيانات ويزيد من فعالية استخدام النظام.
### حقل الارتباط	
حقل الارتباط هو عبارة عن حقل يتيح للمستخدم ربط المدخل الحالي بمدخل آخر في الكيان أو تجميعة أخرى. يُستخدم لإنشاء روابط وعلاقات بين الكيانات والتجميعات ذات الصلة.

هذا الحقل يسمح بربط المدخل الحالي مع مدخل آخر في نفس الكيان أو في تجميعة أخرى، مما يسمح بإنشاء علاقات بين مختلف العناصر في النظام. يُستخدم على نطاق واسع لتنظيم البيانات وربطها معًا بطريقة تمكن من تتبع العلاقات بين المكونات المختلفة لتحسين فهم البيانات وتحليلها.


### حقل التصنيف	

حقل التصنيف هو عبارة عن حقل يسمح للمستخدم باختيار قيمة من بين عدة خيارات مُحددة مسبقًا، والتي يقوم المستخدم بتعيينها لكل كيان على حدة. يُستخدم غالبًا لتمييز حالات محددة لكل مدخل عن الآخرين، مع إمكانية تحديد ألوان مميزة لكل قيمة.

الفائدة الرئيسية لحقل التصنيف هي تمكين التمييز بين حالات مختلفة لكل مدخل في النظام. يُمكن استخدامه في إنشاء خلاصات أو تجميعات بناءً على هذا الحقل لفهم الحالات المختلفة أو لتسهيل التصفية والتنظيم حسب القيم المختارة.



## المفاهيم المرتبطة 
- [الكيانات](./entities.md)
- [القوائم](./lists.md)


**(للمزيد حول العمليات على الحقول اطلع على : [إدارة الحقول](../../data-management/field-types))**