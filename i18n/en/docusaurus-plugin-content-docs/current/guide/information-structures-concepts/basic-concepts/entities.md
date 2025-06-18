---
title: "Entities"
sidebar_position: 2
---

# Entities

Entities are the primary element for storing data and can be likened to tables in databases, where they are defined in each system to represent different sections or elements. These entities allow interconnection through relationships, leading to a smooth data flow in the system and reflecting automation mechanisms within the system. An entity is often designated to represent a specific set of information or functions within the system, such as a task entity in a task management system.


## Types of Entities

### Normal Entities
These are the entities described above.

### Virtual Entities
Virtual entities are a special type of entity that are not standalone but depend on another entity, where the entries of the virtual entity consist of the entries of the primary entity it depends on. These virtual entities are divided into several types:

#### Types of Virtual Entities

#### Proxy Virtual Entity
Represents a virtual entity that allows interaction with another entity, whether inside or outside the module. It can be used to interact with a specific entity through other functions and parts within the module.

#### Joiner Virtual Entity
This type of virtual entity aggregates entries of the primary entity and the entities associated with it. It displays information of the primary entity and its related fields, including related entities within the same module.

Using these virtual entities, the system can facilitate interaction with different data and functions without needing to duplicate information. Proxy and joiner virtual entities can improve the system's user experience and make data interaction more seamless.

## Important to Know

### What Cannot Be Changed in the Entity After Creation

There are two fields in the entity that cannot be changed after creation:

#### Normalized Field
It is defined by assigning a standard and clear name to the entity using English letters. This designation helps facilitate data analysis and search operations and prevents spelling and translation errors. Even when attempting to modify its value and save the changes, the normalized field remains constant and retains the value entered during creation. This field is used in import and export operations to maintain the entity's representation.

#### Entity Type
It includes two main types: natural entity and virtual entity.

Using these two fields, the system can maintain the stability of the entity's representation and prevent undesirable changes, as well as help organize and understand the different entities within the system.

#### Entity Versions
New versions of the entity are issued when modifications are made to the entity structure or its workflow, leading to changes in the description of the acceptable data.

### Modifications Leading to a New Version
A new version of the entity is issued if any of the following modifications occur:
- Adding a required field.
- Deleting a required field.
- Adding a step to the workflow.
- Deleting a step from the workflow.
- Changing the target step for an event.
- Changing the step owner.
- Making a field multiple.
- Canceling the multiplicity of a field.

## Related Concepts

- [Entries](./entries.md)
- [Queries](./queries.md)
- [Pages](./pages.md)
- [Buttons](./buttons.md)
- [Lists](./lists.md)
- [Dashboards](./dashboards.md)
- [Reports](./reports.md)
- [Relations](./relations.md)
- [Permissions](./permissions.md)
- [Reactions](./reactions-and-automation.md)
- [Fields](./fields.md)
- [Workflows](./workflows.md)
- [Timelines](./timeline.md)

**Note: For more on entities operations, see: [Entities Management](../../data-management/entities.md)**