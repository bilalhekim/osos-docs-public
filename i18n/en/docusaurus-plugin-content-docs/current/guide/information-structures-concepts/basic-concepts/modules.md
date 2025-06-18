---
title: "Modules"
sidebar_position: 1
---

# Modules

Modules are one of the fundamental elements of the platform, used to organize the program more systematically and effectively. They act like containers that hold various elements and entities that execute a specific function or task within the complete system. This structural assembly facilitates understanding how the system works and how the different elements interact with each other.

Modules are components used to group a set of related functions into an integrated unit. For example, there can be a module dedicated to task management within the system.


## Important to Know
### What Cannot Be Changed in a Module After Creation
#### The Normalized Name Field
The normalized name field is defined with a clear, standard name for the module using English characters. This design facilitates data analysis and search operations, preventing spelling and translation errors. Even if you attempt to modify its value and save the changes, the normalized name field remains fixed and retains the value entered during the module creation.

The normalized name field plays a significant role in data retrieval and export operations. Thanks to this field, you can benefit from a clear and fixed value for the module without dealing with unwanted changes. This ensures the module's stability and users' understanding of the data it represents accurately.

#### Dependencies Between Modules
A module is an independent, self-contained program that executes its functions without directly depending on other modules. However, modules can interact with each other using what is known as the virtual entity.

#### The Core Module
The core module is a default module on the platform that includes the essential entities required by the system to set up its environment effectively. The core module is created automatically in the system, and users cannot modify its information or create entities under this module, as is allowed in other system modules.

## Related Concepts
- [Entities](./entities.md)
- [Dashboards](./dashboards.md)
- [Pages](./pages.md)
- [Permissions](./permissions.md)


**Note: For more information on modules operations, see: [Modules Management](../../data-management/modules.md).**