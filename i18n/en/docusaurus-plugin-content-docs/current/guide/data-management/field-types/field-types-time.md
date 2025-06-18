---
title: "Time Field"
sidebar_position: 6
---

# Time Field

By adding a time field to the entity structure, users can easily select the time through a pop-up window displaying the current time or the previously set time. The window shows the time in the format "H : M : S : AM/PM" with ascending and descending arrows for time control.

| Name  | Description                   | Data Type |
|-------|-------------------------------|-----------|
| Time  | A field that allows selecting time in hour/minute format. | Time      |

## Advanced Settings

Clicking the "Settings" button in the "Time" field in the entity structure opens a sidebar with advanced settings for the time field. This sidebar contains several sections:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the time field with translations in both Arabic and English.

2. **Normlized Name:** Contains the Normlized Name for the time field, automatically generated from the English name. This name can be changed and serves as a unique identifier for the field.

3. **Description:** Optional, used to add a description for the time field.

4. **Data Type:** Shows the data type stored in the time field, which in this case is "Time."

### Default Value

This section contains the following properties:

#### Default Value

You can set a default value for the time field when creating a new entry. The default value can be specified by entering a time in the default value field or by using a script expression by enabling the "Advanced" option in the time field settings.

**How to use: If you want to use a script expression:**

1. Open the time field settings.
2. Enable the "Advanced" option.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** Can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field will appear for the default value.
   - **Triggers:** Can be used to specify when the script expression for the default value should be applied, such as on page load, form submission, entry change, or field change.

#### Lock Field

The "Lock Field" feature allows you to lock the time field when creating a new entry. If this option is enabled, an additional input field will appear, allowing you to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the time field settings.
2. Enable the "Lock Field" feature.
3. After enabling it, an additional field will appear. In this field, you can enter a script expression (optional) specifying the condition to be met to lock the time field.
4. (Optional) If the "Lock Field" option is enabled, you must provide a default value for the time field.

#### Hide Field

This allows you to hide the time field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by going to the time field settings you want to hide.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for hiding the time field.

**Simple Example:**

When the "Subscription" toggle is enabled, an additional "Subscription Time" field will be shown. When this toggle is disabled, the field will be hidden automatically.

#### Required

This determines whether the time field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by going to the time field settings you want to validate.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for making the time field required.

### Searchable

The "Searchable" feature allows you to enable the search function for the time field when displaying entries in the user interface. When this feature is enabled, users can search for values in this time field using the search bar in the entry display interface.

**How to use:**

1. Enable the "Searchable" feature in the time field settings.
2. Once enabled, the search function will be activated for this field.
3. In the interfaces: When clicking the search button and entering the desired keyword in the search bar, the system will search in this field as well.

### Unique

The "Unique" feature ensures that each value stored in this time field is unique and does not repeat in other entries.

**How to use:**

1. Enable the "Unique" feature in the time field settings.
2. After enabling it, the system ensures that no duplicate values can be entered in this field.
3. When a user tries to enter a value that already exists in another field, they will be prevented and shown a warning message indicating that the value is a duplicate and a unique value must be used.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the ability to repeatedly enter the same time field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Go to "Field Settings" then "Field Value Settings" for the field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Specify Minimum and Maximum Repetitions (Optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum repetition fields are not filled, repetition will be unlimited, and users can add values ​​to the time field without limits.

#### Show in List

This feature allows displaying the value of the time field in the entry list, enabling the user to see the field value easily without having to open each entry individually.

**How to use:**

1. In the time field settings, open the "Field Value Settings" section and then the "Display" section, this will show the display properties.
2. Enable the "Show in List" option.

#### Time Range

Description: The "Time Range" feature allows the user to specify a specific time range by selecting a start and end time within the same time field.

**How to use:**

1. Enable the "Time Range" feature in the time field settings.
2. When the user selects a time in this field, arrows will appear at the top of the time picker window to select the start and end time.
3. Using the "Time Range" feature enhances the user experience and simplifies the process of specifying the required time range.

**Example:**

In a project management system, there may be a field to specify the start and end time for a specific task. Using the "Time Range" feature in this field, the user can specify a specific time range based on the selected start and end times.