---
title: "Date and Time"
sidebar_position: 7
---

# Date and Time Field

By adding the Date and Time field to the entity structure, users can easily select dates and times within the form. The Date and Time field allows users to specify a precise date and time based on the application's or system's requirements.

| Name         | Description                                                             | Data Type  |
|--------------|--------------------------------------------------------------------------|------------|
| Date and Time | A field that allows selecting a date and time in the format day/month/year and hour/minute | Date/Time  |

## Advanced Settings

When clicking the "Settings" button on the Date and Time field in the entity structure, a side window for advanced settings will open, displaying several sections as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you must specify a name for the Date and Time field with translations in both Arabic and English.
2. **Normlized Name:** This includes the Normlized Name of the Date and Time field, which is automatically generated from the name in English. This name can be changed and acts as a unique identifier (ID) for the field.
3. **Description:** Optional. This can be used to add a description for the Date and Time field.
4. **Data Type:** Here, the data type stored in the field is displayed, which in this case is Date and Time.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the Date and Time field when creating a new entry. The default value is specified by entering a date and time in the default value field or through a script by enabling the "Advanced" button in the field settings.

**How to use: in case you want to use a script:**

1. Open the Date and Time field settings.
2. Enable the "Advanced" button.
3. Enter the script representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after the entry is created. When this option is enabled, another field related to the default value will appear.
   - **Triggers:** These can be used to specify when the script for the default value should be applied, such as when loading the page, submitting the form, changing the entry, or changing the field.

#### Lock Field

The "Lock Field" feature allows users to lock the Date and Time field when creating a new entry. If this option is enabled, an additional input field will appear, allowing the user to enter an optional script to add a condition for locking the field.

**How to use:**

1. Open the Date and Time field settings.
2. Enable the "Lock Field" feature.
3. After enabling, an additional field will appear. In this field, the user can enter an optional script to specify the condition that must be met to lock the Date and Time field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the Date and Time field.

#### Hide Field

The "Hide Field" feature allows users to hide the Date and Time field based on a specific condition, making it invisible when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by navigating to the Date and Time field settings you want to hide.
2. After enabling it, an additional field will appear for entering the script that specifies the conditions for hiding the Date and Time field.

**Simple Example:**

When enabling the "Subscription" checkbox, an additional "Subscription Date and Time" field will be shown. When disabling this checkbox, the "Subscription Date and Time" field will be hidden automatically.

#### Required

This specifies whether the Date and Time field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by navigating to the Date and Time field settings you want to validate.
2. After enabling it, an additional field will appear for entering the script that specifies the conditions for making the Date and Time field required.

#### Searchable

The "Searchable" feature allows users to enable the search function for the Date and Time field when displaying entries in the user interface. When this feature is enabled, users can search for values in this field using the search box in the entry display interface.

**How to use:**

1. Enable the "Searchable" feature in the Date and Time field settings.
2. Once enabled, the search function in this field will be activated.
3. In the interfaces: When clicking the search button and entering the keyword in the search box, the system will search in this field as well.

#### Unique

The "Unique" feature prevents duplicate values in the Date and Time field, ensuring that each value stored in this field is unique and not repeated in other entries.

**How to use:**

1. Enable the "Unique" feature in the Date and Time field settings.
2. After enabling, the system ensures that no duplicate value can be entered in this field.
3. When a user attempts to enter a value that already exists in another Date and Time field, they will be prevented from doing so and a warning message will appear indicating that this value is duplicated and a unique value must be used.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the ability to enter the same Date and Time field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Navigate to the "Date and Time" field settings, then to the "Field Value Settings" section of the field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Specify Minimum and Maximum Repetition (Optional):**

After enabling the "Repeatable" feature, two additional fields will appear, which can be used to specify the minimum and maximum number of repetitions allowed.

**Note:** If the minimum and maximum fields are not filled in, repetition will be unlimited, and users can add values to the Date and Time field indefinitely.

#### Date Range

Description: The "Date Range" feature allows users to specify a specific date range by selecting a start date and time and an end date and time in the same Date and Time field.

**How to use:**

1. Enable the "Date Range" feature in the Date and Time field settings.
2. When the user selects a date and time in this field, arrows will appear at the top of the calendar window to select the start and end date and time.
3. Using the "Date Range" feature improves the user experience and facilitates the process of specifying the required time period.

**Example:**

In a project management system, there may be a field for specifying the start and end date and time of a specific task. Using the "Date Range" feature in this Date and Time field, the user can specify a specific time range based on the selected start and end date and time.

#### Show in List

This feature allows displaying the value of the Date and Time field in the entry list, so the user can easily see the field value without opening each entry individually.

**How to use:**

1. In the Date and Time field settings, open the "Field Value Settings" section, then the "Display" section. This will show the display-related features.
2. Enable the "Show in List" option.