---
title: "Block Field"
sidebar_position: 11
---

# Block Field

Adding a block field to the entity structure allows users to build content consisting of multiple sub-fields.

| Name  | Description                                      | Data Type |
|-------|--------------------------------------------------|-----------|
| Block | A field that allows creating content with multiple sub-fields. | Block     |

## Advanced Settings

When clicking the settings icon on the block field in the entity structure, a side window for advanced settings will open, displaying several sections as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you must specify a name for the block field with translations in both Arabic and English.
2. **Normlized Name:** This includes the Normlized Name of the block field, which is automatically generated from the name in English. This name can be changed and acts as a unique identifier (ID) for the block field.
3. **Description:** Optional. This can be used to add a description for the block field.
4. **Data Type:** Here, the data type represented by the block is displayed.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" property represents the ability to repeat the same block with different values within the same entry. When this option is enabled, users can add multiple blocks of the same type within one entry.

**How to use:**

1. Navigate to "Field Settings" and then to "Field Value Settings."
2. Enable the "Repeatable" property.

**Specify Minimum and Maximum Repetition (Optional):**

After enabling the "Repeatable" property, two additional fields will appear, allowing you to specify the minimum and maximum number of repetitions allowed.

**Note:** If the minimum and maximum fields are not filled in, repetition will be unlimited, and users can add unlimited values to the block field.

**Simple Example:**

When creating a new project, the user can add more than one employee for the same time period, with each employee having their own name and ID number. By using the "Repeatable" property in the worker field, the user can easily add more than one worker without needing to create an entry for each worker.

#### Display Format

The "Display Format" option allows users to choose how the internal fields of the block are displayed in the user interface.

**How to use:**

1. Go to the block field settings, then the "Field Value Settings" section, and look for the "Display Format" option.
2. You can choose one of the available options for displaying the block field:
   - **Key/Value:** Displays the block field in a "key/value" format, where the field name (key) is displayed alongside its value.
   - **Two Columns:** Displays the block field in a two-column layout, where two fields are displayed per row.
   - **Three Columns:** Displays the block field in a three-column layout, where three fields are displayed per row.
   - **Four Columns:** Displays the block field in a four-column layout, where four fields are displayed per row.

**Simple Example:**

In an inventory management system, a "Product Details" block field containing the product name, description, price, and available quantity is defined. By choosing the "Three Columns" display format, the product name will be displayed in the first column, the description in the second column, and the price in the third column, making it easy for the user to see product information in an organized and suitable manner. This option is available only for block fields containing internal fields.

### Display

This section contains properties related to the display of the field:

#### Display as Tab

The "Display as Tab" property allows users to group the internal fields of the block into a separate tab, helping to organize and categorize the content in an orderly manner.

**How to use:**

1. Go to the block field settings and enable the "Display as Tab" property to allow displaying the fields within a separate tab.

**Simple Example:**

In a project management application, a "Task Information" block field containing the main task details is defined. Using the "Display as Tab" property, the fields of this block can be displayed in a separate tab from the other fields.