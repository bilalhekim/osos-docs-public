---
title: "Image Field"
sidebar_position: 17
---

# Image Field

By adding an image field to the entity structure, users can easily upload and attach images to the form. The image field allows users to select the image they want to upload from their local disks or device storage.

| Name       | Description                              | Data Type |
|------------|------------------------------------------|-----------|
| Image      | Field allows uploading images.           | Blob      |

## Advanced Settings

Clicking on the "Settings" button in the image field within the entity structure opens a side window for advanced settings. This window has several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the image field with translations in Arabic and English.
2. **Normlized Name:** Contains the Normlized Name for the image field, automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the field.
3. **Description:** An optional field for adding a description of the image field.
4. **Data Type:** Shows the data type stored in the image field, which in this case is Blob.

### Lock Field

The lock field feature allows the user to lock the image field when creating a new entry. If this option is enabled, an additional input field will appear, allowing the user to enter an optional script expression to lock the field.

**Usage:**

1. Open the image field settings.
2. Enable the lock field option.
3. After enabling, an additional field will appear where the user can enter an optional script expression specifying the condition for locking the field.

### Hide Field

This feature allows the user to hide the image field based on a specified script expression, making it invisible when interacting with the form.

**Usage:**

1. Enable the hide field option in the image field settings.
2. After enabling, an additional field will appear for entering the script expression to hide the image field.

### Required

This feature specifies whether the image field is required to complete the form or can be left empty.

**Usage:**

1. Enable the required option in the image field settings.
2. After enabling, an additional field will appear for entering the script expression to make the image field required.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" property represents the ability to repeat the same image field with different values in the same entry. Enabling this option allows users to add multiple values to the same field within a single entry.

**Usage:**

1. Go to the "Image Field Settings" then to the "Field Value Settings" section for the image field you want to make repeatable.
2. Enable the "Repeatable" property.

**Setting Minimum and Maximum Limits (Optional):**

After enabling the "Repeatable" property, two additional fields will appear where you can specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum fields are left empty, repetitions will be unlimited, allowing the user to add values to the image field without restriction.

#### Show in List

This property allows the image field value to be displayed in the list of entries, enabling the user to see the field value without opening each entry individually.

**Usage:**

1. In the image field settings, open the "Field Value Settings" section.
2. Open the "Display" section.
3. Enable the "Show in List" option.

#### Main Image "Use as Entry Image"

The main image property allows you to specify the main image that will be primarily used for the entity. When setting the image field as the main image, it will be used as the reference image for the entity in various locations.