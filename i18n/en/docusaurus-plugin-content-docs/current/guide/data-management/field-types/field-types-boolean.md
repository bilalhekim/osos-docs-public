---
title: "Boolean"
sidebar_position: 12
---

# Boolean Field

By adding a Boolean field to the entity structure, users can specify a boolean value with just one click. This field is used for controlling simple binary options, where the value can either be true or false.

| Name     | Description                                     | Data Type  |
|----------|-------------------------------------------------|------------|
| Boolean  | A field that allows selecting a "True" or "False" value. | Boolean    |

## Advanced Settings

When clicking the settings icon on the Boolean field in the entity structure, a side window for advanced settings will open, displaying several sections as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you must specify a name for the Boolean field with translations in both Arabic and English.
2. **Normlized Name:** This includes the Normlized Name of the Boolean field, which is automatically generated from the name in English. This name can be changed and acts as a unique identifier (ID) for the Boolean field.
3. **Description:** Optional. This can be used to add a description for the Boolean field.
4. **Field Type:** Here, the data type stored in the Boolean field is displayed, which in this case is "Boolean".

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the Boolean field when creating a new entry. The default value is determined by a standard checkbox or through a script by enabling the "Advanced" button in the Boolean field settings.

**How to use: in case you want to use a script:**

1. Open the Boolean field settings.
2. Enable the "Advanced" button.
3. Enter the script representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after the entry is created. When this option is enabled, another field related to the default value will appear.
   - **Triggers:** These can be used to specify when the script for the default value should be applied, such as when loading the page, submitting the form, changing an entry, or when the Boolean field changes.

**Example:**
Suppose we have a field "Completed" and we want to make the default value for this field "False". We can achieve this by disabling the "Completed" checkbox. When creating a new entry, this field will automatically appear as unchecked and can be edited by the user if necessary.

#### Lock Field

The "Lock Field" property allows the user to lock the Boolean field when creating a new entry. If this option is enabled, an additional input field appears, allowing the user to enter an optional script to add a condition for locking the field.

**How to use:**

1. Open the Boolean field settings.
2. Enable the "Lock Field" property.
3. After enabling, an additional field will appear. In this field, the user can enter an optional script specifying the condition that must be met to lock the Boolean field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the Boolean field.

**Example:**

Suppose we have a Boolean field named "Completed" and another dropdown field named "Task" containing options like "Open" and "Closed". We want to lock the "Completed" field and set its value to "True" when the "Closed" option is selected in the "Task" field.

In this case, we will enable the "Lock Field" property for the Boolean field "Completed," then add a script in the "Lock Condition" for this field. Thus, when the "Closed" option is selected in the "Task" field, the "Completed" field will automatically lock and set its value to "True," preventing the user from changing it thereafter.

#### Hide Field

This allows the user to hide the Boolean field based on a specified condition, making it invisible when interacting with the form.

**How to use:**

1. Enable the "Hide Field" property by navigating to the settings of the Boolean field you want to hide.
2. After enabling, an additional field will appear for entering a script to specify the conditions for hiding the Boolean field.

**Example:**

When the Boolean field "Subscription" is enabled, an additional "Discount Code" field will appear. When this checkbox is disabled, the "Discount Code" field will automatically be hidden.

#### Required

This determines whether the Boolean field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" property by navigating to the settings of the Boolean field you want to validate.
2. After enabling, an additional field will appear for entering a script to specify the conditions for making the Boolean field required.

### Field Value Settings

This section contains the following properties:

#### Display

##### Show in List

This property allows displaying the Boolean field value in the list of entries, enabling users to see the Boolean field value without opening each entry individually.

**How to use:**

1. In the Boolean field settings, open the "Field Value Settings" section and then the "Display" section. Here, you will find the display-related properties.
2. Enable the "Show in List" option.

**Example:**

In the employee list of an HR management system, only the employee's name and ID number are shown. By enabling the "Show in List" option for the salary field, each employee's salary will be displayed next to their name in the employee list.