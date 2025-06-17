---
title: "File Field"
sidebar_position: 15
---

# File Field

By adding a file field to the entity structure, users can upload and attach files of various types to the form. The file field allows users to select the file they want to upload by browsing their local disks or the files stored on their devices.

| Name   | Description                             | Data Type |
|--------|-----------------------------------------|-----------|
| File   | Field allows users to upload files.     | Blob      |

## Advanced Settings

Clicking on the "Settings" button in the file field within the entity structure opens a side window for advanced settings. This window has several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the file field with translations in Arabic and English.
2. **Normlized Name:** Contains the Normlized Name for the file field, automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the field.
3. **Description:** An optional field for adding a description of the file field.
4. **Data Type:** Shows the data type stored in the file field, which in this case is Blob.

### Lock Field

The lock field feature allows the user to lock the file field when creating a new entry. If this option is enabled, an additional input field will appear, allowing the user to enter an optional script expression to lock the field.

**Usage:**

1. Open the file field settings.
2. Enable the lock field option.
3. After enabling, an additional field will appear where the user can enter an optional script expression specifying the condition for locking the field.

### Hide Field

This feature allows the user to hide the file field based on a specified script expression, making it invisible when interacting with the form.

**Usage:**

1. Enable the hide field option in the file field settings.
2. After enabling, an additional field will appear for entering the script expression to hide the file field.

**Simple Example:**

When enabling the "Subscription" checkbox, an additional "Subscription File" field will be displayed. When disabling this checkbox, the field will be hidden automatically.

### Required

This feature specifies whether the file field is required to complete the form or can be left empty.

**Usage:**

1. Enable the required option in the file field settings.
2. After enabling, an additional field will appear for entering the script expression to make the file field required.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" property represents the ability to repeat the same file field with different values in the same entry. Enabling this option allows users to add multiple values to the same field within a single entry.

**Usage:**

1. Go to the "File Field Settings" then to the "Field Value Settings" section for the file field you want to make repeatable.
2. Enable the "Repeatable" property.

**Setting Minimum and Maximum Limits (Optional):**

After enabling the "Repeatable" property, two additional fields will appear where you can specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum fields are left empty, repetitions will be unlimited, allowing the user to add values to the file field without restriction.

#### Show in List

This property allows the file field value to be displayed in the list of entries, enabling the user to see the field value without opening each entry individually.

**Usage:**

1. In the file field settings, open the "Field Value Settings" section.
2. Open the "Display" section.
3. Enable the "Show in List" option.