---
title: "Entries"
sidebar_position: 6
---

# Entries
Entries are the actual data within entities. This guide explains how to create, list, edit, archive, view, and interact with fields related to entries.

## Creating an Entry {#creating-entries}

Entries can be created in two ways:

1. **Through the Admin Interface**:
   - Navigate to the sidebar.
   - Select "Admin".
   - Choose the relevant module, then select the entity.
   - Click on the "+" icon to create a new entry.
   - Fill in the required information, such as mandatory fields.
   - Click the "Save" button.

2. **Through the End User Interface**:
   - Navigate to the sidebar.
   - Select "Views".
   - Click on "+" to add a new entry.
   - Fill in the required information.
   - Click the "Save" button.

When creating entries, pay attention to mandatory and unique fields, and adjust default values as needed.

## Listing Entries {#listing-entries}

Entries can be listed in two ways:

1. **Through the Admin Interface**:
   - Navigate to the sidebar.
   - Select "Admin".
   - Choose the relevant module and entity.
   - Select "Entries".
   - A list of entries will be displayed, and you can sort and filter them based on various criteria.

2. **Through the End User Interface**:
   - Navigate to the sidebar.
   - Select "Views".
   - Search and filter entries according to your needs.

When listing entries, you can determine the order and method of display, as well as enable search and filtering for easy access to entries.

## Creating a Draft Entry

When creating an entry within the platform, you should pay attention to mandatory and unique fields. Users must fill in the fields according to field requirements and workflow requirements (if any). The system will not save the entry until all these conditions are met. However, when creating a draft entry, no validation checks are applied.

### 1. Creating a Draft Entry in the Admin Section

1. Navigate to the entity where you want to create the entry.
2. Start creating the new entry by clicking on the "Create Entry" button.
3. Enter values in the entry fields; at least one field value is required.
4. Click the arrow next to the save button.
5. Select the "Save as Draft" option.

### 2. Creating a Draft Entry in the End User Section

1. From the sidebar, navigate to the view you have access to.
2. Ensure that the view allows "Create Draft Entry".
3. Start creating the new entry by clicking on the "Create Entry" button.
4. Enter values in the required entry fields; at least one field value is required.
5. Select the "Save as Draft" option.

### 3. Viewing Saved Draft Entries

1. From the sidebar, navigate to the required view.
2. Go to the drafts section to see the saved draft entries.
3. You can only view entries you created yourself. Other users cannot see these entries.
4. To continue filling in the fields in the entry, you can edit the draft and update the data.
5. After completing the fields, you can choose "Save" to save the changes or "Save as Draft" to keep it as a draft.

### Important Notes

- **Interactions**: Draft entries do not trigger any interactions within the system and cannot be selected in any references, lists, or incoming relationships to the entity.
- **Publishing**: Once all required fields are completed according to field requirements and workflow requirements, you can publish the entry to make it "Active", and the entry will be treated normally within the system.

## Viewing Entries {#entry-details}

There are multiple ways to view entries in the system:

1. **Through the Admin Interface**:
   - Navigate to the sidebar.
   - Select "Admin".
   - Choose the relevant module and entity.
   - View entries in various formats such as tables, kanban boards, cards, timelines, tree structures, and calendars.
   - To access entry details, click on the "..." button and select "View".

2. **Through the End User Interface**:
   - Navigate to the sidebar.
   - Select "Views".
   - View entries in the same formats available to admins, and you can view and edit details.

## Editing Entries {#editing-entries}

Entries can be edited in multiple ways:

1. **Through the Admin Interface**:
   - Navigate to the details page of the desired entry via "Admin".
   - Click on the "..." button and select "Edit".
   - Modify the required details.

2. **Through the End User Interface**:
   - Navigate to the details page of the desired entry via "Views".
   - Click on the "..." button and select "Edit".
   - Modify the required details.

Pay attention to mandatory and unique fields and default values during the editing process. Users will be provided with necessary instructions in case of errors or successful edits.

## Archiving Entries {#archiving-entries}

Entries can be archived in different ways:

1. **Through the Admin Interface**:
   - Navigate to the control panel.
   - Select the relevant module and entity.
   - Click on the "..." button at the end of the entry row.
   - Press the "Archive" button to hide the entry in the archive and update the entry list.

2. **Via Interactions**:
   - You can set up specific interactions to archive an entry upon meeting certain conditions.
   - Navigate to the entity in the control panel and add an interaction that allows archiving the entry upon meeting the conditions.

Entries can also be archived through the end user interface in the same way available in the control panel.

### Obsolete Entries

Obsolete entries are those that no longer match the new structure or workflow of the entity.

#### Handling Obsolete Entries {#handling-obsolete-entries}

Obsolete entries are handled by updating the entry to match the new version and making it usable.

# Viewing Entry Details

From the entries page within the entity, entries are displayed with some of their fields according to the chosen view. However, you can view more details about a specific entry by clicking on the entry from the entries table or the "..." icon, then selecting "View" from the dropdown menu to navigate to its details.

## Entry Details Page Layout {#details-layout-page}

Upon navigating to the entry details page, a table with two columns appears: the first contains the names of all entry fields, and the second contains the entered values for those fields. Additionally, there is a section with tabs (history - discussion - workflow if any). You can navigate between entries using the navigation buttons at the top of the page, one for the previous entry and the other for the next entry.

## Discussions {#discussions}

In the discussion tab, all previously added comments are displayed. You can add a new comment by entering the text in the text box at the bottom of the discussion tab and clicking the send icon. Once added, **comments cannot be deleted**. You can mention a user in the comment by typing **@username** to direct the comment to them.

## Attachments {#attachments}

You can add an attachment when adding a comment by clicking the attachment icon and selecting the attachment from the following types: (image - video - Word document - PDF). Wait for the file to upload, then click the send icon.

## Entry History Log {#entry-history-log}

In this tab, you can view the log of changes made to the entry, such as creation date and time, entered values, notification dates and times, and dates and times of all previous entry edits. It also shows all messages, events, and workflow actions with the user who performed the event.

## Meta Information {#meta-information}

- Meta information can be displayed in the entry details page for the end user if enabled in one of the views through the display (kanban board - cards) and enabling the option to display additional information.
- It can also be displayed when there is an interaction that makes recipients of the variable type (i.e., the field value is taken from another field within the same entity or a related entity, such as the field **Assigned to** equals **meta-data->modified by**), and it is displayed within the history tab in the details of the interaction where the meta information was displayed.

## Emails

All sent and executed email messages related to the current entry can be viewed on the entry details page by clicking on the **"Emails"** tab. The following features are available:

- **Display all emails related to the current entry**, sorted from newest to oldest.
- The following details are shown for each message:
  - **Subject**
  - **Sent Date**
  - **Recipient(s)**

### Expand and View the Message

You can click the **"Expand"** button to open the message in a dialog box displaying all of the following details:

- **To:** Names of users or groups who received the message.
- **CC:** Names of users or groups in the carbon copy.
- **BCC:** Names of users or groups in the blind carbon copy.
- **Subject:** The defined subject field text.
- **Body:** The main message content in the format specified at the time of sending.
- **Sent Date:** The date and time the message was sent.
- **Reaction Name**

## Workflow {#workflow}

When there are workflow steps for the entry, a "Workflow" tab is added to the entry details page. This tab displays all steps and shows the current step the entry is at. Completed steps are shown in green, and details of completed steps can be viewed by clicking on them, while upcoming steps are shown in gray.

## Editing the Entry {#editing-the-entry}

You can edit a task from within the details by clicking the "Edit" button at the top left corner, entering new values, and clicking the "Save" button.

## Archiving an Entry {#archiving-an-entry}

You can archive a task from within the details by clicking the arrow next to the "Edit" button at the top left corner and selecting "Archive". **This action cannot be undone**.

## Viewing the Relations {#viewing-the-relations}

When there is a relationship between two entities, and you access the details of the latest entries of the parent entity, there will be an additional tab within the entry details page that displays all entries branching from this entry.

## UI Buttons {#ui-buttons}

When adding a button for an interaction, this button is added to the entry details page. You can access it by clicking the arrow next to the "Edit" button at the top left corner and then clicking on it.