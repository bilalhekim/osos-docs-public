---
title: "Switch"
sidebar_position: 23
---

# Switch Field

Adding a Switch field to the entity structure allows users to enable or disable a specific option with a single click. The Switch is displayed as a button that can be slid to the right or left to enable or disable the option.

| Name      | Description                             | Data Type     |
|-----------|-----------------------------------------|---------------|
| Switch    | A field that allows toggling between different values. | Boolean       |

## Advanced Settings

Clicking the settings icon on the Switch field in the entity structure opens a sidebar for advanced settings. This sidebar contains several sections:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the Switch field with translations in both Arabic and English.

2. **Normlized Name:** Contains the Normlized NameName for the Switch field, automatically generated from the English name. This name can be changed and serves as a unique identifier for the field.

3. **Description:** Optional, used to add a description for the Switch field.

4. **Data Type:** Shows the data type stored in the Switch field, which in this case is "Boolean."

### Answer Options

The "Answer Options" feature allows specifying the type of Switch and customizing the values corresponding to each state.

**Usage:**

1. Go to the Switch field settings.
2. Find the "Answer Options" section.
3. In the first field, select the Switch type from the following options:
   - Choice: A regular Switch state that allows the user to select one answer from the available options.
   - Switch: A binary Switch state that allows the user to enable or disable the state.
   - Selection Group: A Switch state used to create a group of options.

4. In the second field, the user can enter the name of the new option they want to add. The user can also provide translations for the new option by clicking the translation icon at the end of the field and entering the translation in Arabic and English.

5. After clicking the "Add" button, the options you added will appear in the type of Switch you previously selected.

### Default Value

This section contains the following properties:

#### Default Value

You can set a default value for the Switch field when creating a new entry. The default value can be specified by selecting an option from the Switch in the default value field or by using a script expression by enabling the "Advanced" option in the Switch field settings.

**How to use: If you want to use a script expression:**

1. Open the Switch field settings.
2. Enable the "Advanced" option.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** Can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field will appear for the default value.
    - **Triggers:** Can be used to specify when the script expression for the default value should be applied, such as on page load, form submission, entry change, or field change.

#### Lock Field

The "Lock Field" feature allows you to lock the Switch field when creating a new entry. If this option is enabled, an additional input field will appear, allowing you to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the field settings.
2. Enable the "Lock Field" feature.
3. After enabling it, an additional field will appear. In this field, you can enter a script expression (optional) specifying the condition to be met to lock the Switch field.
4. (Optional) If the "Lock Field" option is enabled, you must provide a default value for the Switch field.

#### Hide Field

This allows you to hide the Switch field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by going to the Switch field settings you want to hide.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for hiding the Switch field.

**Simple Example:**

When the "Subscription" Switch is enabled, an additional "Subscription Type" field will be shown. When this Switch is disabled, the field will be hidden automatically.

#### Required

This determines whether the Switch field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by going to the Switch field settings you want to validate.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for making the Switch field required.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the ability to repeatedly enter the same Switch field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Go to the "Field Settings" then to the "Field Value Settings" for the field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Specify Minimum and Maximum Repetitions (Optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum repetition fields are not filled, repetition will be unlimited, and users can add values to the Switch field without limits.

#### Show in List

This feature allows displaying the value of the Switch field in the entry list, enabling the user to see the field value easily without having to open each entry individually.

**How to use:**

1. In the Switch field settings, open the "Field Value Settings" section and then the "Display" section, this will show the display properties.
2. Enable the "Show in List" option.