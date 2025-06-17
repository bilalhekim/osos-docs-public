---
title: "Password Field"
sidebar_position: 19
---

# Password Field

By adding a password field to the entity structure, users can enter a secure and confidential password based on system requirements. When a password is entered in this field, the characters are obscured to protect the entered information. When modifying the entry, the user cannot see the previously entered password in the field, and if they want to change it, they must enter a new password.

| Name      | Description                               | Data Type |
|-----------|-------------------------------------------|-----------|
| Password  | A field that allows entering a secure password. | Text      |

## Advanced Settings

Clicking on the "Settings" button in the password field within the entity structure will open a side window for advanced settings of the password field. This window displays several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you should specify a name for the password field with translations in Arabic and English.
2. **Normlized Name:** This contains the Normlized Name for the password field, which is automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the password field.
3. **Description:** Optional, can be used to add a description for the password field.
4. **Data Type:** This shows the data type stored in the password field, which in this case is: Text.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the password field when creating a new entry. The default value is specified by entering the password in the default value field or using a script expression by enabling the "Advanced" button in the password field settings.

**How to use: in case of using a script expression:**

1. Open the password field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
  - **Lock Field:** This can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field related to the default value will appear.
  - **Triggers:** These can be used to specify when the script expression for the default value is applied, such as when the page loads, the form is submitted, the entry is changed, or the field is changed.

#### Lock Field

The "Lock Field" feature allows the user to lock the password field when creating a new entry. If this option is enabled, an additional input field appears in its scope, allowing the user to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the password field settings.
2. Enable the "Lock Field" feature.
3. After enabling, an additional field will appear. In this field, the user can enter a script expression (optional) to define the condition that must be met to lock the password field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the password field.

#### Hide Field

Allows the user to hide the password field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by navigating to the password field settings that you want to hide.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for hiding the password field.

**Simple Example:**

When the "Subscription" toggle field is enabled, an additional "Subscription Password" password field will be shown. When this toggle is disabled, it will be automatically hidden.

#### Required

Specifies whether the password field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by navigating to the password field settings that need to be completed.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for making the password field required.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the possibility of repeating the same password field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Navigate to "Password Field Settings" and then to "Field Value Settings" for the password field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Set the minimum and maximum repetitions (optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to set the minimum and maximum number of repetitions allowed.

**Note:** If the fields for setting the minimum and maximum values are not filled, the repetition will be unlimited, allowing users to add values to the password field indefinitely.

#### Show in List

This feature allows the password field value to be displayed in the list of entries, enabling users to see the field value without opening each entry individually.

**How to use:**

1. In the password field settings, open the "Field Value Settings" section and then the "Display" section. This will show the display-related features.
2. Enable the "Show in List" option.