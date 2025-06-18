---
title: "اختبار النظام"
sidebar_position: 5
---

# اختبار نظام التوظيف 
هذا الاختبار يهدف إلى التحقق من أن جميع مكونات نظام التوظيف تعمل بشكل صحيح. يتضمن هذا الاختبار إجراءات لمختلف المستخدمين في النظام.

## إنشاء شاغر جديد
- هاته المرحلة ستتم بين الأدوار التالية : 
    - عضو الموارد البشرية
    - عضو قسم تقنية المعلومات

**1. إنشاء أدوار المستخدمين:**
   - قم بإنشاء دور "عضوة إدارة الموارد البشرية" وأضفه إلى مجموعة "الموارد البشرية".
   
   ![HR member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(1).png)

   - ثم قم بإنشاء دور "عضو تقنية المعلومات" وأضفه إلى مجموعة "تقنية المعلومات".
   
   ![IT member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(2).png)

**2. تسجيل الدخول:**
   - قم بفتح متصفح وقم بتسجيل الدخول إلى النظام باستخدام حساب عضو الموارد البشرية.    
   ![hr member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(3).png)

   - قم بفتح متصفح آخر وقم بتسجيل الدخول إلى النظام باستخدام حساب عضو تقنية المعلومات.
   ![IT member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(4).png)

**3. إنشاء وظيفة جديدة:**
   - في متصفح عضو تقنية المعلومات، انتقل إلى صفحة "نظام التوظيف" من الشريط الجانبي للنظام.
   - انقر على "أنشئ وظيفة جديدة في قسم الروابط السريعة".
   ![IT member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(5).png)
   ![IT member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(6).png)
   - قم بملء النموذج بالمعلومات المطلوبة وانقر على "إرسال".
   ![IT member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(7).png)
   ![IT member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(8).png)

**4. الموافقة على الوظيفة:**
   - انتقل إلى المتصفح الذي قمت بتسجيل الدخول به كعضو الموارد البشرية.
   -سيصلك إشعار جديد يخبرك بأنه تم إنشاء وظيفة جديدة.
    ![HR member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(10).png)
   - انقر على الإشعار وقم بالموافقة على الوظيفة.
   ![HR member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(11).png)
   ![HR member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(12).png)
   - قم بنشر الوظيفة
   ![HR member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(13).png)
   ![HR member](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(14).png)

**5. التحقق من الوظيفة:**
   - انتقل إلى علامة تبويب متصفح جديد أو نافذة خاصة وقم بفتح هذا [الرابط](https://onboarding.osos.roaa.tech/v/bed19094-9aec-451d-ac5c-2743dc0a3966/entries/add).
   
   - يجب أن ترى الوظيفة الجديدة هناك. قم بالتحقق من صحة ظهورها.

بالطبع، سأقوم بتصحيح السيناريو وتنظيمه بشكل أفضل:

## تقديم و تتبع طلب وظيفي
- هاته العملية ستتم بين الأدوار التالية : 
    - عضو الموارد البشرية
    - مستخدم مجهول سيتم إدخال بريده الاكتروني أثناء ملأ الطلب الوظيفي، و هو الذي سنعتمد عليه هنا
    - مسؤول التواصل مع المترشح

**6. التقديم للوظيفة:**
   - في علامة تبويب المتصفح التي تم فتحها بدون حساب (مجهول)، انقر على الرابط المتوفر في منشور الوظيفة التي أنشأناها في المراحل السابقة.
   
      ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(15).png)

   - سيتم فتح نموذج طلب وظيفي جديد.
   - قم بملء النموذج بالمعلومات المطلوبة وقم بإرسال النموذج.

      ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(16).png)

   - سستظهر النافذة التالية عندما تقوم بحفظ الطلب بشكل صحيح

      ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(17).png)


**7. مراجعة الطلب:**
   - انتقل إلى علامة تبويب متصفح عضو الموارد البشرية.
   - ستتلقى إشعارًا جديدًا يُخطرك بوصول طلب وظيفي جديد.

      ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(18).png)

   - انقر على الإشعار لمراجعة الطلب.
   - الطلب الآن في مرحلة معالجة الطلب
      ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(42).png)

      ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(19).png)

   - قم بتعديل تفاصيل الطلب لإدخال معلومات التقييم الأولي 

      ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(20).png)

   - إذا كان المترشح مؤهلا، قم بتحديد  مسؤول التواصل ومعلومات المقابلة الأولى

      ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(21).png)

- أنقر فوق **المقابلة** لتمرير سير العمل للخطوة الموالية

   ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(43).png)


**9. المقابلة L1:**
   - ستصل رسالة خاصة بتفاصيل المقابلة إلى البريد الالكتروني الذي قمت بإدخاله أثناء ملأ نموذج الطلب (بريد المترشح)، كما ستصل إشعارات دعوات حضور المقابلة ‘لى كل من الحضور و مجري المقابلة
   - باعتبار أن المقابلة تمت بنجاح. انتقل إلى علامة تبويب متصفح عضو الموارد البشرية.
   - انقر على "البريد الوارد" في "الخدمات" في الشريط الجانبي
   - ابحث عن الطلب الوظيفي الحالي، أو قم بالدخول إلى تفاصيل الطلب مباشرة،عن طريق الإشعار الذي سيصلك 

      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(24).png)
   
   - قم باستكمال سير العمل من خلال تعديل تفاصيل الطلب مرة أخرى و إدخال معلومات المهمة الأولى

      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(25).png)
      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(26).png)
   
   - بعد حفظ الطلب، قم بالنقر فوق إجراء **تعيين مهمة**، هكذا أصبح سير العمل في مرحلة المهمة الأولى عند مسؤول التواصل
      
      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(27).png)


**11. المهمة الأولى:**

   - ستصل إلى بريد المترشح، رسالة بريد الكتروني  بتقاصيل المهمة و بريد مسؤول التواصل لإرسال الأجوبة و الاستفسارات.
   - بعد توصل مسؤول التواصل بالأجوبة، يدخلها إلى النظام و يقوم بتمرير سير العمل للمرحلة الموالية عن طريق النقر فوق إجراء **إعادة التقييم**
      
      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(28).png)
      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(29).png)

   - سيعود سير العمل إلى خطوة المقابلة L1، لنعتبر أن المترشح تم قبوله و لا يحتاج إلى مقابلة ثانية
   - عد إلى متصفح عضو تقنية المعلومات
   - قم بتعديل المدخل، و أدخل تقييم المترشح ثم احفظ التعديلات
      
      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(30).png)

   - قم بالضغط على زر الموافقة في قائمة الإجراءات، لتمرير سير العمل إلى مرحلة عرض العمل
      
      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(31).png)

**12. عرض العمل:**
   - عد إلى متصفح عضو الموارد البشرية، و ادخل الى الطلب من خلال صندوق الوارد (الشريط الجانبي > الخدمات > صندوق الوارد)
   - انقر فوق إجراء أخذ الملكية
   - قد بالدخول إلى وضع تعديل الطلب و أدخل عقد العمل في تبويبة عرض العمل ثم احفظ التعديلات
   - قم بالضغط على إجراء إرسال عرض العمل

      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(32).png)

   - سيتوصل المترشح برسالة بريد جديدة تحمل تفاصيل العرض و رابط للرد على العرض و بريد مسؤول التوظيف لإرسال الرد على عرض العمل، بعد توصل مسؤول التواصل بالرد يمكنه إدخال الملفات في النظام في تويبة "توقيع العقد"، ثم تمرير سير العمل

      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(33).png)
      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(34).png)

**13. إضافة الموظف**
   - سيتوصل مدير المنصة بإشعار لإضافة المستخدم
   - في متصفح آخر قم بالدخول إلى حساب **مدير المنصة**
   - قم بالضغط على الإشعار الذي وصلك، لرؤية معلومات الموظف الذي ستضيفه

      - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(35).png)

   - اذهب إلى قسم المسخدمين و قم لإضافة مستخدم جديد

     - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(36).png)
   
   - انتقل إلى قسم مجموعات المستخدمين و قم بإضافة المستخدم إلى مجموعة تقنية المعلومات

     - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(37).png)
     - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(38).png)
   - عد إلى الطلب و قم بإضافة اسم المستخدم داهل قسم إضافة المستخدم

     - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(39).png)

   - قم بإنهاء سير العمل

        - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(40).png)
        - ![job](../../../../../../static/img/tutorial/recruitment-system/testing-the-system(41).png)

## استقبال الموظف

- ادخل إلى حساب عضوة الموارد البشرية
- ستتوصل بإشعار لإضافة استقبال للموظف الجديد
- ادخل إلى واجهة إنشاء الاستقبالات في الرشيط الجانبي (التوظيف > إنشاء الاستقبالات)
- أنشئ اسنقبال جديد 
