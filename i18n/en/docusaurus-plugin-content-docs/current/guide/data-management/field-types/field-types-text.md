---
title: "Text"
sidebar_position: 1
---

# Text Field

Adding a text field to the entity structure allows users to easily enter text within the form. The text field enables users to input short text, such as names, titles, and other information that requires a small text field.

| Name      | Description                      | Data Type |
|-----------|----------------------------------|-----------|
| Text      | A field that allows short text input. | Text      |

## Advanced Settings

Clicking the "Settings" button in the text field in the entity structure opens a sidebar for advanced settings. This sidebar contains several sections:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the text field with translations in both Arabic and English.

2. **Normlized Name:** Contains the Normlized Name for the text field, automatically generated from the English name. This name can be changed and serves as a unique identifier for the field.

3. **Description:** Optional, used to add a description for the text field.

4. **Data Type:** Shows the data type stored in the text field, which in this case is "Text."

### Default Value

This section contains the following properties:

#### Default Value

You can set a default value for the text field when creating a new entry. The default value can be specified by entering text in the default value field or by using a script expression by enabling the "Advanced" option in the text field settings.

**How to use: If you want to use a script expression:**

1. Open the text field settings.
2. Enable the "Advanced" option.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** Can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field will appear for the default value.
    - **Triggers:** Can be used to specify when the script expression for the default value should be applied, such as on page load, form submission, entry change, or field change.

#### Lock Field

The "Lock Field" feature allows you to lock the text field when creating a new entry. If this option is enabled, an additional input field will appear, allowing you to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the text field settings.
2. Enable the "Lock Field" feature.
3. After enabling it, an additional field will appear. In this field, you can enter a script expression (optional) specifying the condition to be met to lock the text field.
4. (Optional) If the "Lock Field" option is enabled, you must provide a default value for the text field.

#### Hide Field

This allows you to hide the text field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by going to the text field settings you want to hide.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for hiding the text field.

**Simple Example:**

When the "Subscription" toggle is enabled, an additional "Subscription Title" field will be shown. When this toggle is disabled, the field will be hidden automatically.

#### Required

This determines whether the text field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by going to the text field settings you want to validate.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for making the text field required.

### Searchable

The "Searchable" feature allows you to enable the search function for the text field when displaying entries in the user interface. When this feature is enabled, users can search for values in this text field using the search bar in the entry display interface.

**How to use:**

1. Enable the "Searchable" feature in the text field settings.
2. Once enabled, the search function will be activated for this field.
3. In the interfaces: When clicking the search button and entering the desired keyword in the search bar, the system will search in this field as well.

**Simple Example:**

Using the "Searchable" feature in the text field, users can search by entering part of a name in the search bar. The system will display all entries containing the entered keyword in the search bar. The system will search in all searchable fields, including this field.

### Unique

The "Unique" feature ensures that each value stored in this text field is unique and does not repeat in other entries.

**How to use:**

1. Enable the "Unique" feature in the text field settings.
2. After enabling it, the system ensures that no duplicate values can be entered in this field.
3. When a user tries to enter a value that already exists in another field, they will be prevented and shown a warning message indicating that the value is a duplicate and a unique value must be used.

**Simple Example:**

In an employee management system database, you may have a job title field for each employee. By enabling the **"Unique"** property on this field, the system ensures that job titles cannot be duplicated.

### Text Field Format and Validation

The system allows you to define the format of a text field to validate the entered values. You can choose from the following text formats:

- **Unformatted:** The value is treated as plain text without any validation.  
- **URL:** The system checks that the entered value is a valid URL.  
- **Email:** The system checks that the entered value is a valid email address.

Choosing the appropriate format ensures that values comply with usage requirements and helps reduce input errors.

#### Setting the Text Format to URL

1. Go to the entity structure settings.  
2. Add a new field of type "Text".  
3. Go to the advanced field settings.  
4. Select "URL" from the available text formats.  
5. Save the settings.  

When a value is entered in this field, the system will validate it as a proper URL.  
If the value is invalid, the system will display a warning message below the field: **"Invalid value"**.

#### Setting the Text Format to Email

1. Repeat the same steps above.  
2. Select "Email" from the available text formats.  
3. Save the settings.  

When a value is entered in this field, the system will validate it as a proper email address.  
If the value is invalid, a warning message will appear below the field: **"Invalid value"**.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the ability to repeatedly enter the same text field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Go to "Field Settings" then to "Field Value Settings" for the field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Specify Minimum and Maximum Repetitions (Optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum repetition fields are not filled, repetition will be unlimited, and users can add values to the text field without limits.

#### Show in List

This feature allows displaying the value of the text field in the entry list, enabling the user to see the field value easily without having to open each entry individually.

**How to use:**

1. In the text field settings, open the "Field Value Settings" section and then the "Display" section, this will show the display properties.
2. Enable the "Show in List" option.

#### Main Title

The main title feature enables you to designate the main title that will be primarily used in the entity. When the text field is set as the main title, it will be used as the reference title for the entity in many places. 

#### Subtitle

The subtitle feature is assigned to a title field in the entity, allowing you to add an additional subtitle displayed alongside the main title in the entity. 

#### Subtitle 2

Subtitle 2 is a feature assigned to a title field in the entity, enabling you to add another subtitle displayed alongside the main title and subtitle in the entity. Subtitle 2 can be used to further clarify the main title and subtitle or to add other additional information about the entity.