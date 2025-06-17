---
title: "Sequence"
sidebar_position: 22
---

# Sequence Field

Adding a sequence field to the entity structure allows users to record a sequential numeric order within the form. The sequence field is used to record a series of consecutive numbers or the numeric order of entries.

| Name      | Description                             | Data Type     |
|-----------|-----------------------------------------|---------------|
| Sequence  | A field that allows for automatic number sequencing. | Number        |  

## Advanced Settings

Clicking the "Settings" button on the "Sequence" field in the entity structure opens a sidebar for advanced settings. This sidebar contains several sections:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the sequence field with translations in both Arabic and English.

2. **Normlized Name:** Contains the Normlized NameName for the sequence field, automatically generated from the English name. This name can be changed and serves as a unique identifier for the field.

3. **Description:** Optional, used to add a description for the sequence field.

4. **Data Type:** Shows the data type stored in the sequence field, which in this case is "Number."

### Auto Increment Settings 

The "Auto Increment Settings" feature allows users to specify the starting value and the increment amount for automatic sequencing.

**Usage:**

1. Go to the sequence field settings, then to the "Auto Increment Settings" section.
2. Two fields will appear for entering the starting value and the increment amount you want to use for automatic sequencing.
3. Enter the starting value, which will be the initial value for the sequence.
4. Enter the increment amount.

**Simple Example:**

In an employee database, you may have a sequence field representing the employee number. Using the "Auto Increment Settings" feature, you can specify the starting and increment values for the automatic sequence. For example, you can set the starting value to 1000 and the increment amount to 1. When creating a new employee, the sequence number will start at 1000, and for the next employee, it will be 1001, and so on, increasing automatically with each new employee added to the database.

### Lock Field

The "Lock Field" feature represents locking the sequence field when creating a new entry. This option is enabled by default and cannot be changed.

### Hide Field

Allows users to hide the sequence field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by going to the sequence field settings you want to hide.
2. After enabling it, an additional field will appear to enter the script expression to specify the conditions for hiding the sequence field.

**Simple Example:**

When the "Subscription" toggle is enabled, an additional "Subscription Number" field will be shown. When this toggle is disabled, the field will be hidden automatically.

### Searchable

The "Searchable" feature enables the search function for the sequence field when viewing entries in the user interface. When this feature is enabled, users can search for values in this field using the search box in the entry viewing interface.

**How to use:**

1. Enable the "Searchable" feature in the sequence field settings.
2. Once the feature is enabled, the search function will be activated for this sequence field.
3. In the interfaces: When clicking the search button and entering the desired keyword in the search box, the system will also search in this field.

### Field Value Settings

This section contains the following properties:

#### Show in List

This feature allows displaying the value of the sequence field in the entry list, enabling the user to see the field value easily without having to open each entry individually.

**How to use:**

1. In the sequence field settings, open the "Field Value Settings" section, then the "Display" section to reveal the display properties.
2. Enable the "Show in List" option.

#### Primary Number

The primary number is a feature assigned to a number field in the entity, allowing you to specify the primary number to be used as the main number for the entity. When assigning the sequence field as the primary number, it will be displayed with priority over other numbers in the entity.
