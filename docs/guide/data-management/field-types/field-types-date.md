---
title: "التاريخ"
sidebar_position: 5
---
# حقل التاريخ
- بإضافة حقل التاريخ (Date Field) إلى هيكل الكيان (Entity Structure)، يصبح بإمكان المستخدمين اختيار التواريخ بنقرة واحدة فقط على الحقل. ستظهر نافذة تقويم مصغرة للشهر و السنة و اليوم. يمكن للمستخدم بسهولة اختيار التاريخ المناسب.



| الاسم            | الوصف                                                                      | نمط البيانات             |
|--------------|--------------------------------------------------------------------------|------------------------|
| التاريخ  | حقل يسمح للمستخدم بتحديد تاريخ معين.                                              | تاريخ                  |

## الإعدادات المتقدمة

عند النقر على زر "الإعدادات" في حقل التاريخ في هيكل الكيان، سيتم فتح نافذة جانبية للإعدادات المتقدمة لحقل التاريخ، تظهر هاته النافذة عدة أقسام، و هي كالتالي :

### الإعدادات الأساسية

هذا القسم يحتوي على أربعة حقول:

1. **اسم الحقل:** هنا يجب تحديد اسم لحقل التاريخ مع الترجمة باللغة العربية والإنجليزية.
2. **الاسم النموذجي:** يحتوي على الاسم النموذجي لحقل التاريخ والذي يتم إنشاؤه تلقائيًا من الاسم باللغة الإنجليزية. يمكن تغيير هذا الاسم وهو يعمل كاسم فريد مثل الهوية (ID) لحقل التاريخ.
3. **الوصف:** اختياري ويمكن استخدامه لإضافة وصف لحقل التاريخ.
4. **نوع الحقل:** هنا يظهر نمط البيانات الذي يتم تخزينه في حقل التاريخ و هو **تاريخ**.

### القيمة الإفتراضية

هذا القسم يحتوي على الخواص التالية :

#### القيمة الافتراضية 

يُمكن تعيين قيمة افتراضية لحقل التاريخ عند إنشاء مدخل جديد. يتم تحديد القيمة الافتراضية من خلال إدخال تاريخ في حقل القيمة الافتراضية أو بواسطة تعبير برمجي عبر تفعيل زر "متقدم" في إعدادات الحقل.

**كيفية الاستخدام: في حالة الرغبة في استعمال التعبير البرمجي:**

1. قم بفتح إعدادات حقل التاريخ.
2. قم بتفعيل زر "متقدم".
3. أدخل التعبير البرمجي الذي يمثل القيمة الافتراضية التي ترغب في تعيينها.
4. (اختياري) يمكنك استخدام حقول إضافية:
   - **قفل الحقل:** يمكن استخدامه لمنع التغيير في القيمة الافتراضية بعد إنشاء المدخل. عند تفعيل هذا الخيار، سيظهر حقل آخر تابع للقيمة الافتراضية:
    - **قوادح:** يمكن استخدامها لتحديد متى يتم تطبيق التعبير البرمجي للقيمة الافتراضية، مثل عند تحميل الصفحة; إرسال النموذج; تغيير
    مدخل أو عند تغيير الحقل.

#### قفل الحقل 

خاصية "قفل الحقل" تمنح المستخدم الحق في قفل حقل التاريخ عند إنشاء مدخل جديد. إذا تم تفعيل هذا الخيار، يظهر حقل إدخال إضافي في نطاقه، يُسمح فيه للمستخدم بإدخال تعبير برمجي (اختياري) لإضافة شرط لقفل الحقل.

**كيفية الاستخدام:**

1. قم بفتح إعدادات حقل التاريخ.
2. قم بتفعيل خاصية **"قفل الحقل"**.
3. بعد التفعيل، سيظهر حقل إضافي. في هذا الحقل يمكن للمستخدم إدخال تعبير برمجي (اختياري) يحدد الشرط الذي يجب تحقيقه لقفل الحقل.
4. (اختياري) إذا تم تفعيل خيار **"قفل الحقل"**، يجب على المستخدم توفير قيمة افتراضية للحقل.

#### إخفاء الحقل 

يسمح للمستخدم بإخفاء حقل التاريخ بناءً على تعبير محدد، مما يجعله غير مرئي للمستخدم عند تعامله مع النموذج.

**كيفية الاستخدام:**

1. قم بتفعيل خاصية **"إخفاء الحقل"** من خلال الانتقال إلى إعدادات حقل التاريخ المراد إخفاؤه.
2. بعد تفعيلها، سيظهر حقل إضافي لإدخال التعبير البرمجي لتحديد شروط  إخفاء الحقل.

**مثال بسيط:**

عند تفعيل حقل التحقق "الاشتراك"، سيتم إظهار حقل إدخال "تاريخ الاشتراك" إضافي. وعند تعطيل هذا الزر، سيتم إخفائه تلقائيًا.

#### مطلوب 

يُحدد ما إذا كان حقل التاريخ مطلوبًا لإكمال النموذج أو يمكن تركه فارغًا.

**كيفية الاستخدام:**

1. قم بتفعيل خاصية "مطلوب" من خلال الانتقال إلى إعدادات الحقل المراد التحقق من إكماله.
2. بعد تفعيلها، سيظهر حقل إضافي لإدخال التعبير البرمجي لتحديد شروط جعل الحقل مطلوبًا.

#### قابل للبحث 

خاصية "قابل للبحث" تسمح بتفعيل وظيفة البحث في حقل التاريخ عند عرض المدخلات في واجهة المستخدم. عند تفعيل هذه الخاصية في الحقل، يمكن للمستخدمين البحث عن القيم في هذا الحقل باستخدام خانة البحث في واجهة عرض المدخلات.

**كيفية الاستخدام:**

   1. قم بتفعيل خاصية "قابل للبحث" في إعدادات حقل التاريخ.
   2. بمجرد تفعيل الخاصية، سيتم تمكين وظيفة البحث في هذا الحقل.
   3. في الواجهات : عند النقر على زر البحث و إدخال الكلمة المراد البحث عنها في خانة البحث، يقوم النظام بالبحث في هذا الحقل أيضا.

#### فريد 

خاصية "فريد" تمنع تكرار القيم في حقل التاريخ, مما يضمن أن كل قيمة مخزنة في هذا الحقل فريدة ولا تتكرر في مدخلات أخرى.

**كيفية الاستخدام:**

   1. قم بتفعيل خاصية "فريد" في إعدادات الحقل الذي ترغب في جعله فريدًا.
   2. بعد تفعيل الخاصية، يضمن النظام أنه لا يمكن إدخال قيمة مكررة في هذا الحقل.
   3. عندما يحاول المستخدم إدخال قيمة موجودة بالفعل في حقل تاريخ آخر، سيتم منعه وعرض رسالة تنبيه تشير إلى أن هذه القيمة مكررة ويجب استخدام قيمة فريدة.

### إعدادات قيمة الحقل

هذا القسم يحتوي على الخواص التالية :

#### قابل للتكرار 

 خاصية "قابل للتكرار" تمثل إمكانية تكرار إدخال نفس حقل التاريخ بقيم مختلفة في نفس المدخل. عند تفعيل هذا الخيار، يمكن للمستخدمين إضافة قيم متعددة لنفس الحقل ضمن مدخل واحد.

**كيفية الاستخدام:**

1. انتقل إلى إعدادات حقل التاريخ ثم إلى "إعدادات قيمة الحقل" المراد جعله قابلًا للتكرار.
2. قم تفعيل خاصية "قابل للتكرار".

**تحديد الحد الأدنى والحد الأقصى للتكرار (اختياري):**

بعد تفعيل خاصية "قابل للتكرار"، سيظهر حقلين إضافيين يمكن استخدامهما لتحديد الحد الأدنى والحد الأقصى لعدد مرات التكرار المسموح بها.

**ملاحظة:** إذا لم يتم ملء حقول تحديد الحد الأدنى والحد الأقصى، فسيكون التكرار غير محدود، ويمكن للمستخدم إضافة قيم بشكل غير محدود للحقل.

#### إظهار في القائمة 

 خاصية تسمح بعرض قيمة حقل التاريخ في قائمة المدخلات، بحيث يمكن للمستخدم رؤية قيمة الحقل بسهولة دون الحاجة لفتح كل مدخل على حدة.

**كيفية الاستخدام:**

1. في إعدادات حقل التاريخ قم بفتح قسم "إعدادات قيمة الحقل " ثم قسم "العرض"، هكذا ستظهر لك الخواص الخاصة بالعرض.
2. قم بتفعيل خيار "إظهار في القائمة".

#### مجال زمني 

خاصية "مجال زمني" تُمكّن المستخدم من تحديد نطاق زمني محدد من خلال اختيار تاريخ البداية وتاريخ النهاية في نفس الحقل.

**كيفية الاستخدام:**

   1. قم بتفعيل خاصية "مجال زمني" في إعدادات حقل التاريخ.
   2. قم باختبار تاريخين, بشرط أن تكون القيمة الأولى التي اخترتها أصغر من الثانية.
   3. يتيح استخدام خاصية "مجال زمني" تحسين تجربة المستخدم وتسهيل عملية تحديد الفترة الزمنية المطلوبة.

**مثال :**

   في نظام إدارة المشاريع، قد يكون لدينا حقل لتحديد تاريخ بداية وتاريخ نهاية مهمة معينة. باستخدام خاصية "مجال زمني" في هذا الحقل، يمكن للمستخدم تحديد نطاق زمني محدد بناءً على تاريخ البداية والنهاية المختارين.

#### التاريخ الرئيسي 

التاريخ الرئيسي هو خاصية تُسند لحقل التاريخ في الكيان، وتُمكّنك من تحديد التاريخ الرئيسي الذي يُعتمد عليه بشكل أساسي في الكيان.
