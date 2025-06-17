---
title: "Queries"
sidebar_position: 7
---

# Filtering Entries
When you need to filter entries, you can use the search box on the entries listing page or use queries.

## Using the Filter Icon
If you want to set conditions for filtering entries, use the filter icon next to the search box. With this icon, you can set the following conditions:

1. **All conditions met**: When adding more than one filter condition, results that match all filter conditions will be displayed.
2. **Any condition met**: Results that match at least one filter condition will be displayed.

## Adding a Filter Condition
To add a filter condition, enter values in the following fields:

1. **Type**: You can filter either by entry fields or entry descriptions.
   - **Entry fields**: Choose the field you want to filter by, such as (Task title - Task description - Assigned to).
   - **Entry descriptions**: You can filter based on:
     1. Created by: The person who created the entry.
     2. Creation date: The date the entry was created.
     3. Updated by: The person who updated the entry.
     4. Update date: The date the entry was updated.

2. **Operation**: Specify whether you want to display entries that equal the value chosen in the type field or entries that do not equal it.

3. **Source**: Options appear based on the value chosen in the type field.
   - **Fixed**: Use this option when there is a field linked to another entity, such as the (Assigned to) field linked to the employees entity.
   - **Indicator**: Filter based on indicators.
   - **Code expression**: Enter a code expression for filtering.
   - **Variable**: Means that the field value will be taken from another field in the same entity or a related entity, such as the (Assigned to) field equals **metadata->modified by**.

By entering values in the above fields, you have created one filter condition. To add other conditions, re-enter values in the required fields.

## Filtering by Search {#by-search}
On the entries listing page, you can use the search box to type the value you want to search for. In this case, all results matching the entered value will be displayed without conditions, meaning all entries in text fields, numerical fields, email, etc., will appear.

### Allowing Search in a Specific Field {#allow-searching-in-a-field}
You can allow search in a specific field in two ways:

1. **Within Views**: When creating a view, you can enable search permission, and in this case, the search will be within the added fields only.
2. **By adding a specific field to the entity**: After adding the fields as shown in the guide, click on the settings icon next to the added field to enable the search option.

# Filtering by Query

Filtering by query is used when we want to retrieve a set of entries within the entity that meet certain conditions. A query can be one condition or more, and logical operations are used between conditions.

## Creating a Query Condition

When you click on one of the entities, several tabs will appear. By clicking on the "Query" tab, you can create and store queries.

### Field

The field here means selecting one of the entity's structure fields you want to filter entries by. You can choose fields from the structure or entry descriptions such as (Created by, Updated by, Created on, Updated on). The field represents the first part of the equation.

### Operator

The operator expresses the type of relationship between the two parts of the equation, and includes the following options: (equals, not equals, greater than or equal to, less than or equal to, ...).

### Values and Their Types

Values represent the second part of the equation in the condition and have several types:

1. **Fixed values**: The second part of the equation can be a fixed and specific value.
2. **Variable values**: The second part of the equation can be dynamic, according to the structure fields or entry descriptions.
3. **Values linked to a code expression**: The second part of the equation can be a code expression written in JavaScript to achieve a certain condition.
4. **Indicator values**: There are specific values in the system that refer to popular and frequently used values.

# Query Condition

The platform provides access to information by building a query or a set of queries to access and filter entries either once or by saving the query and reusing it when needed.

## Creating a Query Condition

To create a query, follow these steps:

1. Enter the entity.
2. Click on the "Queries" tab.
3. Click on the "Add New Query" button.

A window will appear to add the query criteria, which includes operations:

- **All conditions met** (default): Means that if there is more than one condition, all conditions must be met to return a result.
- **Any condition met**: Means that one condition is enough to return a result.

## Field {#query-criteria-field}

Specify the type of field, whether it is from the entry fields or entry descriptions, which will be the data source for the query.

### Entry Fields

These are the fields created during the [entity creation](./entities.md) and are displayed in the dropdown list according to the entity structure.

### Entry Descriptions

Entry descriptions include:

- **Created by**: The user who entered the values in the entity.
- **Creation date**.
- **Updated by**: The user who modified the entry.
- **Update date**.

## Operator {#query-criteria-operator}

The following operators are available:

### Equals

Used with all field types and means that the entry value must exactly match.

### Not equals

Used with all field types and means that the entry value must not match.

### Contains

Used with text fields and means that the entry value must contain the specified set of characters in a certain order.

### Does not contain

Used with text fields and means that the entry value must not contain the specified set of characters in a certain order.

### Starts with

Used with text fields and means that the entry value must start with a character or set of characters.

### Does not start with

Used with text fields and means that the entry value must not start with a character or set of characters.

### Like

Used with text fields and means that the entry value contains a specific pattern within the original text.

### Not like

Used with text fields and means that the entry value does not contain a specific pattern within the original text.

### Less than

Used with date or time fields and means that the entry value is less than the value being searched for.

### Less than or equals

Used with date or time fields and means that the entry value is less than or equal to the value being searched for.

### Greater than

Used with date or time fields and means that the entry value is greater than the value being searched for.

### Greater than or equals

Used with date or time fields and means that the entry value is greater than or equal to the value being searched for.

### In

Used with entity fields (user, reference, and classification) to search for records containing specific values, which can be multiple, instead of writing separate conditions for each value.

### Not in

Used with entity fields (user, reference, and classification) to search for records that do not contain specific values, which can be multiple, instead of writing separate conditions for each value.

### Empty

Used with all field types and means that the field does not contain any value.

### Not empty

Used with all field types and means that the field contains a value.


## Values and Their Types {#query-criteria-value-and-types}

Values are what is being searched for within the entries and can be of the following types:

### Fixed

The search value is entered manually and is unchangeable.

### Variable

The search value is variable and is determined by entry fields or entry descriptions.

### Indicator

The search value refers to an object in the system. For example, in the tasks application, when searching for the user assigned to a specific task, the @me indicator can be used to refer to the current user. Another example is the @today indicator with date fields, where date entries are compared with the current date when the indicator is executed.

### Code Expression

It appears with a date field and is used to search for values that are not covered by previous value types, providing system administrators with greater flexibility in customizing the search and accessing data.

## Executing the Query

After creating the query, you can execute it directly without saving it, or you can **save the query** for reuse in various places such as views, reports, reference fields, and dashboards, among others.

## Combining Query Conditions {#criteria-groups}

The platform allows you to add more than one condition in the query and combine the conditions using one of the logical relationships (and - or). This is done by selecting one of the following options:
- **All conditions met**: All conditions must be met.
- **Any condition met**: At least one condition must be met.

## Nesting Query Conditions {#criteria-group-nesting}

One of the important features in building queries on the platform is the ability to create nested query conditions and group them together with logical relationships. To do this, follow these steps:

1. After entering the entity by clicking on its name, choose the "Queries" tab.
2. Click on the "Add Query" button to display a screen for adding query conditions.
3. Add an additional condition and specify the logical relationship between conditions (all conditions met or any condition met).
4. To add a group of conditions:
    - Select "

Add Condition Group" from the "Add Condition" dropdown menu.
    - Specify the logical relationship between the query conditions (all conditions met or any condition met).
    - The fields for adding query conditions will appear.
    - You can repeat the process and add a condition group within another group.

**Note**: When creating nested query conditions, you can create a group within another group and specify the logical relationship between groups.

# Saving and Reusing Queries

This guide explains how to save and retrieve queries in the application by the administrator.

## Saving a Standard Query by the Administrator
1. Navigate to the sidebar in the application.
2. Click on the "Modules" option.
3. Choose the module that contains the entity you want to apply the query to from the list of modules.
4. Click on the desired entity within the selected module.
5. Go to the "Query" tab within the entity.
6. Click on the "Add Query" button to apply a specific query.
7. After applying the query, click on the "Save Query" button.
8. A dialog box will appear asking you to enter the query information. Enter the multilingual name of the query (minimum of 3 characters and maximum of 128 characters).
9. Click on the "Save" button to save the query in the query tab.
10. The query will be saved in the query list and will be distinguished from other queries by the "Standard Query" tag.

## Reusing a Standard Query by the Administrator
1. **In Reference Fields**: Use the query as a source for the reference field. 
2. **In Views**: Use the query as a source for the view. 
3. **In Reports**: Use the query as a source for reports. 
4. **In Summaries**: Use the query as a source for the summary.

## Saving a Quick Query by the Administrator
1. Navigate to the sidebar in the application.
2. Click on the "Modules" option.
3. Choose the module that contains the entity you want to apply the query to from the list of modules.
4. Click on the desired entity within the selected module.
5. Go to the "Query" tab within the entity.
6. Click on the "Add Query" button to apply a specific query.
7. After applying the query, click on the "Save Query" button.
8. A dialog box will appear asking you to enter the query information. Enter the multilingual name of the query (minimum of 3 characters and maximum of 128 characters).
9. Enable the "Quick Query" toggle.
10. Click on the "Save" button to save the query in the query tab.
11. The query will be saved in the query list and will be distinguished from the standard query by the "Quick Query" tag.

### Applying a Quick Query
1. From the entries listing tab.
2. Go to the "Status" list, which is a dropdown list containing additional filtering options.
3. The quick queries will appear alongside the additional filters.
4. Enable the desired status option and disable other options.
5. When a quick filter is enabled from the "Status" list, the quick filter conditions will be added to the currently applied filters and combined with an "AND" operator.
6. The filter conditions will appear in the custom filters list as disabled.

## Saving a Query with a Tag by the Administrator
1. Navigate to the sidebar in the application.
2. Click on the "Modules" option.
3. Choose the module that contains the entity you want to apply the query to from the list of modules.
4. Click on the desired entity within the selected module.
5. Go to the "Query" tab within the entity.
6. Click on the "Add Query" button to apply a specific query.
7. After applying the query, click on the "Save Query" button.
8. A dialog box will appear asking you to enter the query information. Enter the multilingual name of the query (minimum of 3 characters and maximum of 128 characters).
9. Enable the "Save with Tag" toggle.
10. A dialog box will appear asking you to enter the tag name. Enter the multilingual name of the tag (minimum of 3 characters and maximum of 128 characters).
11. Choose the tag color.
12. Click on the "Tag Group" button to display previously defined groups.
13. Enable the "New Tag Group" toggle.
14. Enter the name of the group you want to create.
15. Click on the "Save" button to save the query in the query tab.
16. The query will be saved in the query list and will be distinguished from the standard query by the "Tag Name" and "Standard Query" tags.

### Applying a Tagged Query
1. From the entries listing tab.
2. Go to the "Tag" list, which contains two options:
  - Color Frame
  - Colored Background
4. After selecting one of the above options, a list of individual or grouped defined tag names will appear.
5. Enable the desired tag.
6. The tag colors will be applied with the selected option (color frame or colored background) to the entries that meet the query conditions.

## Applying a Query {#apply-query}
1. Navigate to the sidebar in the application.
2. Click on the "Modules" option.
3. Choose the module that contains the entity you want to retrieve the query for from the list of modules.
4. Click on the desired entity within the selected module.
5. Go to the "Query" tab within the entity.
6. All saved queries within the entity will be displayed.
7. Select the desired query to apply.
8. Click on the "Apply Query" button to execute the query.
9. The entries matching the query will be displayed.

## Editing a Query {#edit-query}
1. Navigate to the sidebar in the application.
2. Click on the "Modules" option.
3. Choose the module that contains the entity you want to modify the query for from the list of modules.
4. Click on the desired entity within the selected module.
5. Go to the "Query" tab within the entity.
6. All saved queries within the entity will be displayed.
7. Click on the query you want to edit.
8. The query settings will be displayed.
9. Make the required changes to the query.
10. Click on the "Save" button to save the changes applied to the query.

## Deleting a Query {#delete-query}
1. Navigate to the sidebar in the application.
2. Click on the "Modules" option.
3. Choose the module that contains the entity you want to delete the query for from the list of modules.
4. Click on the desired entity within the selected module.
5. Go to the "Query" tab within the entity.
6. All saved queries within the entity will be displayed.
7. Select the query you want to delete.
8. Click on the delete icon next to the query name.
9. A confirmation message will appear asking "Are you sure? Once deleted, this action cannot be undone."
10. Confirm the deletion.
11. The query will be permanently deleted.


# Sorting Entries

When navigating to the entries of an entity, these entries are displayed in a table sorted by default in descending order by modification date. You can change the sorting in two ways:

## Method 1: Using the Dropdown Menu (Sort)

1. Click on the "Sort" dropdown menu next to the search box.
2. Choose the sorting from the following options:

### Sorting Direction

- **Ascending**: 
  - If sorting by "Created by", "Updated by", or a specific text field, the sorting will be alphabetical from (0 to 9) then (A to Z) then (أ to ي).
  - If sorting by "Creation Date", "Modification Date", or a date field, the sorting will be from the oldest date to the newest.

- **Descending**:
  - If sorting by "Created by", "Updated by", or a specific text field, the sorting will be alphabetical from (ي to أ) then (Z to A) then (9 to 0).
  - If sorting by "Creation Date", "Modification Date", or a date field, the sorting will be from the newest date to the oldest.

### Sort By

- **Created by**: Sort entries by the person who added the entries, in this case, all entries by the user will be grouped together.
- **Creation Date**: Sort entries by the date the entries were entered.
- **Updated by**: Sort entries by the user who modified the entry.
- **Modification Date**: Sort entries by the date the entry data was modified.
- **Sort by Entity Fields**: Select the field you want to sort entries by.

## Method 2: Using the Sort Icon in the Field Header

1. Select the field you want to sort entries by.
2. Click on the sort icon in the field header.
3. The sorting will toggle between ascending and descending.

Example: If you want to sort by the "Name" field, click on the sort icon at the top of this field to toggle the sorting between ascending and descending.

# Additional Filters

## Concept of Additional Filters

Additional filters are those that depend on the state of the entry, whether it is

 active, archived, obsolete, or non-obsolete. They can be accessed from the dropdown menu next to the filter, either from the administrator options or from the views for the end user if allowed and activated by the administrator according to granted permissions.

## How to Use Additional Filters

You can use additional filters to filter entries by their state through:

1. Going to the dropdown menu next to the filter.
2. Enabling the desired state option and disabling other options.

### Examples of Using Filters

- Enabling the "Archived" option will display only archived entries.
- Entries can be filtered by one or more of these states, such as enabling "Archived" and "Obsolete" together to display entries that match both states.

## Types of Entries by State

### Obsolete Entries {#obsolete-entries}
These are entries that no longer match the new structure or workflow of the entity.

### Valid Entries {#valid-entries}
These are entries that match the current structure and workflow of the entity.

### Current Entries {#current-entries}
These are entries present within the system in all states.

### Archived Entries {#archived-entries}
These are entries that have been archived and moved to the archive section.

### Quick Queries
These are queries saved as quick queries in the entity.
