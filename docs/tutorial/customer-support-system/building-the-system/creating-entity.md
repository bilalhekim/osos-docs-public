---
title: " الكيان"
sidebar_position: 2
---

# بناء كيان تذاكر الدعم 
الكيان هو العنصر الرئيسي لتخزين البيانات ويمكن تشبيهها بالجداول في قواعد البيانات، حيث يتم تعريفها في كل نظام لتمثيل أقسام أو عناصر مختلفة 
(للمزيد حول الكيان اطلع على : [الكيانات](../../../guide/information-structures-concepts/basic-concepts/entities.md)).

## إضافة كيان تذاكر الدعم 
لبناء كيان ضمن وحدة دعم العملاء يضم العمليات على تذاكر الدعم يجب اتباع الخطوات التالية:
1. النقر على وحدة دعم العملاء.
2. الضغط على زر **إضافة كيان**.
   
![image info](../../../../static/img/tutorial/customer-support-system/customer-support-creating-entity(1).png)

تظهر نافذة إضافة كيان يتعين عليك ملء بيانات الكيان:
1. **الاسم (إلزامي):** نقوم بتسميته  "تذاكر الدعم" باللغتين العربية والانكليزية.
2. **الأيقونة (إلزامي):** يجب على مدير النظام اختيار الايقونة الخاصة بالكيان ولنقم هنا باختيار ايقونة مفتاح الربط"**wrench**".
3. **نوع الكيان(إلزامي):**  يجب على مدير النظام تحديد نوع الكيان وفي هذا الحالة يكون نوع الكيان "كيان طبيعي" وللمزيد حول أنواع الكيانات اطلع على : [الكيانات](../../../guide/information-structures-concepts/basic-concepts/entities.md)).
4. **الحقل النموذجي(إلزامي):** يتم توليد هذا الحقل تلقائياً بمجرد كتابة اسم الكيان باللغة العربية أو الإنجليزية، ولكن يمكن لمدير النظام تعديل هذا الحقل، ولا يمكن تركه فارغًا. لمزيد من المعلومات حول الحقل النموذجي اطلع على : [الحقل النموذجي](../../../guide/information-structures-concepts/basic-concepts/modules.md).
5. **حقل الوحدة(إلزامي):** هو حقل مقفل لا يمكن التعديل عليه , مملوء تلقائياً باسم الوحدة الذي يتم إنشاء الكيان ضمنها "نظام دعم العملاء".
6. **اسم المفرد(اختياري):** وهو الاسم المفرد من مدخلات الكيان وهنا يكون "تذكرة الدعم" يتم كتابته باللغتين العربية والإنكليزية.
7. **اسم الجمع:** وهو اسم الجمع من عناصر الكيان ويكون هنا "تذاكر الدعم" يتم كتابته باللغتين .
8. **إدارة السماحيات أو الصلاحيات (اختياري):** يمكن لمدير النظام التحكم في صلاحيات الكيان حسب الحاجة.لمزيد من المعلومات حول الصلاحيات اطلع على  [الصلاحيات](../../../guide/information-structures-concepts/basic-concepts/permissions.md).
9. الضغط على زر "إنشاء" فيتم إنشاء كيان "تذاكر الدعم".

![image info](../../../../static/img/tutorial/customer-support-system/customer-support-creating-entity(2).png)

## إضافة بنية الكيان
فور إضافة الكيان يتم توجيه المستخدم إلى صفحة تفاصيل الكيان ولبناء بنية الكيان يتم اتباع الخطوات التالية: 
1. الضغط على نافذة **البنية** .
2. تظهر صفحة فارغة.
3. سحب وإفلات الحقول الخاصة بالبنية ضمن المنطقة الفارغة والحقول كالتالي:

![image info](../../../../static/img/tutorial/customer-support-system/customer-support-creating-entity(3).png)

  - رقم التذكرة(حقل متسلسل).
  - عنوان التذكرة(نص متعدد اللغات).
  - وصف التذكرة(نص متعدد اللغات).
  - حالة التذكرة(تصنيف): حالات التذكرة(مفتوحة,قيد المعالجة,الرد على التذكرة,مكررة, مغلقة).
  - المسند إليه (مستخدم).
  - تاريخ فتح التذكرة(تاريخ ووقت).
  - تاريخ إغلاق التذكرة(تاريخ ووقت).
  - الحل(كتلة).
  - الحل "نص متعدد اللغات".
  - تقييم الخدمة(كتلة).
  - درجة التقييم(محول):إضافة خيارات التقييم من (1-5).
  - الضغط على ايقونة الخيارات الموجودة في اقصى يسار الحقل.
  - إضافة الخيارات التالية لحقل درجة التقييم.
  - التعليق(نص متعدد اللغات).
4. الضغط على زر "حفظ"  لحفظ هيكلية أو بنية كيان "تذاكر الدعم".


  ![image info](../../../../static/img/tutorial/customer-support-system/customer-support-creating-entity(4).png)
  ![image info](../../../../static/img/tutorial/customer-support-system/customer-support-creating-entity(5).png)
  ![image info](../../../../static/img/tutorial/customer-support-system/customer-support-creating-entity(6).png)
  ![image info](../../../../static/img/tutorial/customer-support-system/customer-support-creating-entity(7).png)


## إضافة سير العمل:
لبناء سير عمل للكيان يتم اتباع الخطوات التالية:

  - الضغط على نافذة سير العمل.
  - تظهر صفحة سير العمل.
  - الضغط على "اضغط لتفعيل مسارالعمل" الموجودة في منتصف الصفحة.
  - تم تفعيل سير العمل

  ![نافذة سير العمل](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(1).png).

  ![صورة 2](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(2).png)

  - الضغط على "البداية" لتغيير اسم خطوة العمل.
  - تظهر إعدادات الخطوة.
  - تغيير اسم "البداية" إلى اسم "فتح تذكرة".

  ![صورة 3](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(3).png)

  - تغيير اسم الإجراء "البدء" إلى "إرسال الطلب".

  ![صورة 4](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(4).png)

  - تغيير إعدادات الحقول ضمن الخطوة من خلال الضغط على "فتح التذكرة".
  - الضغط على "قابل للتغيير" فتظهر خيارات الحقل نختار منها حسب ما نريد عرضه.

  ![صورة 5](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(5).png)
  
  ![صورة 6](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(6).png)

  - نقوم ببناء الخطوة الثانية وهي "مكتب الدعم" من خلال الضغط على "إضافة خطوة".
  
  ![صورة 7](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(7).png)

  - تظهر نافذة منبثقة نقوم من خلالها بملء معلومات الخطوة.
  - الضغط على زر "إنهاء" لحفظ الخطوة.
 
  ![صورة 8](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(8).png)
 
  ![صورة 9](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(9).png)

  - في حال أردنا حذف الخطوة نقوم بالضغط على "حذف خطوة".
   ![صورة 10](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow.png)

  - تغيير اسم "الإجراء الأساسي" إلى "إرسال للمعالجة" كما فعلنا في أول خطوة.
    
  ![صورة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(10).png)  
  
  ![صورة 11](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(11).png)
  
  - بناء خطوة جديدة "معالجة التذكرة" باتباع نفس الخطوات السابقة لبناء خطوة.
    
  ![صورة 11](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(12).png)
  ![صورة 11](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(13).png)
  
  - تغيير اسم "الإجراء الرئيسي" إلى "مراجعة الحل"
  - تغيير الخطوة الهدف إلى "الخطوة السابقة"

  ![صورة 11](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(14).png)
  
  - إضافة خطوة جديدة "تقييم الخدمة" باتباع نفس الخطوات السابقة لإضافة خطوة.
  - تغيير اسم "الإجراء الأساسي" إلى "تم التقييم".
  - تغيير الخطوة الهدف إلى "مكتب الدعم".
  - تغيير إعدادات الحقول لخطوة "تقييم الخدمة".
  ![صورة 14](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(15).png)
 
  ![صورة 15](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(16).png)
  
  ![خطوة موافقة المدير](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(17).png)
  
   ![خطوة تقييم الخدمة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(33).png)

  ![إعدادات الحقول](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(34).png)
 
  
   - تغيير الخطوة الهدف في إجراء "إرسال للمعالجة" في الخطوة الثانية "مكتب الدعم" إلى "معالجة التذكرة".

  ![خطوة موافقة المدير](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(18).png)
  
  ![خطوة موافقة المدير](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(19).png)

  - إضافة إجراء جديد "إغلاق التذكرة" من خلال الضغط على إشارة **+** الموجودة أعلى الخطوة.
  - تظهر شاشة منبقة نقوم بملئها بمعلومات الإجراء.
  ![خطوة موافقة المدير](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(20).png)

  - إضافة إجراء جديد "إرسال الحل".
 ![خطوة موافقة المدير](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(21).png)

  ![خطوة معالجة التذكرة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(22).png)

  ![خطوة معالجة التذكرة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(23).png)

  - بناء خطوة جديدة "موافقة المدير" باتباع نفس الخطوات السابقة لبناء خطوة.
  - تغيير اسم "الإجراء الأساسي" إلى "موافق".
  - تغيير الخطوة الهدف إلى "الخطوة السابقة".
  ![خطوة معالجة التذكرة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(24).png)
 
  ![الإجراء الأساسي](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(25).png)
  
  ![إعدادات الحقول](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(26).png)
  
  - إضافة إجراء جديد لخطوة "موافقة المدير"  هو "رفض" باتباع نفس الخطوات السابقة.
  ![إعدادات الحقول](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(27).png)

  - إضافة إجراء جديد في الخطوة الثانية "مكتب الدعم" هي "موافقة المدير" كما فعلنا سابقاً.
  - الضغط على إشارة **+** الموجودة في أعلى الخطوة.
 
  ![إضافة إجراء جديد](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(28).png)

   - تغيير إعدادات حقول خطوة "مكتب الدعم" .

  ![خطوة تقييم الخدمة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(29).png)
 
  ![خطوة تقييم الخدمة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(30).png)
  
   - تغيير إعدادات حقول خطوة "معالجة التذكرة"
   - يمكننا ايضاً حذف خطوة من خلال الضغط على زر "حذف خطوة" الموجود في إعدادات الخطوة.
   ![خطوة تقييم الخدمة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(31).png)

  ![خطوة تقييم الخدمة](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(32).png)
  
  - الضغط على زر "حفظ" لحفظ سير العمل.
  - في حال أردنا حذف سير العمل نقوم بالضغط على أيقونة سلة الحذف الموجودة أعلى سير العمل.
  - 
  ![حذف سير العمل](../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(35).png)

لمزيد من المعلومات حول سير العمل أو تدفق العمل، يمكنك الاطلاع على
[تدفق العمل](../../../guide/information-structures-concepts/basic-concepts/workflows.md).


## إضافة التفاعلات
يمكنك من خلال التفاعلات تعيين الاشعارات وإرسالها إلى الجهات المعنية ولكي تقوم بإضافة إشعار اتبع الخطوات التالية : 
  - الضغط على تبويبة التفاعلات في صفحة تفاصيل الكيان.
  - الضغط على ايقونة "+".

![الرد على العميل](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(1).png)

  - تظهر شاشة منبثقة لملء معلومات التفاعلات .
  - إضافة تفاعل "الرد على العميل".

![الرد على العميل](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(2).png)

![الرد على العميل](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(3).png)

![الرد على العميل](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(4).png)

  - إضافة تفاعل ثاني  "وصول تذكرة جديدة" باتباع نفس الخطوات السابقة وملء معلومات التفاعل.

![وصول تذكرة جديدة](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(5).png)

![وصول تذكرة جديدة](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(6).png)

![وصول تذكرة جديدة](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(7).png)

  - إضافة تفاعل جديد "تم إسناد التذكرة إليك" باتباع نفس الخطوات السابقة.

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(8).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(9).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(10).png)

  - إضافة تفاعل جديد باسم "مراجعة الحل" باتباع نفس الخطوات السابقة لإضافة تفاعل.

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(11).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(12).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(13).png)

  - إَضافة تفاعل جديد "تمت مراجعة الحل" .

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(14).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(15).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(16).png)

  - إضافة تفاعل "تم حل الطلب".

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(17).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(18).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(19).png)

  - إضافة تفاعل "تقييم الخدمة" .

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(20).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(21).png)

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(22).png)

  - الضغط على زر "حفظ" لحفظ التفاعلات .

![تم إسناد التذكرة إليك](../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(23).png)

ولمزيد من المعلومات حول التفاعلات، يمكنك الاطلاع على [التفاعلات](../../../guide/information-structures-concepts/basic-concepts/reactions-and-automation.md).



