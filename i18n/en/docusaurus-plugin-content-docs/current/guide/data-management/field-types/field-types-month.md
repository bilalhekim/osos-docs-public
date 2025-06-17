---
title: "Month Field"
sidebar_position: 10
---

# Month Field

By adding a month field to the entity structure, users can easily select a month within the form. The month field allows users to accurately choose the desired month in the appropriate temporal context.

| Name        | Description                                | Data Type |
|-------------|--------------------------------------------|-----------|
| Month       | A field that allows selecting a month.     | Month     |

## Advanced Settings

Clicking on the "Settings" button in the month field within the entity structure will open a side window for advanced settings of the month field. This window displays several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you should specify a name for the month field with translations in Arabic and English.
2. **Normlized Name:** This contains the Normlized Name for the month field, which is automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the month field.
3. **Description:** Optional, can be used to add a description for the month field.
4. **Data Type:** This shows the data type stored in the month field, which in this case is: Month.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the month field when creating a new entry. The default value is specified by entering a month in the default value field or using a script expression by enabling the "Advanced" button in the month field settings.

**How to use: in case of using a script expression:**

1. Open the month field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field related to the default value will appear.
   - **Triggers:** These can be used to specify when the script expression for the default value is applied, such as when the page loads, the form is submitted, the entry is changed, or the field is changed.

#### Lock Field

The "Lock Field" feature allows the user to lock the month field when creating a new entry. If this option is enabled, an additional input field appears in its scope, allowing the user to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the month field settings.
2. Enable the "Lock Field" feature.
3. After enabling, an additional field will appear. In this field, the user can enter a script expression (optional) to define the condition that must be met to lock the month field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the month field.

#### Hide Field

Allows the user to hide the month field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by navigating to the month field settings that you want to hide.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for hiding the month field.

**Simple Example:**

When the "Subscription" toggle field is enabled, an additional "Subscription Month" month field will be shown. When this toggle is disabled, it will be automatically hidden.

#### Required

Specifies whether the month field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by navigating to the month field settings that need to be completed.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for making the month field required.

#### Searchable

The "Searchable" feature allows enabling the search function within the month field when displaying entries in the user interface. When this feature is activated, users can search for values in this field using the search box in the entries display interface.

**How to use:**

1. Enable the "Searchable" feature in the month field settings.
2. Once the feature is activated, the search function in this month field will be enabled.
3. In the interfaces: When clicking the search button and entering the word to search for in the search box, the system will search in this month field as well.

#### Unique

The "Unique" feature prevents duplicate values in the month field, ensuring that each value stored in this field is unique and does not repeat in other entries.

**How to use:**

1. Enable the "Unique" feature in the month field settings you want to make unique.
2. After enabling the feature, the system ensures that a duplicate value cannot be entered in this field.
3. When the user tries to enter a value that already exists in another field, they will be prevented, and a warning message will be displayed indicating that this value is a duplicate and a unique value must be used.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the possibility of repeating the same month field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Navigate to "Month Field Settings" and then to "Field Value Settings" for the month field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Set the minimum and maximum repetitions (optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to set the minimum and maximum number of repetitions allowed.

**Note:** If the fields for setting the minimum and maximum values are not filled, the repetition will be unlimited, allowing users to add values to the month field indefinitely.

#### Date Range

Description: The "Date Range" feature allows the user to specify a specific range by selecting the start month and end month within the same month field.

**How to use:**

1. Enable the "Date Range" feature in the month field settings.
2. When the user selects a month in this field, arrows will appear at the top of the date picker to select the start and end months.
3. Using the "Date Range" feature improves the user experience and simplifies specifying the required date range.

#### Show in List

This feature allows the month field value to be displayed in the list of entries, enabling users to see the field value without opening each entry individually.

**How to use:**

1. In the month field settings, open the "Field Value Settings" section and then the "Display" section. This will show the display-related features.
2. Enable the "Show in List" option.

#### Main Date

The main date is a feature assigned to the date field in the entity, allowing you to set the primary date to be used as the main reference for the entity.