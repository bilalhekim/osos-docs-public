---
title: "Permissions"
sidebar_position: 17
---

# Permissions

Permissions on the platform are used to define access levels and control capabilities at the unit and entity levels. They are essential for maintaining data security and organizing how users interact with available resources and information.

**The importance of permissions on the platform includes:**

1. **Data Security:** Protect data and prevent unauthorized access.
2. **Access Organization:** Facilitate management of who can access information or resources within the platform.
3. **Behavior Control:** Define the extent of interaction and control within the platform.
4. **Granular Permissions:** Allow specific permissions for certain functions without needing full access.

Understanding the concept of permissions is crucial for designing systems that ensure security and smooth operations.

## Important to Know

### Types of Permissions

1. **Admin:** Grants the user unlimited permissions to access and manage all modules and entities without restrictions within the Administration section.

2. **Developer:** Grants the user permission to create or modify all modules and entities as structures, but they cannot view the entries of any entity defined in the Administration section.

3. **Edit:** Grants the user permission to modify all modules and entities and allows them to view core entities.

4. **View:** Grants the user permission to view all modules and entities as structures, except core entities such as Users entities.

5. **None:** The user with this permission cannot access the Administration section at all. Access to specific elements is controlled through access permissions.

### Access Permissions
Access permissions are assigned in views, reports, services, and other components of the platform, allowing the holder to:

**Authenticated:** A user who is logged into the platform can access various components like views and reports, regardless of the specific permissions assigned to them.

**Anonymous:** A dedicated link can be enabled, allowing anyone, even if not registered in the system, to view the gallery or service.

**Restricted:** Specific users and groups allowed to use the gallery, service, report, etc., are defined.

## Intersection of Access Permissions and Permissions

Access permissions and general permissions work together to ensure secure and controlled access and viewing. For example, a user with "None" permission cannot view anything in the system. However, if the access permission for a gallery is set to authenticated, the user can access and view the information if they are authenticated. This shows how different permissions can interact and function in a specific context to allow or deny access.

## Related Concepts
- [Users](./users.md)
- [Modules](./modules.md)
- [Entities](./entities.md)


**Note: For more information on permissions operations, see: [Permissions Management](../../data-management/permissions.md).**