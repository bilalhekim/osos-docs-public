---
title: "Map Field"
sidebar_position: 18
---

# Map Field

Adding a map field to the entity structure allows users to search and pinpoint a location on a map easily. This field displays a geographical map and enables users to select the desired location by clicking on the map.

| Name       | Description                             | Data Type  |
|------------|-----------------------------------------|------------|
| Map        | Field allows specifying a location on the map | GeoJson    |

## Advanced Settings

Clicking on the settings icon in the map field within the entity structure opens a side window for advanced settings. This window has several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Specify a name for the map field with translations in Arabic and English.
2. **Normlized Name:** Contains the Normlized Name for the map field, automatically generated from the name in English. This name can be changed and serves as a unique identifier (ID) for the field.
3. **Description:** An optional field for adding a description of the map field.
4. **Data Type:** Shows the data type stored in the map field, which in this case is GeoJson.

### Default Value

This section contains the following properties:

#### Default Value

A default value can be set for the map field when creating a new entry. The default value is set by clicking the add button in the default value field, which opens the map window to choose a location, or by using a script expression by enabling the "Advanced" option in the map field settings.

**Usage: To use a script expression:**

1. Open the map field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changes to the default value after creating the entry. Enabling this option will display another field related to the default value.
   - **Triggers:** These can be used to specify when the script expression for the default value should be applied, such as on page load, form submission, entry change, or field change.

#### Lock Field

The lock field feature allows the user to lock the map field when creating a new entry. If this option is enabled, an additional input field will appear, allowing the user to enter an optional script expression to lock the field.

**Usage:**

1. Open the map field settings.
2. Enable the lock field option.
3. After enabling, an additional field will appear where the user can enter an optional script expression specifying the condition for locking the field.
4. (Optional) If the lock field option is enabled, the user must provide a default value for the map field.

#### Hide Field

This feature allows the user to hide the map field based on a specified script expression, making it invisible when interacting with the form.

**Usage:**

1. Enable the hide field option in the map field settings.
2. After enabling, an additional field will appear for entering the script expression to hide the map field.

**Simple Example:**

When the "Subscription" checkbox is enabled, an additional "Subscription Location" input field will be shown. When this checkbox is disabled, the "Subscription Location" field will be hidden automatically.

#### Required

This feature specifies whether the map field is required to complete the form or can be left empty.

**Usage:**

1. Enable the required option in the map field settings.
2. After enabling, an additional field will appear for entering the script expression to make the map field required.

### Field Value Settings

This section contains the following properties:

#### Repeatable

The "Repeatable" property allows the same map field to be entered multiple times with different values in the same entry. Enabling this option allows users to add multiple values to the same map field within a single entry.

**Usage:**

1. Go to "Field Settings" then to "Field Value Settings" for the map field you want to make repeatable.
2. Enable the "Repeatable" property.

**Setting Minimum and Maximum Limits (Optional):**

After enabling the "Repeatable" property, two additional fields will appear where you can specify the minimum and maximum number of allowed repetitions.

**Note:** If the minimum and maximum fields are left empty, repetitions will be unlimited, allowing the user to add values to the map field without restriction.

#### Show in List

This property allows the map field value to be displayed in the list of entries, enabling the user to see the field value without opening each entry individually.

**Usage:**

1. In the map field settings, open the "Field Value Settings" section.
2. Open the "Display" section.
3. Enable the "Show in List" option.