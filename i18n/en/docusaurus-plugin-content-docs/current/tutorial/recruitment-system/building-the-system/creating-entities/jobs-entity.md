---
title: "كيان الوظائف"
sidebar_position: 2
---

# كيان الوظائف 
 هذا الكيان مخصص لتتبع وإدارة معلومات الوظائف المتاحة.
 
ولمزيد من المعلومات حول الكيانات، يمكنك الاطلاع على [الكيان](../../../../guide/information-structures-concepts/basic-concepts/entities).

## إنشاء كيان الوظائف

1.  انقر على زر **أضف كيان** بعد الدخول إلى وحدة **نظام التوظيف**.

![إضافة كيان](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(1).png)

2. ستظهر نافذة إنشاء كيان جديدة حيث يجب عليك إدخال المعلومات التالية:
   
   - **اسم الكيان**: قم بإدخال اسم الكيان **الوظائف** و أدخل الترجمة بالانجليزية.
   - **اختيار الرمز**: حدد رمزًا للكيان لتمثيله بصريًا.
   - **نوع الكيان**: حدد **كيان عادي**.
   - **في قسم الإعدادات المتقدمة**: قم بإدخال اسم الكيان بالمفرد و الجمع.

3. بمجرد إدخال جميع المعلومات، انقر على زر **إنشاء**،هكذا تمت إضافة كيان **الوظائف** بنجاح

![إضافة كيان](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(2).png)

### إنشاء البنية

1. انتقل إلى وحدة **نظام التوظيف**: للوصول إليها،في الشريط الجانبي انقر على **الإدارة**، ثم **التطبيقات**، ثم **الوحدات**. ابحث عن **نظام التوظيف** وانقر عليه.

2. داخل **نظام التوظيف**، انتقل إلى علامة التبويب **الكيانات**.

3. في قائمة الكيانات، ابحث عن **الوظائف** وانقر على **...** في بطاقته.

4. اختر **تعديل الكيان** للوصول إلى واجهة تعديل الكيان.

![تعديل الكيان](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(4).png)

5. انتقل إلى علامة التبويب **البنية**.

![إضافة حقل النص المترجم](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(5).png)

6.  داخل قائمة الحقول الجانبية، ابحث عن **نص متعدد اللغات** واسحبه إلى منطقة بناء البنية ثم أفلته. أدخل اسم الحقل (عنوان الوظيفة)و أدخل الترجمة بالانجليزية، وحدد خيار **مطلوب**.

![إضافة حقل النص المترجم](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(6).png)

7. بنفس الطريقة فم بإضافة حقل **الوصف**

![إضافة حقل الوصف](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(7).png)


8. الآن، ابحث عن حقل **ارتباط** واسحبه إلى منطقة بناء البنية ثم أفلته. ستظهر نافذة منبثقة لإدخال الكيان المراد الارتباط به. ابحث عن **الوحدات التنظيمية** وحددها، ثم انقر على **حفظ**. أدخل اسم الحقل **القسم** و أدخل الترجمة بالانجليزية واجعله مطلوبًا.

![إضافة حقل ارتياظ](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(8).png)

![إضافة حقل ارتياظ](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(9).png)

9. قم بإضافة حقل **ارتباط** آخر بنفس الطريقة، واسحبه إلى منطقة بناء البنية. ستظهر نافذة لإدخال الكيان/القائمة المراد الارتباط بها. اختر القوائم ثم ابحث عن **الجدارات** (لقد قمنا بإنشاء هاته القائمة مسبقا) وحددها، ثم انقر على **حفظ**. أدخل اسم الحقل **المؤهلات المطلوبة** واجعله مطلوبًا.

![إضافة حقل مجموعة مراجعة](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(10).png)

10. قم بإضافة حقل **ارتباط** آخر بنفس الطريقة، واسحبه إلى منطقة بناء البنية. ستظهر نافذة لإدخال الكيان/القائمة المراد الارتباط بها. اختر القوائم ثم ابحث عن **المؤهلات الدراسية** (لقد قمنا بإنشاء هاته القائمة مسبقا) وحددها، ثم انقر على **حفظ**. أدخل اسم الحقل **المؤهلات الدراسية** واجعله مطلوبًا.

![إضافة حقل مجموعة مراجعة](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(11).png)

11. ابحث عن **تصنيف** واسحبه إلى منطقة بناء البنية. ستظهر نافذة لإدخال الخيارات. أدخل خيار**-1 سنة** و أدخل الترجمة بالانجليزية في الحقل النصي، ثم اختر لونًا لهذا الخيار باستخدام مولد الألوان، وانقر على زر **إضافة**، قم بتكرار هذه العملية للخيارات الأخرى **1 سنة**، **2-5 سنوات**، **5-10 سنوات**، **+10 سنوات**. قم بإدخال **سنوات الخبرة المطلوبة** كاسم الحقل و أدخل الترجمة بالانجليزية،ثم حدد الحقل كــ **مطلوب**.

![إضافة حقل تصنيف](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(12).png)

12. ابحث عن **تصنيف** واسحبه إلى منطقة بناء البنية. ستظهر نافذة لإدخال الخيارات. أدخل خيار **عن بعد** و أدخل الترجمة بالانجليزية في الحقل النصي، ثم اختر لونًا لهذا الخيار باستخدام مولد الألوان، وانقر على زر **إضافة**، قم بتكرار هذه العملية للخيارات الأخرى **هجين** و **حضوري**. قم بإدخال **الموقع** كاسم الحقل و أدخل الترجمة بالانجليزية،ثم حدد الحقل كــ **مطلوب**.

   ![إضافة حقل تصنيف](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(13).png)

13. ابحث عن **عدد** واسحبه إلى منطقة بناء البنية. أدخل **ساعات العمل في اليوم** كاسم الحقل و أدخل الترجمة بالانجليزية، وحدد الحقل كـ **مطلوب**.

   ![إضافة حقل العدد](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(14).png)

14. ابحث عن **تاريخ** واسحبه إلى منطقة بناء البنية. أدخل **آخر موعد للتسجيل** كاسم الحقل و أدخل الترجمة بالانجليزية، وحدد الحقل كـ **مطلوب**.

   ![إضافة حقل التاريخ](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(15).png)

15. الآن، ابحث عن **تصنيف** واسحبه إلى منطقة بناء البنية. ستظهر نافذة لإدخال الخيارات. أدخل **مفتوحة**و أدخل الترجمة بالانجليزية في الحقل النصي، ثم اختر لونًا لهذا الخيار باستخدام مولد الألوان، وانقر على زر **إضافة**. قم بتكرار هذه العملية للخيارات الأخرى **مغلقة** و **مؤرشفة**.

   ![إضافة حقل تصنيف](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(16).png)

16. أضف حقل نص متعدد اللغات **تعليقات الموارد البشرية**

   ![إضافة حقل تصنيف](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(17).png)


17. بعد الانتهاء من إضافة الخيارات، انقر على **حفظ**.

18. انقر على **حفظ** في أعلى الصفحة.

### إنشاء سير العمل

1. في نفس الصفحة انتقل إلى تبويبة **سير العمل**

![بدأ سير العمل](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(18).png)

2.  قم بالنقر فوق المنطقة المشار إليها في الصورة لبدأ سير العمل، سينشأ سير عمل بخطوتين افتراضيتين **البداية  و النهاية**.

![سير عمل افتراضي](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(19).png)

3. ابدأ أولا بتغيير اسم الخطوة الأولى **البداية** إلى **وظيفة جديدة**، من خلال النقر فوق اسم الخطوة، لتظهر نافذة إعدادات الخطوة، قم بتغيير قيمة حقل الاسم، بعد تغيير الاسم قم بالضغط على علامة **X** أو النقر فوق المنطقة الرمادية خارج نافذة الاعدادات للعودة إلى سير العمل.

![سير العمل الافتراضي](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(20).png)

4. انقر فوق **+ إضافة خطوة** لإضافة خطوة جديدة

![إضافة خطوة جديدة](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(21).png)

5. ستفتح تافذة معلومات الخطوة، قم بإدخال المعلومات كما هو موضح  في الصور التالية :

![نافذة إضافة خطوة جديدة 1](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(22).png)

![نافذة إضافة خطوة جديدة 2](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(23).png)

![نافذة إضافة خطوة جديدة 3](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(24).png)

6. قم بتغيير اسم الإجراء الرئيسي إلى **موافقة**.

![تغيير اسم الإجراء الرئيسي](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(25).png)

7. قم بإضافة خطوة جديدة **نشر الوظيفة** باتباع نفس الخطوات السابقة لإضافة خطوة.

![خطوة جديدة **نشر الوظيفة**](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(63).png)

![خطوة جديدة **نشر الوظيفة**](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(66).png)

8. قم بتغيير اسم الإجراء الرئيسي إلى **إنهاء**.

9. انقر فوق زر الحفظ أعلى الصفحة لحفظ إعدادات الكيان بما فيها سير العمل

   ![حفظ تعديلات الكيان](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(27).png)

### إنشاء التفاعلات

- في هذا القسم، سنقوم بإنشاء مجموعة من التفاعلات المهمة لكيان الوظائف. يتضمن كل تفاعل معلومات حول الحدث المستدعي والإجراءات المطلوبة. يمكنك اتباع الخطوات التالية لإعداد هذه التفاعلات.

   1. انتقل إلى علامة التبويب **التفاعلات**.

      ![انتقل إلى التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(28).png)

   2. انقر على **إضافة تفاعل** لإنشاء تفاعل جديد.

      ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(29).png)


   3. تفاعل إرسال إشعار إلى إدارة الموارد البشرية عند إنشاء وظيفة جديدة

      1.  قم بإخال التفاصيل المشار إليها في الصور التالية

      ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(30).png)

      ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(31).png)

      2. انقر على **إضافة تفاعل** لإضافته إلى قائمة التفاعلات 

      ![إضافة التفاعل](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(33).png)

      3. اضغط على **حفظ** لحفظ التفاعل

      ![حفظ التفاعل](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(34).png)

- بنفس الخطوات السابقة سنضيف باقي التفاعلات أدناه : 

   4. تفاعل إرسال إشعار إلى مُنشئ الوظيفة عندما تتم الموافقة عليها

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(35).png)

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(36).png)


   5. تفاعل لإرسال إشعار إلى مُنشئ الوظيفة عندما يتم أرشفتها

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(38).png)

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(39).png)

   6. تفاعل لإرسال إشعار إلى مُنشئ الوظيفة عندما يتم إرجاع الوظيفة

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(41).png)

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(42).png)

   7. تفاعل لتغيير حالة الوظيفة إلى**مقبولة**

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(44).png)

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(45).png)

   8. تفاعل لتغيير حالة الوظيفة إلى**مؤرشفة**

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(47).png)

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(48).png)

   9. تفاعل لتغيير حالة الوظيفة إلى**مغلقة**

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(49).png)

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(50).png)

   10. تفاعل نقل سير العمل إلى خطوة البداية عند إنشاء مدخل جديد

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(51).png)

   11. تفاعل نقل سير العمل إلى خطوة النهاية عندما يصبح التاريخ اليوم هو تاريخ آخر موعد للتقديم

   ![إضافة التفاعلات](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(53).png)

   12. انقر فوق زر **حفظ** مرة أخرى لتأكيد حفظ جميع التفاعلات المضافة


### إنشاء الشريط الزمني

- الشريط الزمني سيلعب دورا مهما في عملية نشر و حجب الوظائف حسب الحالة (مفتوحة أو مغلقة)، لإعداده بشكل صحيح قم بتتبع المراحل التالية : 

   1. في صفحة تعديل كيان الوظائف، قم بالانتقال إلى تبويبة **شريط زمني**، ثم قم بالنقر وسط الصفحة للإضافة شريط زمني

   ![الشريط الزمني](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(62).png)

   2. قم بإدخال التفاصيل المشار إليها في الصور النالية

   ![الشريط الزمني](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(59).png)

   ![الشريط الزمني](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(60).png)

   ![الشريط الزمني](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(61).png)

   - بالنسبة للصورة المضافة في حقل القيمة بالنسبة للمرفقات، يمكنك استعمال أي صورة لديك مناسبة لمنشورات الوظائف الجديدة، مثلا هنا استعملنا الصورة التالية

   ![الشريط الزمني](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-job-entity-creating-entity(58).png)

   3. انقر فوق زر حفظ أعلى الصفحة، لحفظ إعدادات الشريط الزمني

   