---
title: "Views"
sidebar_position: 5
---

# Views Settings

## Entries Listing {#entries-listing}
### Display Methods {#views-faces}
#### Table {#table}
The admin user can display entries as a table by:
1. Enabling **Entries List View**.
2. Enabling the **Table** option in the view selection menu.
3. When the **Table** option is enabled, the following fields appear:
   1. Table Columns (Mandatory): Specify the fields to be displayed as table columns in the final view (at least one field must be selected).
   2. Allow Field Changes (Optional): The admin can enable the option to allow field changes.

Note: The admin can set the table view as the default by selecting **Default Value** so that this view appears as the initial display.

#### Calendar {#calendar}
The admin user can display entries as a calendar by:
1. Enabling **Entries List View**.
2. Enabling the **Calendar** option in the view selection menu.
3. When the **Calendar** option is enabled, the following fields appear:
   1. Primary Title (Mandatory): Select a text field from the entity to appear as the main title in the calendar (this field must be selected to enable the display type).
   2. Secondary Title (Optional): Select a text field from the entity to appear as the secondary title in the calendar.
   3. Image/File (Optional): Select an image field to appear as an image or file in the calendar.
   4. Date (Mandatory): Select a date field from the entity (this field must be selected to enable the display type).

Note: The admin can set the calendar view as the default by selecting **Default Value** so that this view appears as the initial display.

#### Cards {#cards}
The admin user can display entries as cards by:
1. Enabling **Entries List View**.
2. Enabling the **Cards** option in the view selection menu.
3. When the **Cards** option is enabled, the following fields appear:
   1. Primary Title (Mandatory): Select a text field from the entity to appear as the main title on the card (this field must be selected to enable the display type).
   2. Secondary Title (Optional): Select a text field from the entity to appear as the secondary title on the card.
   3. Image/File (Optional): Select an image field to appear as an image or file on the card.
   4. Display Additional Information (Optional): Enable this option to display metadata such as creation/update date and the name of the creator or the person who updated the entry.

Note: The admin can set the cards view as the default by selecting **Default Value** so that this view appears as the initial display.

#### Kanban {#kanban}
The admin user can display entries as a Kanban board by:
1. Enabling **Entries List View**.
2. Enabling the **Kanban** option in the view selection menu.
3. When the **Kanban** option is enabled, the following fields appear:
   1. Primary Title (Mandatory): Select a text field from the entity to appear as the main title on the card (this field must be selected to enable the display type).
   2. Secondary Title (Optional): Select a text field from the entity to appear as the secondary title on the card.
   3. Image/File (Optional): Select an image field to appear as an image or file on the card.
   4. Category (Mandatory): Select a classification field from the entity to appear as columns in the Kanban board (this field must be selected to enable the display type).
   5. Main Reference (Optional): Select a reference field from the entity to appear as the main reference on the card.
   6. Subcategory (Optional): Select a classification field from the entity to appear as a subcategory in the Kanban board.
   7. Date (Optional): Select a date field from the entity to appear as a date on the card.
   8. Kanban Columns (Mandatory): To choose the columns, first fill in the classification field so that the classification values appear for selecting the columns to be displayed in the Kanban board (at least one value must be selected).
   9. Display Additional Information (Optional): Enable this option to display metadata such as creation/update date and the name of the creator or the person who updated the entry.

Note: The admin can set the Kanban view as the default by selecting **Default Value** so that this view appears as the initial display.

#### Timeline {#timeline}
To display entries as a timeline, the admin must first add the timeline settings in the entity modification (for more information, see: [Timeline](./timeline.md)). After enabling the timeline via the entity, the admin can display entries as a timeline by:
1. Enabling **Entries List View**.
2. Enabling the **Timeline** option in the view selection menu.
3. When the **Timeline** option is enabled, the following fields appear:
   1. Allow Publishing/Unpublishing Posts (Optional): Enable this option to allow anyone with access to the view to publish/unpublish the post (entry).

Note: The admin can set the timeline view as the default by selecting **Default Value** so that this view appears as the initial display.

#### Tree {#tree}
To display entries as a tree, the admin must first add a reference field and set the source to the same entity, then enable the loop prevention option. The admin can display entries as a tree by:
1. Enabling **Entries List View**.
2. Enabling the **Tree** option in the view selection menu.
3. When the **Tree** option is enabled, the following fields appear:
   1. Reference Field (Mandatory): The admin must select the previously created reference field that represents a reference to the same entity.
   2. Primary Title (Mandatory): Select a text field from the entity to appear as the main title on the card (this field must be selected to enable the display type).
   3. Secondary Title (Optional): Select a text field from the entity to appear as the secondary title on the card.
   4. Image/File (Optional): Select an image field to appear as an image or file on the card.
   5. Main Reference (Optional): Select a reference field from the entity to appear as the main reference on the card.

Note: The admin can set the tree view as the default by selecting **Default Value** so that this view appears as the initial display.

#### Mini Cards {#mini-cards}
To add [Counters](../information-structures-concepts/basic-concepts/counters.md), the admin can add them by:
1. Enabling **Entries List View**.
2. Enabling the **Mini Cards** option in the view selection menu.
3. When the **Mini Cards** option is enabled, the following fields appear:
   1. Primary Title (Mandatory): Select a text field from the entity to appear as the main title on the card (this field must be selected to enable the display type).
   2. Secondary Title (Optional): Select a text field from the entity to appear as the secondary title on the card.
   3. Image/File (Optional): Select an icon field to appear as an icon on the card.
   4. Date (Optional): Select a date field from the entity to appear as a date on the card.

**Note: To fill the fields in all views, the fields must be specified in the display information (for more information on display information, see: [View Concept](../information-structures-concepts/basic-concepts/views.md)).**

### Filtering Options {#filtering}
The admin user can enable the filtering option to allow filtering of entry results based on certain conditions, making it easier for the end user to search for the desired entries by:
1. Enabling **Entries List View**.
2. Enabling the **Allow Search** option.
3. Enabling the **Allow Filters** option.

#### Allowing Entry Meta-Data Filters

The admin user can enable the option to allow the end user to filter by entry Meta-Data fields, which include:  
(Created By, Creation Date, Updated By, Update Date, Entry ID) by following these steps:

1. Enable **Display Entries List**.  
2. Enable **Allow Search** option.  
3. Enable **Allow Filters** option.  
4. Enable **Allow Entry Meta-Data Filters** option.

#### Allowing Entry Meta-Data Details Filters

The admin user can enable the option to allow the end user to filter by entry description details, which include all fields related to **Created By**, by following these steps:

1. Enable **Display Entries List**.  
2. Enable **Allow Search** option.  
3. Enable **Allow Filters** option.  
4. Enable **Allow Entry Meta-Data Filters** option.  
5. Enable **Allow Entry Meta-Data Details Filters** option.

### Allowing Current Step Filters

The admin user can enable the option to allow filtering by the current step, which includes the following fields:  
(Current Step, Current Step Owner, Current Step Primary Owner, Arrival Date to Current Step, Current Primary Step, Additional Step) by following these steps:

1. Enable **Display Entries List**.  
2. Enable **Allow Search** option.  
3. Enable **Allow Filters** option.  
4. Enable **Allow Current Step Filters** option.

### Allowing Previous Step Filters

The admin user can enable the option to allow filtering by the previous step, which includes the following fields:  
(Previous Steps, Previous Step Owners, Primary Owners of Previous Steps, Additional Steps, Execution Duration) by following these steps:

1. Enable **Display Entries List**.  
2. Enable **Allow Search** option.  
3. Enable **Allow Filters** option.  
4. Enable **Allow Previous Step Filters** option.


### Saving Queries {#saving-queries}
The admin user can enable the option to save the queries and filters created by the end user by:
1. Enabling **Entries List View**.
2. Enabling the **Allow Search** option.
3. Enabling the **Allow Filters** option.
4. Enabling the **Allow Saving Queries** option.

### Creating Lists {#collections}
The admin user can enable the option to create a list for entries based on the end user's permissions and use the collection by:
1. Enabling **Entries List View**.
2. Enabling the **Allow Creating List** option.

(For more information on lists, see: [Lists](./lists.md)).

### Obsolete Entries {#obsoletes}
The admin user can enable the option to view obsolete entries that need updating by:
1. Enabling **Entries List View**.
2. Enabling the **Show Obsolete Entries** option.

### Archived Entries {#archived}
The admin user can enable the option to view archived entries by:
1. Enabling **Entries List View**.
2. Enabling the **Show Archived Entries** option.

### "Default Sorting":
1. Ensure that the **Display Entries** option is enabled within the view settings.  
2. In the **Display Entries List** section, the **Sort** option will appear.  
3. The default sorting value is the **Order Field**, with an ascending direction by default. You can change this default value.  
4. Add the fields you want to use for sorting. The options include all fields selected at the view level as well as the entry's additional information fields.  
5. Set the sorting direction: the available options are **Ascending** and **Descending**, with **Descending** being the default.

### Search First {#search-first}
The admin user can enable the search-first option to allow

 filtering before displaying entries by:
1. Enabling **Entries List View**.
2. Enabling the **Search First** option.
3. When the **Search First** option is enabled, the following fields appear:
   1. First Filter (Mandatory): The admin must select the field to be used as the basis for filtering so that the end user can filter based on the selected field before displaying results.
   2. Second Filter (Optional): The admin can select another field along with the first field to be used as the basis for filtering so that the end user can filter based on the selected fields before displaying results.
   3. Third Filter (Optional): The admin can select another field along with the first field to be used as the basis for filtering so that the end user can filter based on the selected fields before displaying results.
   4. Fourth Filter (Optional): The admin can select another field along with the first field to be used as the basis for filtering so that the end user can filter based on the selected fields before displaying results.
   5. Auto-fill Fields When Creating New Entry (Optional): After selecting the filters, the auto-fill fields option can be enabled so that the new entry is filled with the pre-selected filter values.

### "Quick Filters":

1. Ensure that the **Show Entries List** option is enabled within the view settings.  
2. In the **Display Entries List** section, the **Quick Filters** section will appear, displaying all quick queries added to the entity.  
3. Select the specific quick filters you want to make available to the end user as quick filters.  
4. After selecting the quick filters, you can choose one of them in the **Applied Quick Filters** option to be applied by default to the entries.

### Entry Classification Styles

When **Display Entries List** is enabled, the user will see a section titled **"Entry Classification Styles"**.  
The user can select the style to be applied by default upon opening the view using the **"Selected Option"**, which contains a list of all available styles, and can select one or more styles.  

Additionally, the user can enable the **"Allow Edit"** option to allow end users to change the applied style.  
The user can also select which styles are allowed to be changed using the **"Available Options"**.  

As a result, the end user will see a new option in the view called **Styles**, and the styles will be clearly applied to the entries.  
When the user opens the **"Style"** menu, a list of grouped and individual styles configured in the view will appear, allowing them to activate the desired styles.


## Dashboard View {#dashboards}
The admin user can enable the dashboard view option so that the end user can view summaries and statistics related to the entity by:
1. Enabling **Dashboard View**.

Note: The **Search First** option cannot be enabled simultaneously with the dashboard view. The admin user can set the dashboard as the default view for the interface by enabling the option to make the dashboard the default page for the interface.

## Entry Details {#entry-details}
The end user can view the details of any entry by:
1. Enabling **Entry Details View**.
2. When the **Entry Details View** option is enabled, the following fields appear:
   1. Select Fields (Mandatory): The admin user must select the fields to be displayed in the entry details view for the end user.

**Note: To fill the fields, the fields must be specified in the display information first (for more information on display information, see: [View Concept](../information-structures-concepts/basic-concepts/views.md)).**

### Discussion {#discussion}
The admin user can enable the discussion option for the end user to add and interact with comments by:
1. Enabling **Entry Details View**.
2. Enabling the **Show Discussion** option.

#### Permissions for Discussions {#permissions}
The admin user can allow mentioning people by:
1. Enabling **Entry Details View**.
2. Enabling the **Show Discussion** option.
3. Enabling the **Allow Mentioning People** option.

By enabling **Allow Attachments**, the end user can attach files in the discussion. Note: When enabling attachments, at least one type of attachment must be specified, and the maximum size of the attachment must be set.

#### Scoping Access to Discussions
The admin user can control access permissions to the discussion by:
1. Enabling **Entry Details View**.
2. Enabling the **Show Discussion** option.
3. Enable the **Restrict Mentions Within View** option.  
4. When this option is enabled, a dropdown list will appear with the following options:
   - **All Users:** The end user can mention any user in the system.
   - **Based on View Permissions:** The end user can only mention users who match the view's defined permissions.
   - **Custom Mention Scope:** If you select **Custom Mention**, the system will display the **Custom Mention Scope Type** option with the following choices:
     - **Static Value:** The system will display a user selector and a group selector. Select one or more users, or one or more groups. When mentioning or searching, only the selected users and groups will be displayed.
     - **dynamic Value:** The system will display a field selector containing all fields defined in the entity (such as User field, reference field to Users entity, or reference field to Groups entity). Select one or more fields, and the users or groups listed in the selected field at the entry level will be displayed for mentions.

#### Allowed File Types
There are six types of files that the admin user can allow to be attached in discussions:
1. Word
2. PDF
3. ZIP Archive
4. RAR Archive
5. All Images
6. MP4 Videos

The admin user can specify the allowed attachments by:
1. Enabling **Entry Details View**.
2. Enabling the **Show Discussion** option.
3. Enabling the **Allow Attachments** option.
4. Selecting the attachment from the **Attachment Type** list.

### Entry History Log
The admin user can show the entry history and modifications made to the entry in the entry details page by:
1. Enabling **Entry Details View**.
2. Enabling the **Show Entry History** option.

After enabling the **Show Entry History** option, the user can view operations on the entry in the history section of the view and specify the types of operations by enabling the following options:
1. Show Modifications: Allows displaying all modifications made to the entry.
2. Show Who Made Modifications: Allows displaying modifications and who made them.
3. Show Reactions: Allows displaying reactions made on the entry.
4. Show Reaction Details: Allows displaying reactions, who made them, and the date of reaction.

### Show Workflow Path

The system allows administrators to enable the **Show Workflow Path** option when enabling the **Display Entry Details** feature.  
This option allows the end user to view the workflow path of the entry when viewing its details.

#### Controlling the Display of Step Owner Name

Administrators can control how the step owner name is displayed within the workflow diagram by enabling the **Display Step Owner** option.  
The user must select one of the following scopes:

- **All:**  
  The system will display the owners of the current, future, and previous steps.

- **Owned by User:**  
  The system will display only the steps where the current user is the owner.

**Additional Notes:**  
1. If the scope is set to **Owned by User** and the step is assigned to a group that the user is not a member of, the step owner names will be hidden.  
2. Steps where the current user is a member of the group will appear, but the names of other group members will be hidden.


### Navigating Between Entries
The admin user can allow the end user to navigate between entries without returning to the entries page by:
1. Enabling **Entry Details View**.
2. Enabling the **Quick Navigation Between Entries** option.

### Show Emails

After enabling **Display Entry Details**, administrators can enable the **Show Emails** option.  
This option allows the end user to view emails related to the entry when viewing its details, based on the available display options.

**Available Display Options:**

- **UI Integration Emails:** Emails sent via UI reactions. The user can enable one of the following options:
  - **All Emails:** Displays all sent emails without conditions.
  - **Sent by User:** Displays only emails sent by the current user.
  - **Received by User:** Displays only emails addressed to the current user.
    
- **Background Integration Emails:** Emails sent via background reactions. The user can enable one of the following options:
  - **All Emails:** Displays all emails without conditions.
  - **Sent by User:** Displays only emails sent by the current user.
  - **Received by User:** Displays only emails addressed to the current user.


### Relations

By enabling **Show Relations**, the end user can view relations in the entry details, depending on the selected display method.  
Administrators can enable relations by following these steps:

1. Enable the required inbound relation.  
2. Select the associated view.  
3. After enabling the relation, a **"Display As"** option will appear next to the relation.  
4. Choose one of the available display methods:
   - **Tab:** The relation will be displayed as a tab when opening the entry details.
   - **Sub View:** The relation will be displayed as a mini view inside the entry details, showing a list of related entries.

5. If **"Sub View"** is selected, an additional **"Display Mode"** option will appear:
   - Choose from the following:
     - **Show as Block**

### Enabling/Disabling Buttons
Buttons that will be displayed to the end user can be enabled by following these steps:
1. In the Enable/Disable Buttons section, all buttons created and published by the admin will be displayed.
2. Click on the button to be enabled.
3. If the button links to a related view (**Relation**), all available views of the related entity will be displayed.
4. Select the desired view.

### Ordering Enabled Buttons
Ordering the action buttons in the view helps the end user to display the enabled buttons based on the order used in the view, enhancing the user experience and interface browsing.
To order the buttons, follow these steps:
1. In the **Button Ordering** section, the main buttons for the system's primary actions, as well as the buttons created and enabled by the admin, will appear.
2. Drag the button to the desired new position.
3. Drop it in the new location.
4. Confirm saving changes after rearranging the buttons to ensure the changes are applied.

## Creating Entries {#creating-entries}
By enabling the **Allow Adding Entry** option, the end user can add a new entry. When this option is enabled, the fields allowed for the end user to fill out must be specified, with at least one mandatory field. Additionally, the admin must set the action the system will take after saving the entry:
1. Display Message: A message will appear to the user indicating the success of the entry. The user can write the message in the message field in both Arabic and English.
2. Return to Entries View: This action will redirect the user back to the entries view.
3. Clear Fields: This action will clear the fields after saving to create a new entry.
4. Return to Entry Details View: This action will redirect the end user to the entry details page.

## Updating Entries {#updating-entries}
By enabling the **Allow Updating Entry** option, the end user can update a previous entry. When this option is enabled, the fields allowed for the end user to fill out must be specified, with at least one mandatory field. Additionally, the admin must set the action the system will take after saving the entry:
1. Display Message: A message will appear to the user indicating the success of the update. The user can write the message in the message field in both Arabic and English.
2. Return to Entries View: This action will redirect the user back to the entries view.
4. Return to Entry Details View: This action will redirect the end user to the entry details page.

## Archiving Entries {#archiving-entries}
By enabling the **Allow Archiving Entry** option, the end user can archive a previous entry. When this option is enabled, the admin must set the action the system will take after archiving the entry:
1. Display Message: A message will appear to the user indicating the success of the archiving. The user can write the message in the message field in both Arabic and English.
2. Return to Entries View: This action will redirect the user back to the entries view.
4. Return to Entry Details View: This action will redirect the end user to the entry details page.

## Ask User For
By enabling the **Ask User For** option, administrators can select a set of fields to prompt the user for input when executing a UI event. This feature allows configuring an interactive experience where a dialog box containing the specified fields is displayed to the end user.

## Enabling Workflow Actions

This section aims to enable efficient management of workflows and reduce data access and management complexities.  
The responsible administrator can enable all or some of these permissions, allowing authorized end users to perform these actions regardless of the step owner's permissions.

### Creating a View with Special Permissions

1. Create a view for a specific entity.  
2. Ensure the entity has a defined workflow.  
3. When enabling **Edit Entry**, the system will display the **Administrative Permissions** section with checkboxes for the following actions:

   - **Edit Entry:** Displays the entry details without applying any workflow-specific requirements. The user can execute any available workflow actions.
   
   - **Execute Workflow Action on Behalf of Step Owner:** If an entry is stuck at any step other than the final step, the user can select one of the available actions, and the system will execute the action, recording the details in the entry history. The user will be registered as executing on behalf of the step's primary owner.
   
   - **End Workflow:** If the workflow is at a certain step, the user can select **End Workflow**, and the system will terminate the workflow and record the details in the workflow history.
   
   - **Move to Step:** If the workflow is at any step other than the final step, the user can select **Move to Step**, and the system will move the workflow to the selected step and record the details in the entry history.
   
   - **Return to Previous Step:** If the workflow is at any step other than the final step, the user can select **Return to Previous Step**, and the system will return to the previous step and record the details in the entry history.
   
   - **Reset Workflow:** If the workflow is at any step other than the final step, and the user selects **Reset Workflow**, the system will reset the workflow and record the details in the entry history.
   
   - **Change Temporary Step Owner:** If the workflow is at any step other than the final step, and the user selects **Change Step Owner**, a dialog box will appear to select the type of change and the new user. The system will change the step owner from the original user to the new user temporarily for this specific execution. In the next execution of the same step, the step owner will revert to the original owner. The system will record the details and the full name of the action executor in the entry history.
   
   - **Change Permanent Step Owner:** If the workflow is at any step other than the final step, and the user selects **Change Step Owner**, a dialog box will appear to select the type of change and the new user. The system will change the step owner from the original user to the new user permanently, making the new user the owner of the step in all future executions. The system will record the details and the full name of the action executor in the entry history.

   - **Note:**  
     When changing the step owner temporarily or permanently, if the workflow is reset, the step ownership will return to the original owner as defined by the workflow settings.

# Operations on Views

## Creating a View {#creating-view}

In this section, we will cover the process of creating views following specific steps.

### Creating a New View
1. Navigate to the entity you wish to create the view on.
2. Go to the views section in the entity, accessible by clicking on the **"Views"** tab.
3. Click on the **"+"** button next to **"New View"**.

### Entering Basic Information
1. In the view form, enter the required general information, such as the title and description.
2. Go to the "Access Permissions" section and specify who will have access to the view, whether authenticated users, anonymous visitors, or custom permissions.

### Completing Additional Settings
1. Complete any additional settings required for the view, such as specifying categories or view-specific options.
2. Ensure all mandatory fields are filled.
3. Once the information is complete, click on the "Save" button at the top of the page.

### Verifying the Data
1. If all mandatory fields are correctly filled, a green pop-up window will appear for a few

 seconds, indicating that the information has been successfully saved.
2. If there are errors, a red pop-up window will alert you to the issue.

### Viewing the List
1. You will be redirected to the views list after a successful save.
2. Views are grouped according to their types: Authenticated, Anonymous, or Restricted.
3. The default type is Authenticated, but you can click on other types to view additional views.

### Setting the Default View
1. To set the current view as the default, click on the **"Set Default View"** button.
2. You can also set the view as default from the view settings, specifically in the Access Permissions section, by clicking the **Set Default View** button.

## Sidebar Display
1. To pin the view to the sidebar, click on the **Pin to Sidebar** button.
2. You can also set the sidebar display behavior to closed/open/retain as explained [**here**](../information-structures-concepts/basic-concepts/views.md).

## Editing a View {#editing-view}

To edit an existing view, follow these steps:

1. Navigate to the entity you wish to edit the view for.
2. Go to the **"Views"** tab available in the entity.
3. Click on the view you want to edit from the listed views.
4. The view details page will appear. Make the desired changes to the view's information or settings.
5. After completing the edits, click on the "Save" button at the top of the page.

By following these steps, you can easily and professionally edit views. Always ensure to review and save the changes to ensure they are applied correctly.

## Publishing a View {#publishing-view}

To publish a view and make it available for display, follow these steps:

1. First, navigate to the view you wish to publish in the views list.
2. Find the **"Publish"** button and click on it.
3. After clicking **"Publish"**, the view will become available for display.
4. The view will appear in the sidebar if the **Pin to Sidebar** option is enabled in the view settings.
5. The publish view button will change to "Unpublish," allowing you to unpublish the view at any time.

By following these steps, you can easily manage the process of publishing available views.

## Deleting a View {#deleting-view}

To delete an existing view, the user must follow these steps:

1. Navigate to the entity you wish to delete a view for.
2. Go to the **"Views"** tab available in the entity.
3. Find the view you wish to delete from the listed views.
4. In the row of the view you wish to delete, find the trash icon (delete) and click on it.
5. A confirmation window will appear to verify the deletion. Click "Delete" to confirm the action.

By following these steps, the view will be permanently deleted. Always ensure to confirm your intent to delete before performing the action, as the view cannot be restored once deleted.
