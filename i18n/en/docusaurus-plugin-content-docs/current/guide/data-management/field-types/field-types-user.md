---
title: "User"
sidebar_position: 24
---

# User Field

Adding a user field to the entity structure allows users to select a specific user within the form. This field can be used to link records to the responsible users or to assign users to specific activities or tasks.

| Name   | Description                                      | Data Type |
|--------|--------------------------------------------------|-----------|
| User   | A field that allows selecting a user from the list of registered users in the system. | Entity    |

## Advanced Settings

When clicking the settings icon for the user field in the entity structure, a sidebar with advanced settings for the user field will open. This sidebar contains several sections:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the user field with translations in both Arabic and English.

2. **Normlized Name:** Contains the Normlized Name for the user field, automatically generated from the English name. This name can be changed and serves as a unique identifier for the field.

3. **Description:** Optional, used to add a description for the user field.

4. **Data Type:** Shows the data type stored in the user field, which in this case is "User".

### Data Source

The data source property in the user field settings allows you to define the data source for the dropdown options in this field. It specifies where the options will be fetched from and displayed in the dropdown list for the user to select.

**How to use:**

1. Select the user field you want to set the data source for.
2. In the user field settings, navigate to the "Data Source" section.
3. Choose one of the following options as the data source for the dropdown:
   - All users: (default option) Fills the dropdown with all users in the system.
   - Group: When selecting this option, an additional field will appear to choose the "group" whose users will be used as options for the dropdown.
   - My organizational unit: Fills the dropdown with users belonging to the current user's organizational unit.

#### Default Value

You can set a default value for the user field when creating a new entry. The default value can be specified by selecting a user in the default value field or by using a script expression by enabling the "Advanced" option in the user field settings.

**How to use the script expression:**

1. Open the user field settings.
2. Enable the "Advanced" option.
3. Enter the script expression that represents the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock field:** Can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field will appear for the default value.
    - **Triggers:** Can be used to specify when the script expression for the default value should be applied, such as on page load, form submission, entry change, or field change.

### Lock Field

The "Lock Field" feature allows you to lock the user field when creating a new entry. If this option is enabled, an additional input field will appear, allowing you to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the user field settings.
2. Enable the "Lock Field" feature.
3. After enabling it, an additional field will appear. In this field, you can enter a script expression (optional) that specifies the condition to be met to lock the user field.
4. (Optional) If the "Lock Field" option is enabled, you must provide a default value for the user field.

### Hide Field

This allows you to hide the user field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by going to the user field settings you want to hide.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for hiding the user field.

**Simple Example:**

When the "Subscription" toggle is enabled, an additional "Subscription Type" field will be shown. When this toggle is disabled, the field will be hidden automatically.

#### Required

This determines whether the user field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by going to the user field settings you want to validate.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for making the user field required.

### Searchable

The "Searchable" feature allows you to enable the search function for the user field when displaying entries in the user interface. When this feature is enabled, users can search for values in this field using the search bar in the entry display interface.

**How to use:**

1. Enable the "Searchable" feature in the user field settings.
2. Once enabled, the search function will be activated for this field.
3. In the interfaces: When clicking the search button and entering the desired keyword in the search bar, the system will search in this field as well.

**Simple Example:**

Using the "Searchable" feature in the text field, users can search by entering part of the name in the search bar. The system will display all entries containing the entered keyword in the search bar. The system will search in all searchable fields, including this one.

### Field Value Settings

This section contains the following properties:

#### Multiple

When the "Multiple" feature is enabled, the user can select more than one value from the available options.

**How to use:**

To enable the multiple values feature, follow these steps:

1. Go to the user field settings.
2. Find the "Multiple" option and enable it.
3. Once enabled, the user will be able to select multiple values from the available options.

#### Repeatable

The "Repeatable" feature represents the ability to repeatedly enter the same user field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Go to "Field Settings" then "Field Value Settings" for the field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Specify Minimum and Maximum Repetitions (Optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum repetition fields are not filled, repetition will be unlimited, and users can add values ​​to the user field without limits.

#### Show in List

This feature allows displaying the value of the user field in the entry list, enabling the user to see the field value easily without having to open each entry individually.

**How to use:**

1. In the user field settings, open the "Field Value Settings" section and then the "Display" section, this will show the display properties.
2. Enable the "Show in List" option.

#### Main Reference

The main reference is a feature that allows you to specify the reference that will be used as the main reference for the entity.