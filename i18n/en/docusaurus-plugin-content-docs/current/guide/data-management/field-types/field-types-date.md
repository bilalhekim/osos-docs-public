---
title: "Date"
sidebar_position: 5
---

# Date Field

By adding a date field to the entity structure, users can select dates with a single click on the field. A mini calendar window for the month, year, and day will appear. Users can easily select the appropriate date.

| Name       | Description                         | Data Type |
|------------|-------------------------------------|-----------|
| Date       | Field allows users to select a date | Date      |

## Advanced Settings

Clicking on the "Settings" button in the date field within the entity structure opens a side window for advanced settings. This window has several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the date field with translations in Arabic and English.
2. **Normlized Name:** Contains the Normlized Name for the date field, automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the field.
3. **Description:** An optional field for adding a description of the date field.
4. **Data Type:** Shows the data type stored in the date field, which in this case is **Date**.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the date field when creating a new entry. The default value is specified by entering a date in the default value field or via a script expression by enabling the "Advanced" button in the field settings.

**How to use: In case of using a script expression:**

1. Open the date field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) Additional fields can be used:
   - **Lock Field:** This can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field for the default value will appear.
   - **Triggers:** These can be used to specify when the script expression for the default value is applied, such as on page load, form submission, entry change, or field change.

#### Lock Field

The "Lock Field" feature allows the user to lock the date field when creating a new entry. If this option is enabled, an additional input field will appear, allowing the user to enter an optional script expression to lock the field.

**How to use:**

1. Open the date field settings.
2. Enable the "Lock Field" feature.
3. After enabling, an additional field will appear where the user can enter an optional script expression specifying the condition for locking the field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the field.

#### Hide Field

This feature allows the user to hide the date field based on a specified script expression, making it invisible when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature in the date field settings.
2. After enabling, an additional field will appear for entering the script expression to hide the date field.

**Simple Example:**

When enabling the "Subscription" checkbox, an additional "Subscription Date" field will be displayed. When disabling this checkbox, the field will be hidden automatically.

#### Required

This feature specifies whether the date field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature in the date field settings.
2. After enabling, an additional field will appear for entering the script expression to make the date field required.

#### Searchable

The "Searchable" feature allows enabling the search function in the date field when displaying entries in the user interface. By enabling this feature in the field, users can search for values in this field using the search box in the entry display interface.

**How to use:**

1. Enable the "Searchable" feature in the date field settings.
2. Once the feature is enabled, the search function will be enabled for this date field.
3. In the interfaces: when clicking on the search button and entering the desired search term in the search box, the system will search in this field as well.

#### Unique

The "Unique" feature prevents duplicate values in the date field, ensuring that each value stored in this field is unique and does not repeat in other entries.

**How to use:**

1. Enable the "Unique" feature in the date field settings.
2. After enabling, the system ensures that no duplicate value can be entered in this field.
3. When the user tries to enter a value that already exists in another date field, they will be prevented and shown an alert indicating that the value is duplicate and must use a unique value.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" property represents the ability to repeat the same date field with different values in the same entry. Enabling this option allows users to add multiple values to the same field within a single entry.

**How to use:**

1. Go to the "Date Field Settings" then to the "Field Value Settings" section for the date field you want to make repeatable.
2. Enable the "Repeatable" property.

**Setting Minimum and Maximum Limits (Optional):**

After enabling the "Repeatable" property, two additional fields will appear where you can specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum fields are left empty, repetitions will be unlimited, allowing the user to add values to the date field without restriction.

#### Show in List

This property allows the date field value to be displayed in the list of entries, enabling the user to see the field value without opening each entry individually.

**How to use:**

1. In the date field settings, open the "Field Value Settings" section.
2. Open the "Display" section.
3. Enable the "Show in List" option.

#### Date Range

The "Date Range" feature allows the user to specify a defined time range by selecting the start date and end date in the same field.

**How to use:**

1. Enable the "Date Range" feature in the date field settings.
2. Select two dates, ensuring that the first selected date is smaller than the second.
3. The "Date Range" feature improves user experience and makes it easier to specify the required time period.

**Example:**

In a project management system, there may be a field to specify the start date and end date of a particular task. Using the "Date Range" feature in this field, the user can specify a defined time range based on the selected start and end dates.

#### Main Date

The main date is a feature assigned to the date field in the entity, allowing you to specify the primary date relied upon in the entity.