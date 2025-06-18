---
title: "Fields"
sidebar_position: 3
---

# Fields

Fields are the basic units that hold data in each record or entity. Fields describe the data stored in each entry or record within the system. Fields have various properties that facilitate the organization and management of data.

## General Field Properties

### Data Types
1. **Date:**
   - Purpose: Represent dates in day/month/year format.
2. **Boolean:**
   - Purpose: Indicate true or false values.
3. **Date/Time:**
   - Purpose: Represent timestamps in day/month/year and hour/minute format.
4. **Icon:**
   - Purpose: Select and display an icon.
5. **Text:**
   - Purpose: Represent short texts, descriptions, and textual content.
6. **Number:**
   - Purpose: Represent numerical values, including integers and fractions.
7. **Time:**
   - Purpose: Represent time in hour/minute format.

### Required Field
A required field is a field that must be filled when creating or updating an entry in the system. It ensures that all data entries contain the essential information needed. For example, the "Username" field in user records might be a required field as it needs to have unique identifying information for each user.

### Unique Field
This type of field requires that the values stored in it be unique and not duplicated across entries. It is used to ensure that certain key data is not repeated in the system. For example, an "Email" field as a unique field ensures that there are no duplicate email addresses among users.

### Default Value
This property sets a default value for the field. When a new entry is created without a specified value, the default value is used as a substitute. This simplifies the process of filling out fields and ensures there is a value even if the user does not specify one. For example, the default creation date for a new record can be set to today's date.

### Repeatable
This property allows the same field to be added with different values within the same record or entry. When enabled, it allows users to add a set of different values for the same field in a single record. For instance, in a "Notes" field, enabling repetition allows the user to add multiple notes in the same record.

### Visibility and Hidden
This property controls the visibility of fields based on certain conditions. It allows showing or hiding fields depending on specific requirements or states. For example, an additional field might be shown if a certain "Type" of record is selected.

### Locked Field
This type of field prevents modification or change of the stored value. It is used to protect sensitive data or data that should not be manually altered. For instance, a creation date can be a locked field to prevent its alteration.

### Multiple Values
When this property is enabled, it allows the user to select multiple values from the available options in the field. For example, in a "Favorite Colors" field, enabling multiple values allows the user to select more than one favorite color.

## Important to Know

### What is a Block
A block field allows grouping a set of fields under one label within a unified frame. It is used to organize and group fields within a single structure. It allows users to organize the final data display, whether by displaying the content within a special tab for the block field or in the main entry view. This feature provides greater flexibility in handling data, especially when there are many fields in the entity.

If a block field is configured to be repeatable, it facilitates repeating data without needing to create a completely new entry, simplifying data organization and entry and increasing system efficiency.

### Reference Field
A reference field allows the user to link the current entry to another entry in the entity or another collection. It is used to create links and relationships between related entities and collections.

This field allows linking the current entry with another entry in the same entity or another collection, enabling the creation of relationships between different elements in the platform. It is widely used to organize and link data together, enhancing data understanding and analysis.

### Category Field
A category field allows the user to choose a value from several predefined options, which the user assigns to each entity individually. It is often used to distinguish specific statuses for each entry from others, with the ability to assign distinct colors to each value.

The main benefit of the category field is enabling the distinction between different statuses for each entry in the system. It can be used to create summaries or collections based on this field to understand different statuses or facilitate filtering and organization according to the chosen values.

## Related Concepts
- [Entities](./entities.md)
- [Lists](./lists.md)
- [Dashboards](./dashboards.md)
- [Pages](./pages.md)
- [Permissions](./permissions.md)

**Note: For more information on fields operations, see: [Fields Management](../../data-management/field-types).**