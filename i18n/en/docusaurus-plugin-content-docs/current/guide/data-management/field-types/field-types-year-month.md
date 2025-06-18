---
title: "Month and Year"
sidebar_position: 8
---

# Month and Year Field

Adding a month and year field to the entity structure allows users to easily specify a particular month within a year in the form. The month and year field enables the precise determination of dates for events occurring in specific months within the year.

| Name       | Description                           | Data Type |
|------------|---------------------------------------|-----------|
| Year-Month | A field that allows selecting a year and month. | Date      |

## Advanced Settings

When you click on the "Settings" button for the "Month and Year" field in the entity structure, a sidebar with advanced settings for the month and year field will open. This sidebar contains several sections:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you must specify a name for the month and year field with translations in both Arabic and English.

2. **Normlized Name:** This contains the Normlized Name for the month and year field, which is automatically generated from the name in English. This name can be changed and serves as a unique identifier for the field.

3. **Description:** Optional, and can be used to add a description for the month and year field.

4. **Data Type:** This shows the data type stored in the month and year field, which in this case is a date.

### Default Value

This section contains the following properties:

#### Default Value

You can set a default value for the month and year field when creating a new entry. The default value is specified by entering a month and year in the default value field or by using a script expression by enabling the "Advanced" button in the month and year field settings.

**How to use the script expression:**

1. Open the month and year field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after the entry is created. When this option is enabled, an additional field appears for the default value.
   - **Triggers:** These can be used to specify when the script expression for the default value is applied, such as when the page loads, the form is submitted, the entry changes, or the field changes.

#### Lock Field

The "Lock Field" feature allows the user to lock the month and year field when creating a new entry. If this option is enabled, an additional input field appears in its scope, where the user can enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the month and year field settings.
2. Enable the "Lock Field" feature.
3. After enabling it, an additional field will appear. In this field, the user can enter a script expression (optional) that specifies the condition to be met to lock the field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the month and year field.

#### Hide Field

This allows the user to hide the month and year field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by going to the settings of the month and year field you want to hide.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for hiding the month and year field.

**Simple Example:**

When the "Subscription" checkbox is enabled, an additional "Subscription Month and Year" input field will be displayed. When this checkbox is disabled, the field will be hidden automatically.

#### Required

This determines whether the month and year field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by going to the settings of the month and year field you want to validate.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for making the month and year field required.

#### Searchable

The "Searchable" feature enables the search function in the month and year field when displaying entries in the user interface. When this feature is enabled for the field, users can search for values in this field using the search box in the entry display interface.

**How to use:**

1. Enable the "Searchable" feature in the month and year field settings.
2. Once enabled, the search function in this field will be activated.
3. In the interfaces: when clicking the search button and entering the desired search term in the search box, the system will also search in this field.

#### Unique

The "Unique" feature prevents duplicate values in the month and year field, ensuring that each value stored in this field is unique and does not repeat in other entries.

**How to use:**

1. Enable the "Unique" feature in the month and year field settings you want to make unique.
2. After enabling the feature, the system ensures that no duplicate values can be entered in this field.
3. When the user tries to enter a value that already exists in another field, they will be prevented and an alert message will be displayed indicating that this value is duplicated and a unique value must be used.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the ability to repeatedly enter the same month and year field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Go to "Field Settings" then "Field Value Settings" for the field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Specify Minimum and Maximum Repetitions (Optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum repetition fields are not filled, repetition will be unlimited, and users can add values ​​to the month and year field without limits.

#### Time Range

Description: The "Time Range" feature allows the user to specify a specific time range by selecting the start month and year and end month and year in the same month and year field.

**How to use:**

1. Enable the "Time Range" feature in the month and year field settings.
2. When the user selects a month and year in this field, arrows will appear above the calendar window to select the start and end month and year.
3. Using the "Time Range" feature improves the user experience and facilitates the process of determining the required time period.

#### Show in List

This feature allows displaying the value of the month and year field in the entry list, enabling the user to see the field value easily without having to open each entry individually.

**How to use:**

1. In the month and year field settings, open the "Field Value Settings" section and then the "Display" section, this will show the display properties.
2. Enable the "Show in List" option.

#### Main Date

The main date is a feature assigned to the date field in the entity, enabling you to specify the primary date that is relied upon mainly in the entity.