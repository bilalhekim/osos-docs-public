---
title: "Mapped Field"
sidebar_position: 26
---

# Mapped Field

Adding a mapped field to the entity structure allows users to read values from fields within a related entity, filter according to these fields, update field values, and store them either at the entity level or the related entity level. It also allows for synchronization of updates across all entities.

| Name          | Description                          | Data Type      |
|---------------|--------------------------------------|----------------|
| Mapped Field  | Field allowing reading values from a related entity's field | Dependent on the linked field from the related entity |

## Advanced Settings

Clicking on the settings icon in the mapped field within the entity structure opens a side window for advanced settings. This window has several sections, as follows:

### Basic Settings

This section contains seven fields:

1. **Relation Field:** Contains the selected relationship from the relationships defined within the current entity.
2. **Source Field:** One of the related entity's fields chosen as the source for the mapped field.
3. **Update Option:** Select the appropriate update option from the following:
   - Never: Not editable.
   - Local update: Editable within the current entity but not reflected in the parent entity.
   - From Parent Entity: Not editable from the current entity but editable from the parent entity, with changes reflected in the current entity.
   - 2-way: Editable from both the current and parent entities, with changes reflected in both.
4. **Field Name:** Specify a name for the mapped field with translations in Arabic and English.
5. **Description:** An optional field for adding a description of the mapped field.
6. **Normlized Name:** Contains the Normlized Name for the mapped field, automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the mapped field.
7. **Data Type:** Shows the data type stored in the mapped field, which in this case is text.

### Lock Field

This feature allows the user to lock the mapped field when creating a new entry. This option is enabled if the selected update option is "Never" or "2-way". It displays an additional input field for the user to enter an optional script expression. This feature is unavailable if the update option is "Local update" or "From Parent Entity".

#### How to Enable Lock Field:

1. Open the mapped field settings.
2. Select the "Never" or "2-way" update option.
3. The lock field feature will be enabled.
4. An additional field will appear, allowing the user to enter a script expression to lock the field.

### Hide Field

The hide field feature allows the user to hide the mapped field based on a specified script expression, making it invisible when interacting with the form.

#### How to Enable Hide Field:

1. Open the mapped field settings.
2. Enable the hide field feature.
3. An additional field will appear, allowing the user to enter a script expression to hide the field.

### Required

This feature specifies whether the mapped field is required to complete the form or can be left empty.

#### How to Enable Required:

1. Open the mapped field settings.
2. Enable the required feature.
3. An additional field will appear, allowing the user to enter a script expression to make the field required.

### Searchable

When this feature is enabled, the values in the mapped field become searchable in the search box when displaying entries in the user interface.

#### How to Enable Searchable:

1. Open the mapped field settings.
2. Enable the searchable feature.

### Unique

When this feature is enabled, the values in the mapped field become unique, ensuring that each value stored in this field is unique and does not repeat in other entries.

#### How to Enable Unique:

1. Open the mapped field settings.
2. Enable the unique feature.

### Value Format

This feature allows the user to choose the text format for displaying the field value. When a value is entered, it is checked against the specified format.

#### How to Choose Value Format for Text Mapped Field:

1. Open the mapped field settings.
2. Open the value format options list, showing:
   - **No Format:** The default option.
   - **Email:** When this format is enabled, the user must enter a value matching an email format.
   - **URL:** When this format is enabled, the user must enter a value matching a URL format.

#### How to Choose Value Format for Number Mapped Field:

1. Open the mapped field settings.
2. Open the value format options list, showing:
   - **General Number:** The default option.
   - **Percentage:** The user can specify the number format as a fixed percentage and:
     - Set precision (a numeric value defining the number of decimal places, from 0 to 3, with the default being 0).
     - Choose the display format from the dropdown list, which includes:
       - **Percentage:** The default option.
       - **Progress Bar.**
       - **Progress Bar with Percentage.**

### Field Value Settings

#### Minimum and Maximum Values

The minimum and maximum value feature allows users to set constraints on the data that can be entered in a specific field, ensuring that the entered values are within an acceptable range and maintaining data integrity. If no values are set for the minimum or maximum, the field will accept any value within its data type range.

##### How to Set Minimum and Maximum Values for a Field:

1. Open the field settings.
2. Go to the field value settings.
3. Enter values for the minimum and maximum fields:
   - Minimum: Enter the lowest acceptable value for this field.
   - Maximum: Enter the highest acceptable value for this field.

###### Usage Examples:

**Example 1:** Numeric Field

If you have a numeric field and want the values to be between 1 and 100:
Minimum = 1
Maximum = 100

**Example 2:** Text Field with a Specified Length

If you have a text field and want the length of the text to be between 5 and 50 characters:
Minimum = 5
Maximum = 50

#### Show in List

This feature allows the mapped field value to be displayed in the list of entries, enabling users to see the field value without opening each entry individually.

#### How to Use:

1. Open the mapped field settings.
2. Open the "Field Value Settings" section.
3. Open the "Display" section.
4. Enable the "Show in List" option.

#### Make the Field:

This feature allows the user to activate one of the following options:
1. Main Title: Assigns the field as the main title.
2. Subtitle 1.
3. Subtitle 2.