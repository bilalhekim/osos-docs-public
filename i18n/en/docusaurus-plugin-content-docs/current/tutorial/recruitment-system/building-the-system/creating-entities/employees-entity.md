---
title: "كيان الموظفين"
sidebar_position: 1
--- 

# كيان الموظفين 
 هذا الكيان مخصص لحفظ وإدارة معلومات الموظفين داخل المنصة.

- **ملاحظة:** سنشير في هذا الملف إلى التفاصيل الخاصة بكيان الموظفين بشكل خاص، مثل المعلومات، البنية، سير العمل، والتفاعلات فقط، دون الإشارة إلى الخطوات وطريقة البناء. لذا يُرجى الرجوع إلى [وثيقة كيان الوظائف](./jobs-entity.md) للمزيد من المعلومات حول هذه التفاصيل.

## إنشاء كيان الموظفين

   - **اسم الكيان**: قم بإدخال اسم الكيان **الموظفون** وأدخل الترجمة بالإنجليزية.
   - **اختيار الرمز**: حدد رمزًا للكيان لتمثيله بصريًا.
   - **نوع الكيان**: حدد **كيان عادي**.
   - **في قسم الإعدادات المتقدمة**: قم بإدخال اسم الكيان بالمفرد والجمع.

   ![تفاصيل الكيان](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(1).png)

## البنية

1. **كتلة معلومات الموظف :**

    - **الاسم الكامل** : حقل إجباري من نوع **نص متعدد اللغات**.
    - **تاريخ الميلاد**: حقل اختياري من نوع **تاريخ**.
    - **البريد الاكتروني**: حقل إجباري من نوع **نص**.
    - **رقم الهاتف**: حقل إجباري من نوع **هاتف**.
    - **الجنسية**: حقل إجباري من نوع **ارتباط** بقائمة **الجنسية**.
    - **الإقامة**: حقل اختياري من نوع **ارتباط** بقائمة **الإقامة**.
    - **التعليم**: حقل اختياري من نوع ارتباط بقائمة **المؤهلات الدراسية**.

   ![كتلة معلومات الموظف](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(2).png)
   ![كتلة معلومات الموظف](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(14).png)

   - أدخل إلى إعدادات الكتلة و قم بتحديد شكل العرض كـ **عرض عمودين** و قم بتفعيل العرض كعلامة تبويب :

   ![كتلة معلومات الموظف](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(5).png)


2. **كتلة المعلومات التابعة للشركة :**

    - **البريد الاكتروني التابع للشركة**: حقل اختياري من نوع **نص**.
    - **الصورة التعريفية**: حقل اختياري من نوع **صورة**.
    - **العقد الموقع**: حقل اختياري من نوع **ملف**.
    - **جواز السفر/البطاقة**: حقل اختياري من نوع **ملف**.

   ![كتلة المعلومات التابعة للشركة](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(4).png)

   - أدخل إلى إعدادات الكتلة و قم بتحديد شكل العرض كـ **عرض عمودين** و قم بتفعيل العرض كعلامة تبويب :

   ![كتلة](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(5).png)

3. لا تنسى الضغط على زر **حفظ** أعلى الصفحة لحفظ هاته التعديلات.

## سير العمل

### الخطوة 1: البداية

- **الاسم**: البداية
- **الإجراءات**:
  - البدء (إلى الخطوة التالية)


### الخطوة 2: إدخال الصورة التعريفية

   - **الاسم**: إدخال الصورة التعريفية
   - **المالك**: الموظف الجديد
   - **الإجراءات**:
   - إنهاء (إلى الخطوة النهائية)

   ![الخطوة 3](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-receptions-entity-creating-entity(14).png)

   ![الخطوة 3](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-receptions-entity-creating-entity(15).png)

### الخطوة 3: النهاية

## التفاعلات

   1. **إشعار استقبال موظف جديد**
      - **الحدث**: عند إنشاء مدخل جديد
      - **الإجراء**: إرسال إشعار
      - **المستقبلون**: مجموعة الموارد البشرية

      ![صورة الإشعار](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(8).png)

   2. **بدء سير العمل**
      - **الحدث**: عند إنشاء مدخل جديد
      - **الإجراء**: نقل سير العمل
      - **الخطوة**: الخطوة 2

      ![صورة الإشعار](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(9).png)

   3. **إعلام باقي الفريق بانضمام الموظف الجديد**
      - **الحدث**: عند إنشاء مدخل جديد
      - **الإجراء**: إرسال إشعار
      - **المستقبلون**: مجموعة الموارد البشرية

      ![صورة الإشعار](../../../../../../../../static/img/tutorial/recruitment-system/recruitment-system-employees-entity-creating-entity(11).png)