---
title: "Other Related Concepts"
sidebar_position: 2
---

# Other Related Concepts

## Identifier
An identifier is a unique, random string generated by the system for every created object. It helps in distinguishing each object and makes it uniquely identifiable, facilitating the linking of tables and establishing relationships between them in the database.

## Normalized Field
The normalized field is a unique name automatically generated by the system (or optionally set by the user, ensuring uniqueness) for any object. The normalized field is exported with the object and preserved during import, serving as the primary identifier, unlike the identifier, which is not preserved during import and is used at the entry level.

## Programming Expressions
The platform provides an environment to create information systems without the need for complex coding, through an interactive visual interface. However, in some cases or specific requirements, programming expressions can be used to enable system administrators or authorized users to customize certain application functions. It is important to note that using programming expressions is optional and not necessary for creating applications. They offer additional flexibility and customization for users with programming expertise or those who need access to functions not available through the user interface.

## Pointers
Pointers are a set of variables that serve as a crucial tool for system administrators, indicating a variable value based on the entry's conditions. Examples include:
- **@me:** Indicates the current logged-in user and is often used in events, queries, and filters.
- **@myOrgUnit:** Similar to the previous example, this indicates the organizational unit of the current user.
- **Date-related pointers:** Such as @now, @StartofDay, @StartofMonth, @StartofWeek, @StartofYear, and @today.

## References
The platform enables the creation of information systems capable of linking data through reference fields, which connect one entry to one or more entries from another entity. This is useful for establishing relationships between data.

## Core Entities
Core entities are a significant part of the platform's fundamental structure, created automatically to manage various operations. Generally, these entities cannot be directly modified or have new fields added to them. However, administrators can adjust some of these entities by adding additional fields or customizing certain properties, reports, and queries associated with them. Core entities vary in types and roles, each playing a crucial part in the system's functionality and operational efficiency.

### Example Core Entities:

- **Posts Entity:** Contains all posts added to the system, displayed as a timeline. Used for statistics and reports on system-wide posts. This entity is non-modifiable, with entries added dynamically through external display pages with timeline views. Key fields include title, description, publication status, timeline settings, and interactions.

- **Users Entity:** Contains all users added to the system. Administrators can add users, triggering an email to the user for password creation. Fields include basic information (first name, last name, email, organizational affiliation), account information (username, role assignments), and direct manager information.

- **Groups Entity:** Lists all system groups, including user groups and those created by organizational units or roles. Useful for setting permissions and generating reports. Fields include group name, description, symbol, users, and group type.

### Additional Core Entities:
Other types include comments, comment interactions, roles, interface buttons, services, counters, publication categories, reports, organization, languages, access, notifications, and dashboards. For more details, refer to the core entities list.

## Basic Lists
Basic lists represent default values reused within the system. Some lists are essential for operations, such as service categories for creating services. They help in organizing and standardizing data entries across the platform.

## Attachments
Attachments refer to all types of files uploaded as part of any entry details. They can be used within discussion windows, as mentioned earlier.

# Related Concepts
- [Entities](../information-structures-concepts/basic-concepts/entities.md)
- [Services](../information-structures-concepts/basic-concepts/services.md)
- [Queries](../information-structures-concepts/basic-concepts/queries.md)
- [Lists](../information-structures-concepts/basic-concepts/lists.md)
