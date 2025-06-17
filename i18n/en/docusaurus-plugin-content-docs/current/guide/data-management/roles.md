---
title: "Roles"
sidebar_position: 20
---

# Roles

Roles are fundamental elements in our system, reflecting the positions and tasks that an employee holds. They significantly contribute to defining permissions and access for various users within the system. Roles are a crucial means for organizing workflow and managing users effectively.

## Listing Roles {#list-roles}

To display the list of roles in the platform, follow these steps:

1. Click on the sidebar menu and select "Administration."
2. From the submenu that appears, click on "Organization" and then "Roles."

The list of roles will automatically appear. You can use the available tools to sort the list and change the display mode (table/cards/board). You can also use search and filter options to find specific roles. In the table view, you will find the following information for each role:
- Role name
- Role description
- Association with organizational unit
- Role type
- Role assignment type

## Creating a New Role {#add-role}

To add a new role to the system, follow these steps:
1. Navigate to the roles list.
2. Click on the "Add Role" button located at the top of the page, in the upper corner.
3. You will be taken to a form page where you need to fill in the role information.
   - **Role Name**: Enter the name of the role you wish to add.
   - **Role Description**: Enter a description for the role (optional).
   - **Association with Structure**: Choose from [Not linked to structure, Linked to one organizational unit, Linked to multiple organizational units].
   - **Role Type**: Select the role type from [Job Position or Abstract Role].
   - **Assignment Type**: Choose how this role is assigned [Repeated or Unique].
4. Once all required information is filled in, click the "Save" button. If the form is saved successfully, a green message indicating the successful save will appear. If there is an error, a red message will appear to alert you to any issues that need addressing.

## Viewing a Role {#show-role}

When viewing the details of a specific role, you will find various information about that role and its associated details. This includes:

### Details Tab

In this section, you can view specific information about the role, which includes the previously mentioned details.

### Discussion Section

In this section, users can interact and share comments related to this role. Users can write their comments and discuss any topic related to the role.

### History Section

This section displays the history of the role's creation and modifications. It documents all activities related to the role, such as detail modifications or previous additions or changes. Users can review the changes made to the role over time.

## Editing a Role {#edit-role}

When editing a specific role, you can update the information and details associated with that role. Here’s how to edit a role:
1. Navigate to the roles list through the main roles page.
2. Choose the role you want to edit from the list.
3. Click on the three dots (...) at the end of the row for the chosen role.
4. A pop-up menu will open, where you should select "Edit."
5. You will be taken to the role details editing page.
6. On this page, you can update various information related to the role, such as the role name, description, type, etc.
7. Once you have finished editing the details, click the "Save" button to save the changes you made.
8. A green confirmation message will be displayed indicating that the changes were successfully saved.
9. If there are errors or issues with the editing, a red message will appear indicating the problem. You need to fix it before saving.

## Archiving a Role {#archive-role}

Managing roles within your system may include modifying or removing roles if they are no longer needed. Archiving roles is an essential step to maintain an organized role structure in the system and ensure its relevance. To help you archive a role, please follow the steps below:

1. Log in to the system using an administrator account.
2. Navigate to the administration section and select "Organization" from the menu.
3. Choose "Roles" to access the list of roles in the system.
4. Select the role you wish to archive from the list.
5. Click on the three dots (...) at the end of the row for the selected role.
6. From the pop-up menu, click the "Archive" button.
7. A confirmation prompt will appear, asking you to confirm the archiving action. Click "Archive" if you are sure about this action.
8. The selected role will be archived in the system and will no longer be available for assignment or use.

Please make sure to review all details and considerations before confirming the archive, as this action cannot be undone.

## Role Assignment {#assignement}

When you want to manage the assignment of users to roles within the organization, you can follow these steps:

1. Open the administration menu from the main application menu.
2. Select "Organization" and then "Organizational Structure" from the available menu.
3. Click on the record of the organizational unit for which you want to manage the assignment.
4. Navigate to the "Assignment" tab, where the current role assignments within this unit are displayed.
5. Click the **+** button to add a new assignment and enter the following information.
   - **Role**: The role to which the user is assigned.
   - **Assignment Level**: The primary or additional role assigned to the user.
   - **Assignment Type**: Original assignment or new assignment.
   - **User**: The user to whom the role will be assigned.
   - **Organizational Unit**: The organizational unit to which the user is assigned (locked field).
   - **Manager**: Specify whether the user is a manager for this role or not.

## How to Control the Role Entity {#roles-entity}

Regarding the modification of the structure, views, and relationships for the roles entity, the process is consistent with how other entities in the system are interacted with. For a comprehensive understanding of these concepts, please refer to the [Entity Management](./entities.md) document.

In the "Edit Roles Entity" section, you will be able to customize the attributes, views, and relationships associated with the roles entities. This allows you to tailor the roles entity according to the specific needs and requirements of your organization. The steps involved in editing the attributes, views, and relationships of the roles entity are similar to those explained in the [Entity Management](./entities.md) document.