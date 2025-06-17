---
title: "Users"
sidebar_position: 18
---

# Users

## Adding a New User {#add-user}

To add a new user to the system, follow these steps:

1. After accessing the Users entity, click on the "Add User" button in the top-left corner of the page.
2. A new page with a form will open, where the user needs to fill in the required information.
3. In the first section, "Main Information":
   - Enter the first name.
   - Enter the middle name (if any).
   - Enter the last name*.
   - The full name will be automatically calculated.
   - Enter the date of birth.
   - Select the gender.
   - Upload a profile picture (if necessary).
   - Choose the user type as "Regular".
4. In the second section, "Account Information":
   - Enter a unique username.
   - Enter a unique email address.
   - Indicate if the user's account is associated with the organization (Yes / No)*.
   - Indicate if the user's account is not associated with the organization (Yes / No).
5. In the last section, assign the supervisor and indicate if the user is a manager or not.
6. After filling in all the required information, click the "Save" button.
7. If the form is successfully saved, a green message will appear confirming that the form has been successfully saved.
8. If an error occurs while filling out the form, a red message will appear indicating that there was an error or missing information.

Please note that fields marked with an asterisk (*) are mandatory and must be filled out.

# Adding a New Application User

To add a new application user to the platform, follow these steps:

1. After accessing the Users entity, click on the "Add User" button in the top-left corner of the page.
2. A new page with a form will open, where the user needs to fill in the required information.

3. In the first section, "Main Information":
   - Enter the first name.
   - Enter the middle name (if any).
   - Enter the last name.
   - The full name will be automatically calculated.
   - Enter the date of birth.
   - Select the gender.
   - Upload a profile picture (if necessary).
   - Choose the user type as "Application".

4. In the second section, "Account Information":
   - Indicate if the user's account is associated with the organization (Yes / No)*.
   - Indicate if the user's account is not associated with the organization (Yes / No).
   - Select the organizational unit manager.
   - Indicate if the user is a manager or not.
   
5. In the last section, "Application Information":
   - Enter the application name.
   - If the "Non-Expiring" option is enabled, the key will be temporarily valid for 30 days. If not enabled, the key will be permanently valid.
   
6. After filling in all the required information, click the "Save" button.
7. If the form is successfully saved, a green message will appear confirming that the form has been successfully saved.
8. If an error occurs while filling out the form, a red message will appear indicating that there was an error or missing information.

**Note:** The generated key should be used in external systems when integrating with the platform. Ensure the key is secured and not shared with untrusted parties.

## Listing Users {#list-users}

To display a list of users in the system, follow these steps:

1. **Access the System:** Log in to the system using your credentials.
2. **Navigate to Administration:** In the sidebar or main menu, look for and click on "Administration."
3. **Access Users:** After clicking on "Administration," a submenu will appear with several sub-items. Look for and select "Organization" then "Users" from this submenu.
4. **Users Page:** Upon selecting "Users," you will be directed to the Users entity page. Here, you will find a list of users in the system along with a set of tools to interact with this list.
   - **Display Options:** You have the flexibility to change the display type according to your preference. You can switch between table view, card view, and calendar view, depending on how you want to visualize user information.
   - **Table View:** By default, the display mode is set to table view. In this view, you will see a tabular representation of user information.
   - **Access Permissions:** It's important to note that users need appropriate permissions to access the "Administration > Users" section. If you do not have the necessary permissions, you may not be able to view this section or manage user-related information.

## Viewing User Details {#show-user}

To see the details of a user, follow these steps:

1. Go to the user list.
2. Click on the row of the user whose details you want to view.
3. The page will automatically navigate to the user details.

### "User Details" Tab

This tab displays the user's basic information as follows:
- **First Name:** The user's first name.
- **Middle Name:** The user's middle name, if any.
- **Last Name:** The user's last name.
- **Full Name:** The user's full name, which is a combination of the first, middle, and last names.
- **Date of Birth:** The user's date of birth.
- **Gender:** The user's gender (Male or Female).
- **Profile Picture:** A representative image of the user used for identification.
- **Username:** The unique username used for logging into the system.
- **Email:** The email address associated with the user.
- **Organization Account (Yes or No):** Indicates whether the user's account is associated with an organization (Yes or No).
- **Organizational Unit:** The organizational unit to which the user belongs if they have an organization account.
- **Primary Role Assignment:** The primary role the user holds within the organization.
- **Additional Role Assignment:** An additional role the user may have if they hold multiple roles within the organization.
- **Direct Manager:** The user who directly supervises this user.
- **Supervisor:** A user with supervisory permissions over this user.
- **Is Manager:** Indicates whether the user holds a managerial position (Yes or No).

### "Supervisors" Tab

This tab is used to enter and display the supervisors for this user. If you need to add a supervisor, you can click the "+" button and fill in the required information, similar to adding a new user.

### "Roles" Tab

This tab displays a list of roles assigned to this user. You can add a new role by clicking the "+" button and filling in the information in the pop-up window. We will discuss roles in detail in the next section.

### "Discussion" Section

Anyone can leave a comment or note about this user in this section. You can also tag others using "@" if you have something specific to share with them.

### "History" Section

This section shows the creation and update history of the user entry, allowing you to track significant events related to this user.

## Editing User {#edit-user}

To edit user information, follow these steps:

1. Go to the user list.
2. Select the user you want to edit from the list.
3. Click on the three dots (...) at the end of the selected user's row.
4. A submenu will open; choose "Edit."
5. The user details page will open, where you can modify the required information.
6. After making the necessary changes, click the "Save" button.

## Archiving User {#archive-user}

To archive a user account, follow these steps:

1. Log in to the platform using an administrator account.
2. Navigate to the administration section and select "Organization" from the menu.
3. Go to "Users" and select the user you wish to archive from the list.
4. Click on the three dots (...) at the end of the selected user's row.
5. In the pop-up menu, click the "Archive" button.
6. A window will appear asking you to confirm archiving the user. Click "Archive" if you are sure about this action.
7. The user will now be archived in the platform and will no longer have access to the platform's functions and data.

Ensure to verify all details and settings before confirming the archiving, as this action is irreversible.

## Resetting User Password

To reset a user's password, follow these steps:

1. Log in to the platform using an admin account.
2. Navigate to the administration section and select "Organization" from the menu.
3. Go to "Users" and select the user whose password you want to reset from the list.
4. Click on the three dots (...) at the end of the selected user's row.
5. In the pop-up menu, click the "Reset Password" button.
6. A window will appear asking you to confirm resetting the user's password. Click "Reset Password" if you are sure about this action.
7. A message will be sent to the user's account containing a link to reset the password.

## Disabling User Account

To disable a user account, follow these steps:

1. Log in to the platform using an admin account.
2. Navigate to the administration section and select "Organization" from the menu.
3. Go to "Users" and select the user whose account you want to disable from the list.
4. Click on the three dots (...) at the end of the selected user's row.
5. In the pop-up menu, click the "Disable Account" button.
6. A window will appear asking you to confirm disabling the user account. Click "Disable Account" if you are sure about this action.
7. The user account will now be disabled in the platform. If the user attempts to log in to the platform, a message will be displayed: "This account has been locked by the platform administrator

."

## Enabling User Account

To enable a user account, follow these steps:

1. Log in to the platform using an admin account.
2. Navigate to the administration section and select "Organization" from the menu.
3. Go to "Users" and select the user with the disabled account that you wish to enable from the list.
4. Click on the three dots (...) at the end of the selected user's row.
5. In the pop-up menu, click the "Enable Account" button.
6. A window will appear asking you to confirm enabling the user account. Click "Enable Account" if you are sure about this action.
7. The user account will now be enabled in the platform.

## How to Manage the Users Entity {#users-entity}

Regarding modifying the structure, views, and relationships of the Users entity, the process is consistent with how you interact with other entities in the system. For a comprehensive understanding of these concepts, please refer to the [Entity Management](./entities.md) documentation.

In the "Edit Users Entity" section, you will be able to customize the attributes, views, and relationships associated with user entities. This allows you to tailor the Users entity to meet the specific needs and requirements of your organization. The steps involved in editing the attributes, views, and relationships of the Users entity are similar to those described in the [Entity Management](./entities.md) documentation.