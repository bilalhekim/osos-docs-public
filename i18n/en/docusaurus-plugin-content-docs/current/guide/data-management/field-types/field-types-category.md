---
title: "Category"
sidebar_position: 13
---

# Category Field

By adding the Category field to the entity structure, users can select categories with just one click on the field. A list of available categories will appear, allowing the user to easily choose the appropriate category.

| Name         | Description                                                         | Data Type |
|--------------|---------------------------------------------------------------------|-----------|
| Category     | A field that allows selecting a value from a dropdown list of options. | Json      |

## Advanced Settings

When clicking the settings icon on the Category field in the entity structure, a side window for advanced settings will open, displaying several sections as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you must specify a name for the Category field with translations in both Arabic and English.
2. **Normlized Name:** This includes the Normlized Name of the Category field, which is automatically generated from the name in English. This name can be changed and acts as a unique identifier (ID) for the Category field.
3. **Description:** Optional. This can be used to add a description for the Category field.
4. **Data Type:** Here, the data type stored in the Category field is displayed, which in this case is JSON.

### Add Options

The "Add Options" feature allows users to add additional options to the Category fields. When using this feature in the Category field, users can add new options to the dropdown list available for categories.

**How to use:**

1. Go to the settings of the Category field you want to add options to.
2. There is an input field where you can enter the name of the option.
3. After entering the option name, click on the translation icon at the end of the field to add an English translation for the option.
4. Click the "Add" button, and the option will be added to the dropdown list for the Category field.
5. Choose a color for the option using the color picker.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the Category field when creating a new entry. The default value is selected by choosing an option from the category in the default value field or through a script by enabling the "Advanced" button in the Category field settings.

**How to use: in case you want to use a script:**

1. Open the Category field settings.
2. Enable the "Advanced" button.
3. Enter the script representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after the entry is created. When this option is enabled, another field related to the default value will appear.
   - **Triggers:** These can be used to specify when the script for the default value should be applied, such as when loading the page, submitting the form, changing the entry, or changing the field.

#### Lock Field

The "Lock Field" feature allows users to lock the Category field when creating a new entry. If this option is enabled, an additional input field will appear, allowing the user to enter an optional script to add a condition for locking the field.

**How to use:**

1. Open the Category field settings.
2. Enable the "Lock Field" feature.
3. After enabling, an additional field will appear. In this field, the user can enter an optional script to specify the condition that must be met to lock the Category field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the Category field.

#### Hide Field

The "Hide Field" feature allows users to hide the Category field based on a specific condition, making it invisible when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by navigating to the Category field settings you want to hide.
2. After enabling it, an additional field will appear for entering the script that specifies the conditions for hiding the Category field.

**Simple Example:**

When enabling the "Subscription" checkbox, an additional "Subscription Type" category field will be shown. When disabling this checkbox, the "Subscription Type" category field will be hidden automatically.

#### Required

This specifies whether the Category field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by navigating to the Category field settings you want to validate.
2. After enabling it, an additional field will appear for entering the script that specifies the conditions for making the Category field required.

#### Searchable

The "Searchable" feature allows users to enable the search function for the Category field when displaying entries in the user interface. When this feature is enabled, users can search for values in this field using the search box in the entry display interface.

**How to use:**

1. Enable the "Searchable" feature in the Category field settings.
2. Once enabled, the search function in this field will be activated.
3. In the interfaces: When clicking the search button and entering the keyword in the search box, the system will search in this Category field as well.

**Simple Example:**

Using the "Searchable" feature in the Category field, users can search by entering part of the name in the search box. The system will display all fields containing the entered keyword in the search box. The system will search in all searchable fields, including this Category field.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the ability to enter the same Category field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Navigate to the settings of the field, then to the "Field Value Settings" section of the field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Specify Minimum and Maximum Repetition (Optional):**

After enabling the "Repeatable" feature, two additional fields will appear, which can be used to specify the minimum and maximum number of repetitions allowed.

**Note:** If the minimum and maximum fields are not filled in, repetition will be unlimited, and users can add values to the Category field indefinitely.

#### Show in List

This feature allows displaying the value of the Category field in the entry list, so the user can easily see the field value without opening each entry individually.

**How to use:**

1. In the Category field settings, open the "Field Value Settings" section, then the "Display" section. This will show the display-related features.
2. Enable the "Show in List" option.

#### Main Category

The main category is a feature assigned to the category field in the entity, making this field the highest priority category in the entity.

#### Subcategory

The subcategory is a feature assigned to the category field in the entity, allowing you to add subcategories for more detailed and organized entry display.