---
title: "Number Field"
sidebar_position: 4
---

# Number Field

By adding a number field to the entity structure, users can easily input numerical values within the form. The number field is used for recording numeric values such as ages, quantities, percentages, and any other information that requires a numeric field.

| Name        | Description                                | Data Type |
|-------------|--------------------------------------------|-----------|
| Number      | A field that allows entering a numeric value. | Number    |

## Advanced Settings

Clicking on the "Settings" button in the "Number" field within the entity structure will open a side window for advanced settings of the number field. This window displays several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you should specify a name for the number field with translations in Arabic and English.
2. **Normlized Name:** This contains the Normlized Name for the number field, which is automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the number field.
3. **Description:** Optional, can be used to add a description for the number field.
4. **Data Type:** This shows the data type stored in the number field, which in this case is: Number.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the number field when creating a new entry. The default value is specified by entering a number in the default value field or using a script expression by enabling the "Advanced" button in the number field settings.

**How to use: in case of using a script expression:**

1. Open the number field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after creating the entry. When this option is enabled, another field related to the default value will appear.
   - **Triggers:** These can be used to specify when the script expression for the default value is applied, such as when the page loads, the form is submitted, the entry is changed, or the field is changed.

#### Lock Field

The "Lock Field" feature allows the user to lock the number field when creating a new entry. If this option is enabled, an additional input field appears in its scope, allowing the user to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the number field settings.
2. Enable the "Lock Field" feature.
3. After enabling, an additional field will appear. In this field, the user can enter a script expression (optional) to define the condition that must be met to lock the number field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the number field.

#### Hide Field

Allows the user to hide the number field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by navigating to the number field settings that you want to hide.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for hiding the number field.

**Simple Example:**

When the "Subscription" toggle field is enabled, an additional "Subscription Number" number field will be shown. When this toggle is disabled, it will be automatically hidden.

#### Required

Specifies whether the number field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by navigating to the number field settings that need to be completed.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for making the number field required.

#### Searchable

The "Searchable" feature allows enabling the search function within the number field when displaying entries in the user interface. When this feature is activated, users can search for values in this field using the search box in the entries display interface.

**How to use:**

1. Enable the "Searchable" feature in the number field settings.
2. Once the feature is activated, the search function in this number field will be enabled.
3. In the interfaces: When clicking the search button and entering the word to search for in the search box, the system will search in this number field as well.

#### Unique

The "Unique" feature prevents duplicate values in the number field, ensuring that each value stored in this field is unique and does not repeat in other entries.

**How to use:**

1. Enable the "Unique" feature in the number field settings you want to make unique.
2. After enabling the feature, the system ensures that a duplicate value cannot be entered in this field.
3. When the user tries to enter a value that already exists in another field, they will be prevented, and a warning message will be displayed indicating that this value is a duplicate and a unique value must be used.

### Numeric Field Format and Display

This feature allows you to define the format of a number, ensuring that entered values comply with the selected type and format.

#### Numeric Field Format – Number

Used to display numbers in their standard form without converting them to special formats like percentages or currencies. This is the default and most suitable format for general numbers that do not require additional customization.

#### Numeric Field Format – Percentage

You can configure the numeric field as a percentage to clearly and neatly display values in this format.

##### How to Use

1. Go to the entity structure settings.  
2. Add a new field of type "Number".  
3. In the advanced field settings:  
   - Select the format "Percentage".  
   - Choose the display style from the dropdown:
     - Percentage (default).  
     - Progress Bar.  
     - Progress Bar with Percentage.  
   - Set the precision: select the number of decimal places (from 0 to 3). The default is 0.

##### Example:

- **Setup:** Display style set to "Progress Bar with Percentage".  
- **Input:** The user enters "75" into the field.  
- **Result:**  
  - A "%" symbol appears next to the input field to indicate the format.  
  - On viewing the entry, the field is shown as a progress bar reflecting 75%.

#### Numeric Field Format – Currency

You can configure the numeric field as a currency to handle financial values and ensure they are displayed accurately.

##### How to Use

1. Go to the entity structure settings.  
2. Add a new field of type "Number".  
3. In the advanced field settings:  
   - Select the format "Currency".  
   - Choose the currency type from the dropdown list.  
   - Configure the currency formatting options:
     - **Decimal Places:** Set the number of decimal places based on the chosen currency.
     - **Decimal Separator:** Choose how large numbers are displayed using the following options:
       - Comma and dot: `1,000,000.00`
       - Dot and comma: `1.000.000,00`
       - Space and comma: `1 000 000,00`
       - Space and dot: `1 000 000.00`
     - **Large Number Shortcuts:** Choose from:
       - No abbreviation.  
       - Thousand.  
       - Million.  
       - Billion.  
     - **Allow Negative Numbers:** Enable this option if negative values are allowed.

###### Example:

- **Setup:**  
  - The admin adds a new "Number" field to the entity structure.  
  - Selects the "Currency" format.  
  - Configures the following:
    - Currency type: "Saudi Riyal"  
    - Decimal places: 2  
    - Large number abbreviation: "Million"  
    - Allow negative numbers: Enabled  
- **Input:** The user enters the value `-1500000`.  
- **Result:** The field displays as `-1.5M` with the currency settings applied.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" feature represents the possibility of repeating the same number field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Navigate to "Number Field Settings" and then to "Field Value Settings" for the number field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Set the minimum and maximum repetitions (optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to set the minimum and maximum number of repetitions allowed.

**Note:** If the fields for setting the minimum and maximum values are not filled, the repetition will be unlimited, allowing users to add values to the number field indefinitely.

#### Show in List

This feature allows the number field value to be displayed in the list of entries, enabling users to see the field value without opening each entry individually.

**How to use:**

1. In the number field settings, open the "Field Value Settings" section and then the "Display" section. This will show the display-related features.
2. Enable the "Show in List" option.

#### Main Number

The main number is a feature assigned to the number field in the entity, allowing you to set the primary number to be used as the main reference for the entity. When this field is set as the main number, it will be prominently displayed over other numbers in the entity.