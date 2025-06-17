---
title: "Reference Field"
sidebar_position: 21
---

# Reference Field

Adding a reference field to the entity structure allows users to link the current entry to another entry in an entity or collection. The reference field is used to create relationships between entities and their related collections.

| Name      | Description                                              | Data Type      |
|-----------|----------------------------------------------------------|----------------|
| Reference | A field that allows selecting an entity/collection as a reference. | Entity         |

## Advanced Settings

Clicking on the settings icon in the reference field in the entity structure will open a side window for advanced settings of the reference field. This window displays several sections, as follows:

### Basic Settings

This section contains four fields:

1. **Field Name:** Here, you should specify a name for the reference field with translations in Arabic and English.

2. **Normlized Name:** This contains the Normlized NameNameName for the reference field, which is automatically generated from the name in English. This name can be changed and serves as a unique identifier for the reference field.

3. **Description:** Optional, can be used to add a description for the reference field.

4. **Data Type:** This shows the data type stored in the reference field, which in this case is: Entity.

### Data Source for Reference Field

The data source is a property in the reference field settings that allows you to specify the data source for the options in the dropdown list of this field. This property is used to determine the source of the data that will be fetched and displayed in the dropdown list for the user to select.

**How to use:**

1. Select the reference field for which you want to specify the data source.
2. In the reference field settings, go to the "Data Source" section.
3. Choose one of the following options as the data source for the dropdown list:
   - **Entities:** Selecting this option will display an additional field to select the entity whose entries you want to use as options for the dropdown list.
   - **Lists:** Selecting this option will display an additional field to select the "lists" whose entries you want to use as options for the dropdown list.

##### Prevent Loops

**Description:** The "Prevent Loops" feature is an important aspect of the reference field that prevents loops in relationships between entities. When the relationship between entities is self-referential (e.g., "parent" - "child" relationship), there is a possibility of creating a loop if a certain entity is chosen as a "parent" for another entity. Consequently, this entity becomes the "child" of the original entity, and so on.

**How to use:**
1. When defining the reference field between entities (e.g., a "parent" - "child" relationship), enable the "Prevent Loops" feature in the field settings.

**Scenario for Preventing Loops:**
Let's assume we have a system for tracking families and an entity "Mohammed" that has a self-referential relationship with "Salma" as a "child." To complete the relationship, "Salma" must be the "parent" of "Mohammed." By enabling the "Prevent Loops" feature, if the user tries to select "Mohammed" as the "parent" of "Salma" (after previously selecting her as a "child"), the system will prevent this relationship, as it leads to a loop.

**Benefit of "Prevent Loops":**
Loops are prevented to maintain the order and logic of relationships between entities, avoiding errors that cause interferences or complexities in data display. This feature ensures that each entry has only one relationship with other entries in a self-referential pattern, ensuring the integrity and consistency of linked data.

##### Cascade

Cascade is a feature in the reference field settings that allows you to enable cascading between two entities (building field reference values based on another reference field value). When this feature is enabled, additional fields are provided to specify the relationship between the two entities and the field to be referenced in the current entity.

**How to use:**

1. In the reference field where you want to enable cascading, go to the data source section, choose "Entities," select an entity in the next field, and the "Cascade" button will appear. Enable it.
2. In the next field, specify the type of cascade from the list (this field refers to one of the reference fields added in the current entity with which you want to build the cascade).
3. In the next field, choose the relationship on which you want to build the cascade from the available relationships list (the list is populated from the current entity's relationships with the reference field's selected entity).

**Simple Example:**

Assuming we have two fields in the tasks entity, "Direct Manager" and "Employee," both of which are reference fields to the "Users" entity, enabling cascade in the "Employee" field will, once a manager is selected, populate the list of users in the "Employee" field with the users managed by the selected manager instead of all users in the system.

#### Default Value

A default value can be set for the reference field when creating a new entry. The default value is specified by selecting a value in the default value field or using a script expression by enabling the "Advanced" button in the reference field settings.

**How to use: in case of using a script expression:**

1. Open the reference field settings.
2. Enable the "Advanced" button.
3. Enter the script expression representing the default value you want to set.
4. (Optional) You can use additional fields:
   - **Lock Field:** This can be used to prevent changing the default value after creating the entry. When this option is enabled, another field will appear for the default value.
   - **Triggers:** These can be used to specify when the script expression for the default value is applied, such as when the page loads, the form is submitted, the entry is changed, or the field is changed.

### Lock Field

The "Lock Field" feature allows the user to lock the reference field when creating a new entry. If this option is enabled, an additional input field appears in its scope, allowing the user to enter a script expression (optional) to add a condition for locking the field.

**How to use:**

1. Open the reference field settings.
2. Enable the "Lock Field" feature.
3. After enabling, an additional field will appear. In this field, the user can enter a script expression (optional) to define the condition that must be met to lock the reference field.
4. (Optional) If the "Lock Field" option is enabled, the user must provide a default value for the reference field.

### Hide Field

Allows the user to hide the reference field based on a specified expression, making it invisible to the user when interacting with the form.

**How to use:**

1. Enable the "Hide Field" feature by navigating to the reference field settings that you want to hide.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for hiding the reference field.

**Simple Example:**

When the "Subscription" toggle field is enabled, an additional "Subscription Type" reference field will be shown. When this toggle is disabled, it will be automatically hidden.

#### Required

Specifies whether the reference field is required to complete the form or can be left empty.

**How to use:**

1. Enable the "Required" feature by navigating to the reference field settings that need to be completed.
2. After enabling it, an additional field will appear to enter the script expression that defines the conditions for making the reference field required.

### Searchable

The "Searchable" feature allows enabling the search function in the reference field when displaying entries in the user interface. When this feature is enabled in the field, users can search for values in this field using the search box in the entries display interface.

**How to use:**

   1. Enable the "Searchable" feature in the reference field settings.
   2. Once enabled, the search function in this reference field will be activated.
   3. In the interfaces: Clicking the search button and entering the search term in the search box will enable the system to search in this field as well.

**Simple Example:** 

Using the "Searchable" feature in the text field, users can search by entering part of the name in the search box. The system will display all the entries containing the entered term. The system will search all searchable fields, including this field.

### Field Value Settings

This section contains the following features:

#### Multiple

When the "Multiple" feature is enabled, users can select more than one value from the available options.

**How to use:**
To enable the multiple values feature, you can follow these steps:

1. Navigate to the reference field settings.
2. Look for the "Multiple" option and enable it.
3. Once enabled, users can select more than one value from the available options.

#### Repeatable

The "Repeatable" feature represents the possibility of repeating the same reference field with different values in the same entry. When this option is enabled, users can add multiple values to the same field within a single entry.

**How to use:**

1. Navigate to "Field Settings" and then to "Field Value Settings" for the reference field you want to make repeatable.
2. Enable the "Repeatable" feature.

**Set the minimum and maximum repetition (optional):**

After enabling the "Repeatable" feature, two additional fields will appear that can be used to set the minimum and maximum number of repetitions allowed.

**Note:** If the fields for setting the minimum and maximum values are not filled, the repetition will be unlimited, allowing users to add values to the reference field indefinitely.

#### Show in List

This feature allows the reference field value to be displayed in the list of entries, enabling users to see the field value without opening each entry individually.

**How to use:

**

1. In the reference field settings, open the "Field Value Settings" section and then the "Display" section. This will show the display-related features.
2. Enable the "Show in List" option.

#### Reference Field Display

The "Reference Field Display" feature allows you to choose how the reference field is displayed, either as a list or in a tree structure. This hierarchical organization makes it easier for users to understand the relationships between entries.

**How to define the reference field and specify the display method:**

1. **Define the reference field properties:**
   - **Field Name:** Enter a suitable name for the reference field.
   - **Linked Entity:** Choose the entity you want to link to.
   - **Prohibit Loops:** If the reference field links to the same entity, enable the "Prohibit Loops" option.

2. **Choose the display method:**
   - A "Display Method" dropdown will appear.
   - Select your preferred display method—either "List" or "Tree." The default value is "List."

3. **Save the settings:**
   - Click "Save" to confirm the reference field settings.
   - If the reference field is configured to display values in a tree structure, the data will appear in nested levels, similar to a tree.


#### Main Reference

The main reference is a feature that allows you to specify the reference that will be used as the main reference for the entity.