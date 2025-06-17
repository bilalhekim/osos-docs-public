---
title: "Long Text Field"
sidebar_position: 2
---

# Long Text Field

Adding a long text field to the entity structure allows users to enter detailed and extensive text within the form. The long text field enables users to write and edit lengthy texts such as articles, descriptions, notes, and any other text that requires a large text field.

| Name       | Description                             | Data Type  |
|------------|-----------------------------------------|------------|
| Long Text  | Field allows entering long text.        | Text       |

## Advanced Settings

Clicking on the "Settings" button in the long text field within the entity structure opens a side window for advanced settings. This window has several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the long text field with translations in Arabic and English.
2. **Normlized Name:** Contains the Normlized Name for the long text field, automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the field.
3. **Description:** An optional field for adding a description of the long text field.
4. **Data Type:** Shows the data type stored in the long text field, which in this case is Text.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the long text field when creating a new entry. The default value is set by entering the long text in the default value field or by using a script expression by enabling the "Advanced" option in the long text field settings.

**Usage: To use a script expression:**

1. Open the long text field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after creating the entry. Enabling this option will display another field related to the default value.
   - **Triggers:** These can be used to specify when the script expression for the default value should be applied, such as on page load, form submission, entry change, or field change.

#### Lock Field

The lock field feature allows the user to lock the long text field when creating a new entry. If this option is enabled, an additional input field will appear, allowing the user to enter an optional script expression to lock the field.

**Usage:**

1. Open the long text field settings.
2. Enable the lock field option.
3. After enabling, an additional field will appear where the user can enter an optional script expression specifying the condition for locking the field.
4. (Optional) If the lock field option is enabled, the user must provide a default value for the long text field.

#### Hide Field

This feature allows the user to hide the long text field based on a specified script expression, making it invisible when interacting with the form.

**Usage:**

1. Enable the hide field option in the long text field settings.
2. After enabling, an additional field will appear for entering the script expression to hide the long text field.

**Simple Example:**

When the "Subscription" checkbox is enabled, an additional "Subscription Description" input field will be shown. When this checkbox is disabled, the "Subscription Description" field will be hidden automatically.

#### Required

This feature specifies whether the long text field is required to complete the form or can be left empty.

**Usage:**

1. Enable the required option in the long text field settings.
2. After enabling, an additional field will appear for entering the script expression to make the long text field required.

#### Searchable

The "Searchable" property allows enabling the search function within the long text field when displaying entries in the user interface. When this property is enabled, users can search for values within this field using the search box in the entries display interface.

**Usage:**

1. Enable the searchable option in the long text field settings.
2. Once enabled, the search function will be activated within this field.
3. In interfaces: Clicking the search button and entering the word to be searched in the search box will make the system search within this field.

**Simple Example:**

Using the searchable property in the long text field, users can search by entering part of the name in the search box. The system will display all entries that contain the entered word in the search box. The system will search within all searchable fields, including this field.

#### Unique

The "Unique" property prevents duplicate values in the long text field, ensuring that each value stored in this field is unique and does not repeat in other entries.

**Usage:**

1. Enable the unique option in the long text field settings.
2. After enabling, the system ensures that no duplicate value can be entered in this field.
3. When a user tries to enter a value that already exists in another field, the system will prevent it and display an alert message indicating that this value is duplicated and a unique value must be used.

**Simple Example:**

In a database for an employee management system, there might be a field for job titles for each employee. Using the unique property in this field ensures that the system does not allow duplicate job titles.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" property represents the ability to repeat the same long text field with different values in the same entry. Enabling this option allows users to add multiple values to the same field within a single entry.

**Usage:**

1. Go to "Field Settings" then to "Field Value Settings" for the long text field you want to make repeatable.
2. Enable the "Repeatable" property.

**Setting Minimum and Maximum Limits (Optional):**

After enabling the "Repeatable" property, two additional fields will appear where you can specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum fields are left empty, repetitions will be unlimited, allowing the user to add values to the long text field without restriction.

#### Show in List

This property allows the long text field value to be displayed in the list of entries, enabling the user to see the field value without opening each entry individually.

**Usage:**

1. In the long text field settings, open the "Field Value Settings" section.
2. Open the "Display" section.
3. Enable the "Show in List" option.

#### Main Title

The main title property allows you to specify the main title that will be primarily used for the entity. When setting the long text field as the main title, it will be used as the reference title for the entity in various locations. 

#### Subtitle

The subtitle property allows you to add an additional subtitle that will be displayed alongside the main title in the entity. 

#### Subtitle 2

Subtitle 2 is a property assigned to the title field in the entity, allowing you to add another additional subtitle displayed alongside the main title and subtitle in the entity. Subtitle 2 can be used to clarify the main title and subtitle or to add other additional information about the entity.