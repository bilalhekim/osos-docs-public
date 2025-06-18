---
title: "Video"
sidebar_position: 25
---

# Video Field

By adding a video field to the entity structure, users can easily add a video file to the form. This allows users to upload the desired video file to share visual content.

| Name       | Description                   | Data Type |
|------------|-------------------------------|-----------|
| Video      | A field that allows video upload. | Blob      |

## Advanced Settings

When you click the "Settings" button for the video field in the entity structure, a sidebar with advanced settings for the video field will open. This sidebar contains several sections:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you must specify a name for the video field with translations in both Arabic and English.

2. **Normlized Name:** This contains the Normlized NameName for the video field, which is automatically generated from the name in English. This name can be changed and serves as a unique identifier for the field.

3. **Description:** Optional, and can be used to add a description for the video field.

4. **Data Type:** This shows the data type stored in the video field, which in this case is a blob.

### Lock Field

The "Lock Field" feature allows the user to lock the video field when creating a new entry. If this option is enabled, an additional input field appears in its scope, where the user can enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the video field settings.
2. Enable the "Lock Field" feature.
3. After enabling it, an additional field will appear. In this field, the user can enter a script expression (optional) that specifies the condition to be met to lock the video field.

### Hide Field

This allows the user to hide the video field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by going to the settings of the video field you want to hide.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for hiding the video field.

### Required

This determines whether the video field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by going to the settings of the video field you want to validate.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for making the video field required.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the ability to repeatedly enter the same video field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Go to "Field Settings" then "Field Value Settings" for the field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Specify Minimum and Maximum Repetitions (Optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum repetition fields are not filled, repetition will be unlimited, and users can add values ​​to the video field without limits.

#### Show in List

This feature allows displaying the value of the video field in the entry list, enabling the user to see the field value easily without having to open each entry individually.

**How to use:**

1. In the video field settings, open the "Field Value Settings" section and then the "Display" section, this will show the display properties.
2. Enable the "Show in List" option.