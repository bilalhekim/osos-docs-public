---
title: "النص"
sidebar_position: 1
---

# حقل النص

بإضافة حقل النص إلى هيكل الكيان، يمكن للمستخدمين إدخال النص بسهولة داخل النموذج. حقل النص يسمح للمستخدمين بإدخال أي نص قصير، مثل الأسماء، العناوين، وأي معلومات أخرى تتطلب حقل نص بحجم صغير.

| الاسم            | الوصف                                                                      | نمط البيانات             |
|--------------|--------------------------------------------------------------------------|------------------------|
| نص  | حقل يسمح بإدخال نص قصير.                                                 | نص                     |

## الإعدادات المتقدمة

عند النقر على زر "الإعدادات" في حقل النص في هيكل الكيان، سيتم فتح نافذة جانبية للإعدادات المتقذمة لحقل النص، تظهر هاته النافذة عدة أقسام، و هي كالتالي :

### الإعدادات الأساسية

هذا القسم يحتوي على أربعة حقول:

1. **اسم الحقل:** هنا يجب تحديد اسم لحقل النص مع الترجمة باللغة العربية والإنجليزية.

2. **الاسم النموذجي:** يحتوي على الاسم النموذجي لحقل النص والذي يتم إنشاؤه تلقائيًا من الاسم باللغة الإنجليزية. يمكن تغيير هذا الاسم وهو يعمل كاسم فريد مثل الهوية  للحقل.

3. **الوصف:** اختياري ويمكن استخدامه لإضافة وصف لحقل النص.

4. **نوع البيانات:** هنا يظهر نمط البيانات الذي يتم تخزينه في حقل النص و هو في هاته الحالة: نص.

### القيمة الإفتراضية

هذا القسم يحتوي على الخواص التالية : 

#### القيمة الافتراضية 

يُمكن تعيين قيمة افتراضية لحقل النص عند إنشاء مدخل جديد. يتم تحديد القيمة الافتراضية من خلال ادخال النص في حقل القيمة الافتراضية أو بواسطة تعبير برمجي عبر تفعيل زر "متقدم" في إعدادات حقل النص. 

**كيفية الاستخدام: في حالة الرغبة في استعمال التعبير البرمجي:**

1. قم بفتح إعدادات حقل النص.
2. قم بتفعيل زر "متقدم".
3. أدخل التعبير البرمجي الذي يمثل القيمة الافتراضية التي ترغب في تعيينها.
4. (اختياري) يمكنك استخدام حقول إضافية:
   - **قفل الحقل:** يمكن استخدامه لمنع التغيير في القيمة الافتراضية بعد إنشاء المدخل. عند تفعيل هذا الخيار، سيظهر حقل اخر تابع للقيمة الافتراضية.
    - **قوادح:** يمكن استخدامها لتحديد متى يتم تطبيق التعبير البرمجي للقيمة الافتراضية، مثل عند تحميل الصفحة، إرسال النموذج، تغيير 
    مدخل أو عند تغيير الحقل.

#### قفل الحقل 

خاصية "قفل الحقل" تمنح المستخدم الحق في قفل حقل النص عند إنشاء مدخل جديد. إذا تم تفعيل هذا الخيار، يظهر حقل إدخال إضافي في نطاقه، يُسمح فيه للمستخدم بإدخال تعبير برمجي (اختياري) لإضافة شرط لقفل الحقل.

**كيفية الاستخدام:**

1. قم بفتح إعدادات حقل النص.
2. قم بتفعيل خاصية "قفل الحقل".
3. بعد التفعيل، سيظهر حقل إضافي. في هذا الحقل يمكن للمستخدم إدخال تعبير برمجي (اختياري) يحدد الشرط الذي يجب تحقيقه لقفل الحقل.
4. (اختياري) إذا تم تفعيل خيار "قفل الحقل"، يجب على المستخدم توفير قيمة افتراضية لحقل النص.

#### إخفاء الحقل 

يسمح للمستخدم بإخفاء حقل النص بناءً على تعبير محدد، مما يجعله غير مرئي للمستخدم عند تعامله مع النموذج.

**كيفية الاستخدام:**

1. قم بتفعيل خاصية "إخفاء الحقل" من خلال الانتقال إلى إعدادات حقل النص المراد إخفاؤه.
2. بعد تفعيلها، سيظهر حقل إضافي لإدخال التعبير البرمجي لتحديد شروط  إخفاء حقل النص.

**مثال بسيط:**

عند تفعيل حقل التحقق "الاشتراك"، سيتم إظهار حقل إدخال "عنوان الاشتراك" إضافي. وعند تعطيل هذا الزر، سيتم إخفائه تلقائيًا.

#### مطلوب 

يُحدد ما إذا كان حقل النص مطلوبًا لإكمال النموذج أو يمكن تركه فارغًا.

**كيفية الاستخدام:**

1. قم بتفعيل خاصية "مطلوب" من خلال الانتقال إلى إعدادات حقل النص المراد التحقق من إكماله.
2. بعد تفعيلها، سيظهر حقل إضافي لإدخال التعبير البرمجي لتحديد شروط جعل حقل النص مطلوبًا.

#### قابل للبحث 

خاصية "قابل للبحث" تسمح بتفعيل وظيفة البحث في حقل النص عند عرض المدخلات في واجهة المستخدم. عند تفعيل هذه الخاصية في الحقل، يمكن للمستخدمين البحث عن القيم في هذا الحقل باستخدام خانة البحث في واجهة عرض المدخلات.

**كيفية الاستخدام:**

   1. قم بتفعيل خاصية "قابل للبحث" في إعدادات حقل النص.
   2. بمجرد تفعيل الخاصية، سيتم تمكين وظيفة البحث في هذا الحقل.
   3. في الواجهات : عند النقر على زر البحث و إدخال الكلمة المراد البحث عنها في خانة البحث، يقوم النظام بالبحث في هذا الحقل أيضا.

**مثال بسيط:** 

 باستخدام خاصية "قابل للبحث" في حقل النص، يمكن للمستخدمين البحث بإدخال جزء من الاسم في خانة البحث. سيقوم النظام بعرض جميع اللتي تحتوي على الكلمة المدخلة في خانة البحث. سيقوم النظام بالبحث في جميع الحقول القابلة للبحث بما فيهم هذا الحقل.

#### فريد 

خاصية "فريد" تمنع تكرار القيم في حقل النص، مما يضمن أن كل قيمة مخزنة في هذا الحقل فريدة ولا تتكرر في مدخلات أخرى.

**كيفية الاستخدام:**

   1. قم بتفعيل خاصية "فريد" في إعدادات حقل النص الذي ترغب في جعله فريدًا.
   2. بعد تفعيل الخاصية، يضمن النظام أنه لا يمكن إدخال قيمة مكررة في هذا الحقل.
   3. عندما يحاول المستخدم إدخال قيمة موجودة بالفعل في حقل آخر، سيتم منعه وعرض رسالة تنبيه تشير إلى أن هذه القيمة مكررة ويجب استخدام قيمة فريدة.

**مثال بسيط:** 

في قاعدة بيانات لنظام إدارة الموظفين، قد يكون لدينا حقل اسم وظيفي لكل موظف. باستخدام خاصية "فريد" في هذا الحقل، سيضمن النظام أنه لا يمكن تكرار هذا الاسم.

### صيغة وشكل القيمة 

يتيح النظام إمكانية إعداد صيغة الحقل النصي لضمان التحقق من القيم المدخلة، يمكن تحديد صيغة الحقل النصي كالتالي:  
- **بدون صيغة**: يتم التعامل مع القيمة كأي نص عادي دون أي قيود أو تحقق خاص.  
- **رابط تشعبي**: يتحقق النظام من أن القيمة المدخلة تمثل رابطًا تشعبيًا صحيحًا.  
- **بريد إلكتروني**: يتحقق النظام من أن القيمة المدخلة تمثل عنوان بريد إلكتروني صحيحًا.
- 
اختيار الصيغة المناسبة يضمن توافق القيم مع متطلبات الاستخدام ويقلل من احتمالية حدوث الأخطاء.

#### إعداد صيغة النص كـ رابط تشعبي

1. انتقل إلى إعدادات بنية الكيان.  
2. قم بإضافة حقل جديد من النوع "نص".  
3. انتقل إلى إعدادات الحقل المتقدمة.  
4. اختر "رابط تشعبي" من قائمة صيغ النص المتاحة.  
5. احفظ الإعدادات.  

عند إدخال قيمة في هذا الحقل، يقوم النظام بالتحقق من أنها تمثل رابطًا تشعبيًا صحيحًا.  
إذا كانت القيمة غير صحيحة، سيعرض النظام رسالة تنبيه أسفل الحقل: **"القيمة غير صالحة"**.

#### إعداد صيغة النص كـ بريد إلكتروني

1. كرر الخطوات المذكورة أعلاه.  
2. اختر "بريد إلكتروني" من قائمة صيغ النص المتاحة.  
3. احفظ الإعدادات.  

عند إدخال قيمة في هذا الحقل، سيقوم النظام بالتحقق من كونها عنوان بريد إلكتروني صحيحًا.  
في حال كانت القيمة غير صحيحة، ستظهر رسالة تحت الحقل: **"القيمة غير صالحة"**.

### إعدادات قيمة الحقل

هذا القسم يحتوي على الخواص التالية : 

#### قابل للتكرار 

 خاصية "قابل للتكرار" تمثل إمكانية تكرار إدخال نفس الحقل بقيم مختلفة في نفس المدخل. عند تفعيل هذا الخيار، يمكن للمستخدمين إضافة قيم متعددة لنفس الحقل ضمن مدخل واحد.

**كيفية الاستخدام:**

1. انتقل إلى "إعدادات الحقل" ثم إلى "إعدادات قيمة الحقل" المراد جعله قابلًا للتكرار.
2. تفعيل خاصية "قابل للتكرار".

**تحديد الحد الأدنى والحد الأقصى للتكرار (اختياري):**

بعد تفعيل خاصية "قابل للتكرار"، سيظهر حقلين إضافيين يمكن استخدامهما لتحديد الحد الأدنى والحد الأقصى لعدد مرات التكرار المسموح بها.

**ملاحظة:** إذا لم يتم ملء حقول تحديد الحد الأدنى والحد الأقصى، فسيكون التكرار غير محدود، ويمكن للمستخدم إضافة قيم بشكل غير محدود لحقل النص.

#### إظهار في القائمة 

 خاصية تسمح بعرض قيمة حقل النص في قائمة المدخلات، بحيث يمكن للمستخدم رؤية قيمة الحقل بسهولة دون الحاجة لفتح كل المدخل على حدة.

**كيفية الاستخدام:**

1. في إعدادات حقل النص قم بفتح قسم "إعدادات قيمة الحقل " ثم قسم "العرض"، هكذا ستظهر لك الخواص الخاصة بالعرض.
2. قم بتفعيل خيار "إظهار في القائمة".

#### العنوان الاساسي 

خاصية العنوان الرئيسي تمكّنك من تحديد العنوان الرئيسي الذي سيتم استخدامه بشكل أساسي في الكيان. عند تعيين حقل النص كعنوان رئيسي، سيتم استخدامه كعنوان مرجعي للكيان في العديد من الأماكن..

#### العنوان الفرعي 

العنوان الفرعي هو خاصية تُسند لحقل العنوان في الكيان، وتُمكّنك من إضافة عنوان فرعي إضافي يُعرض بجانب العنوان الأساسي في الكيان..

#### العنوان الفرعي 2

العنوان الفرعي 2 هو خاصية تُسند لحقل العنوان في الكيان، وتُمكّنك من إضافة عنوان فرعي إضافي آخر يُعرض بجانب العنوان الأساسي والعنوان الفرعي في الكيان. يُمكن استخدام العنوان الفرعي 2 لتوضيح العنوان الأساسي والعنوان الفرعي أو لإضافة معلومات إضافية أخرى عن الكيان.
