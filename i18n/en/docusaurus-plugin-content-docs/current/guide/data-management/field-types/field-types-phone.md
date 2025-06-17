---
title: "Phone Field"
sidebar_position: 20
---

# Phone Field

By adding a phone field to the entity structure, users can easily enter phone numbers within the form. The phone field can be used to record various phone numbers, whether local or international.

| Name   | Description                                              | Data Type |
|--------|----------------------------------------------------------|-----------|
| Phone  | A field that allows entering a phone number considering the country and area code. | Text      |

## Advanced Settings

Clicking on the "Settings" button in the phone field within the entity structure will open a side window for advanced settings of the phone field. This window displays several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you should specify a name for the phone field with translations in Arabic and English.

2. **Normlized NameName:** This contains the Normlized NameName for the phone field, which is automatically generated from the name in English. This name can be changed and serves as a unique identifier for the phone field.

3. **Description:** Optional, can be used to add a description for the phone field.

4. **Data Type:** This shows the data type stored in the phone field, which in this case is: Text.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the phone field when creating a new entry. The default value is specified by entering the phone number in the default value field or using a script expression by enabling the "Advanced" button in the phone field settings.

**How to use: in case of using a script expression:**

1. Open the phone field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field related to the default value will appear.
    - **Triggers:** These can be used to specify when the script expression for the default value is applied, such as when the page loads, the form is submitted, the entry is changed, or the field is changed.

#### Lock Field

The "Lock Field" feature allows the user to lock the phone field when creating a new entry. If this option is enabled, an additional input field appears in its scope, allowing the user to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the phone field settings.
2. Enable the "Lock Field" feature.
3. After enabling, an additional field will appear. In this field, the user can enter a script expression (optional) to define the condition that must be met to lock the phone field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the phone field.

#### Hide Field

Allows the user to hide the phone field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by navigating to the phone field settings that you want to hide.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for hiding the phone field.

**Simple Example:**

When the "Subscription" toggle field is enabled, an additional "Subscription Phone" phone field will be shown. When this toggle is disabled, it will be automatically hidden.

#### Required

Specifies whether the phone field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by navigating to the phone field settings that need to be completed.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for making the phone field required.

### Searchable

The "Searchable" feature allows enabling the search function in the phone field when displaying entries in the user interface. When this feature is enabled in the field, users can search for values in this field using the search box in the entries display interface.

**How to use:**

1. Enable the "Searchable" feature in the phone field settings.
2. Once enabled, the search function in this phone field will be activated.
3. In the interfaces: Clicking the search button and entering the search term in the search box will enable the system to search in this field as well.

#### Unique

The "Unique" feature prevents duplicate values in the phone field, ensuring that each value stored in this field is unique and not repeated in other entries.

**How to use:**

1. Enable the "Unique" feature in the phone field settings that you want to make unique.
2. After enabling the feature, the system ensures that no duplicate value can be entered in this field.
3. When a user attempts to enter a value that already exists in another field, the system will prevent it and display an alert indicating that this value is duplicated and must be unique.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the possibility of repeating the same phone field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Navigate to "Field Settings" and then to "Field Value Settings" for the phone field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Set the minimum and maximum repetitions (optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to set the minimum and maximum number of repetitions allowed.

**Note:** If the fields for setting the minimum and maximum values are not filled, the repetition will be unlimited, allowing users to add values to the phone field indefinitely.

#### Show in List

This feature allows the phone field value to be displayed in the list of entries, enabling users to see the field value without opening each entry individually.

**How to use:**

1. In the phone field settings, open the "Field Value Settings" section and then the "Display" section. This will show the display-related features.
2. Enable the "Show in List" option.

#### Main Phone

The main phone feature allows specifying the primary phone number associated with the entity. This phone number can be displayed and used as a primary contact point or reference.

#### Main Title

The main title feature allows you to specify the main title that will be used primarily in the entity. When assigning the phone field as the main title, it will be used as the primary reference title for the entity in various places. 

#### Sub Title

The subtitle is a feature that assigns a subtitle to the entity, allowing you to add an additional subtitle that is displayed alongside the main title in the entity. 

#### Caption

The caption is a feature that assigns an additional subtitle to the entity, allowing you to add another subtitle that is displayed alongside the main title and subtitle in the entity. The caption can be used to further clarify the main title and subtitle or to add other additional information about the entity.