---
title: "التاريخ والوقت"
sidebar_position: 7
---

# حقل التاريخ و الوقت

بإضافة حقل التاريخ والوقت إلى هيكل الكيان، يصبح بإمكان المستخدمين تحديد التاريخ والوقت بسهولة داخل النموذج. يتيح حقل التاريخ والوقت للمستخدمين تحديد تاريخ ووقت محددين بناءً على متطلبات التطبيق أو النظام.

| الاسم            | الوصف                                                                      | نمط البيانات             |
|--------------|--------------------------------------------------------------------------|------------------------|
| تاريخ و وقت  | حقل يسمح باختيار تاريخ ووقت بتنسيق اليوم/الشهر/السنة والساعة/الدقيقة.   | تاريخ/وقت                |

## الإعدادات المتقدمة

عند النقر على زر "الإعدادات" في حقل "تاريخ و وقت" في هيكل الكيان، سيتم فتح نافذة جانبية للإعدادات المتقمة لحقل التاريخ و الوقت، تظهر هاته النافذة عدة أقسام، و هي كالتالي :

### الإعدادات الأساسية

هذا القسم يحتوي على أربعة حقول:

1. **اسم الحقل:** هنا يجب تحديد اسم لحقل التاريخ و الوقت مع الترجمة باللغة العربية والإنجليزية.

2. **الاسم النموذجي:** يحتوي على الاسم النموذجي لحقل التاريخ و الوقت والذي يتم إنشاؤه تلقائيًا من الاسم باللغة الإنجليزية. يمكن تغيير هذا الاسم وهو يعمل كاسم فريد مثل الهوية (ID) للحقل.

3. **الوصف:** اختياري ويمكن استخدامه لإضافة وصف لحقل التاريخ و الوقت.

4. **نوع البيانات:** هنا يظهر نمط البيانات الذي يتم تخزينه في الحقل و في هاته الحالة النمط هو: تاريخ و وقت.

### القيمة الإفتراضية

هذا القسم يحتوي على الخواص التالية : 

#### القيمة الافتراضية 

يُمكن تعيين قيمة افتراضية لحقل التاريخ و الوقت عند إنشاء مدخل جديد. يتم تحديد القيمة الافتراضية من خلال ادخال تاريخ و وقت في حقل القيمة الافتراضية أو بواسطة تعبير برمجي عبر تفعيل زر "متقدم" في إعدادات حقل التاريخ و الوقت. 

**كيفية الاستخدام: في حالة الرغبة في استعمال التعبير البرمجي:**

1. قم بفتح إعدادات حقل التاريخ و الوقت.
2. قم بتفعيل زر "متقدم".
3. أدخل التعبير البرمجي الذي يمثل القيمة الافتراضية التي ترغب في تعيينها.
4. (اختياري) يمكنك استخدام حقول إضافية:
   - **قفل الحقل:** يمكن استخدامه لمنع التغيير في القيمة الافتراضية بعد إنشاء المدخل. عند تفعيل هذا الخيار، سيظهر حقل اخر تابع للقيمة الافتراضية.
    - **قوادح (Triggers):** يمكن استخدامها لتحديد متى يتم تطبيق التعبير البرمجي للقيمة الافتراضية، مثل عند تحميل الصفحة، إرسال النموذج، تغيير 
    مدخل أو عند تغيير الحقل.

#### قفل الحقل 

خاصية "قفل الحقل" تمنح المستخدم الحق في قفل حقل التاريخ و الوقت عند إنشاء مدخل جديد. إذا تم تفعيل هذا الخيار، سيظهر حقل إدخال إضافي في نطاقه، يُسمح فيه للمستخدم بإدخال تعبير برمجي (اختياري) لإضافة شرط لقفل الحقل.

**كيفية الاستخدام:**

1. قم بفتح إعدادات حقل التاريخ و الوقت.
2. قم بتفعيل خاصية "قفل الحقل".
3. بعد التفعيل، سيظهر حقل إضافي، في هذا الحقل يمكن للمستخدم إدخال تعبير برمجي (اختياري) يحدد الشرط الذي يجب تحقيقه لقفل حقل التاريخ و الوقت.
4. (اختياري) إذا تم تفعيل خيار "قفل الحقل"، يجب على المستخدم توفير قيمة افتراضية لحقل التاريخ و الوقت.

#### إخفاء الحقل 
يسمح للمستخدم بإخفاء حقل التاريخ و الوقت بناءً على تعبير محدد، مما يجعله غير مرئي للمستخدم عند تعامله مع النموذج.

**كيفية الاستخدام:**

1. قم بتفعيل خاصية "إخفاء الحقل" من خلال الانتقال إلى إعدادات حقل التاريخ و الوقت المراد إخفاؤه.
2. بعد تفعيلها، سيظهر حقل إضافي لإدخال التعبير البرمجي لتحديد شروط  إخفاء حقل التاريخ و الوقت.

**مثال بسيط:**

عند تفعيل حقل التحقق "الاشتراك"، سيتم إظهار حقل إدخال "تاريخ و وقت الاشتراك" إضافي. وعند تعطيل هذا الزر، سيتم إخفائه تلقائيًا.

#### مطلوب 

يُحدد ما إذا كان حقل التاريخ و الوقت مطلوبًا لإكمال النموذج أو يمكن تركه فارغًا.

**كيفية الاستخدام:**

1. قم بتفعيل خاصية "مطلوب" من خلال الانتقال إلى إعدادات حقل التاريخ و الوقت المراد التحقق من إكماله.
2. بعد تفعيلها، سيظهر حقل إضافي لإدخال التعبير البرمجي لتحديد شروط جعل حقل التاريخ و الوقت مطلوبًا.

#### قابل للبحث 

خاصية "قابل للبحث" تسمح بتفعيل وظيفة البحث في حقل التاريخ و الوقت عند عرض المدخلات في واجهة المستخدم. عند تفعيل هذه الخاصية في الحقل، يمكن للمستخدمين البحث عن القيم في هذا الحقل باستخدام خانة البحث في واجهة عرض المدخلات.

**كيفية الاستخدام:**

   1. قم بتفعيل خاصية "قابل للبحث" في إعدادات حقل التاريخ و الوقت.
   2. بمجرد تفعيل الخاصية، سيتم تمكين وظيفة البحث في هذا الحقل.
   3. في الواجهات : عند النقر على زر البحث و إدخال الكلمة المراد البحث عنها في خانة البحث، يقوم النظام بالبحث في هذا الحقل أيضا.

#### فريد 

خاصية "فريد" تمنع تكرار القيم في حقل التاريخ و الوقت, مما يضمن أن كل قيمة مخزنة في هذا الحقل فريدة ولا تتكرر في مدخلات أخرى.

**كيفية الاستخدام:**

   1. قم بتفعيل خاصية "فريد" في إعدادات حقل التاريخ و الوقت الذي ترغب في جعله فريدًا.
   2. بعد تفعيل الخاصية، يضمن النظام أنه لا يمكن إدخال قيمة مكررة في هذا الحقل.
   3. عندما يحاول المستخدم إدخال قيمة موجودة بالفعل في حقل آخر، سيتم منعه وعرض رسالة تنبيه تشير إلى أن هذه القيمة مكررة ويجب استخدام قيمة فريدة.

### إعدادات قيمة الحقل

هذا القسم يحتوي على الخواص التالية : 

#### قابل للتكرار 

 خاصية "قابل للتكرار" تمثل إمكانية تكرار إدخال نفس حقل التاريخ و الوقت بقيم مختلفة في نفس المدخل. عند تفعيل هذا الخيار، يمكن للمستخدمين إضافة قيم متعددة لنفس الحقل ضمن مدخل واحد.

**كيفية الاستخدام:**

1. انتقل إلى "إعدادات حقل التاريخ و الوقت" ثم إلى "إعدادات قيمة الحقل" المراد جعله قابلًا للتكرار.
2. تفعيل خاصية "قابل للتكرار".

**تحديد الحد الأدنى والحد الأقصى للتكرار (اختياري):**

بعد تفعيل خاصية "قابل للتكرار"، سيظهر حقلين إضافيين يمكن استخدامهما لتحديد الحد الأدنى والحد الأقصى لعدد مرات التكرار المسموح بها.

**ملاحظة:** إذا لم يتم ملء حقول تحديد الحد الأدنى والحد الأقصى، فسيكون التكرار غير محدود، ويمكن للمستخدم إضافة قيم بشكل غير محدود لحقل التاريخ و الوقت.

#### مجال زمني 

وصف: خاصية "مجال زمني" تُمكّن المستخدم من تحديد نطاق زمني محدد من خلال اختيار تاريخ و وقت البداية وتاريخ و وقت النهاية في نفس حقل التاريخ و الوقت.

**كيفية الاستخدام:**

   1. قم بتفعيل خاصية "مجال زمني" في إعدادات حقل التاريخ و الوقت.
   2. عند اختيار المستخدم لتاريخ و وقت في هذا الحقل سيتظهر له أسهم أعلى نافذة التقويم الزمني لاختيار تاريخ و وقت البداية و التهاية.
   3. يتيح استخدام خاصية "مجال زمني" تحسين تجربة المستخدم وتسهيل عملية تحديد الفترة الزمنية المطلوبة.

**مثال :** 

   في نظام إدارة المشاريع، قد يكون لدينا حقل لتحديد تاريخ و وقت بداية وتاريخ و وقت نهاية مهمة معينة. باستخدام خاصية "مجال زمني" في حقل التاريخ و الوقت هذا، يمكن للمستخدم تحديد نطاق زمني محدد بناءً على تاريخ و وقت البداية والنهاية المختارين.

   
#### إظهار في القائمة 

 خاصية تسمح بعرض قيمة حقل التاريخ و الوقت في قائمة المدخلات، بحيث يمكن للمستخدم رؤية قيمة الحقل بسهولة دون الحاجة لفتح كل المدخل على حدة.

**كيفية الاستخدام:**

1. في إعدادات حقل التاريخ و الوقت قم بفتح قسم "إعدادات قيمة الحقل " ثم قسم "العرض"، هكذا ستظهر لك الخواص الخاصة بالعرض.
2. قم بتفعيل خيار "إظهار في القائمة".

