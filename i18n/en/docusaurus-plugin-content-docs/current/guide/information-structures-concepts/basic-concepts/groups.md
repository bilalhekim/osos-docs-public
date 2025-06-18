---
title: "Groups"
sidebar_position: 19
---

# Groups
A group is a collection of users who are gathered together based on shared criteria. Similar permissions and authorizations are assigned to the members of this group.

The process of creating groups aims to simplify the management of permissions and authorizations for users. Instead of assigning permissions to each user individually and sequentially, you can create groups and assign permissions to these groups collectively. When a user is assigned to a particular group, they automatically inherit the permissions specified for that group.

Groups help in organizing and clustering users according to their functional roles, organizational levels, or any other criteria adopted within the system. This facilitates the effective assignment of access rights and control over resources without the need to assign each user individually.

Using groups, system administrators can define different levels of permissions for various groups, thereby simplifying the management process and enhancing system security by reducing human error and avoiding the duplication of permission configurations for each user.

## Important to Know
### Types of Groups
Groups within the system can be classified into several important types that enhance the organization and management of permissions and authorizations. Here are the different types of groups:

1. **Regular Group:**
   A regular group consists of users who are grouped together based on common criteria. This group allows for the organization of users and the application of similar policies and permissions to its members. When a user is assigned to a regular group, they acquire the permissions specified for that group.

2. **Role Group:**
   A role group is a virtual group created automatically based on users who occupy the same role or function within the organization. Role groups are used to cluster users who require the same level of permissions and authorizations. For instance, there might be a group for project managers, another for employees, and another for supervisors, and so on.

3. **Organizational Unit Group:**
   An organizational unit group is also a virtual group created automatically from users who belong to the same organizational unit or department. This group is used to organize users and facilitate the application of policies and management of permissions at the department or organizational unit level.

These different types of groups enhance the effectiveness of permission and authorization management within the system, contributing to better and more organized user management and policy application.

### Difference Between Group and List
1. **Group:**
   A group is a collection of users or objects that are clustered together based on certain shared criteria, such as job role or organizational unit. Groups are used to organize and manage permissions and authorizations collectively, meaning a set of permissions can be assigned to several users at once. Groups can consist of individuals who share specified common attributes.

2. **List:**
   A list is an aggregation of values or items stored in an ordered manner. It includes different values that can be text, numbers, dates, or any other type of data. Lists are used to organize and store multiple pieces of data in a specified order. Lists can contain multiple entries that share the same data type but differ in values.

In summary, groups are used to organize and manage users or objects in the context of permissions and authorizations, while lists are used to organize and store diverse values or data in a particular order.

## Related Concepts
- [Users](./users.md)
- [Permissions](./permissions.md)
- [Lists](./lists.md)
- [Entries](./entries.md)



**Note: For more information on groups operations, see: [Groups Management](../../data-management/groups.md).**