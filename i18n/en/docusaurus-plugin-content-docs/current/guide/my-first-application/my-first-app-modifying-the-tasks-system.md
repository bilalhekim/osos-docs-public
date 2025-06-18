---
title: "Modifying the Task Management Application"
sidebar_position: 7
---
# Modifying the Task Management Application

After creating the Task Management Application [here](../my-first-application/creating-the-application/creating-module.md), let's assume a request has been made to modify it so that each task can be related to a parent task. We need to display related tasks in a specific tab with an activated tree view, sorted by the creator and task status. To implement this, follow these steps:

### Adding Self-Reference to Tasks {#adding-task-self-reference}

1. **Navigate to the Tasks Entity:**
   - Go to the Tasks entity you created [here](../my-first-application/creating-the-application/creating-entity.md).
2. **Edit the Entity:**
   - Click on the three dots or the menu in the upper corner and choose **Edit Entity**.
3. **Go to the Structure Tab:**
   - Navigate to the **Structure** tab.
4. **Add a Reference Field:**
   - From the sidebar fields list, select **Reference Field**.
   - Drag and drop the field to the desired location, such as after the description field. A pop-up window will appear to specify the source of the field, select the Tasks entity itself from the drop-down list.
5. **Name the Field:**
   - Enter the field name in both languages: **Parent Task**.
6. **Set the Field as Mandatory:**
   - Enable the **Mandatory** option.
   - Note the impact this will have on old entries, as they will become obsolete, which we will address later.
7. **Save the Changes:**
   - Click the save button. A green message will appear confirming the successful save.

### Viewing Tasks in a Tree View {#viewing-tasks-in-tree-view}

1. **Edit the View:**
   - Go to the **Interfaces** tab and select the view you created [here](../my-first-application/creating-the-application/creating-views.md) and click to edit it.
2. **Add the New Field:**
   - Ensure the new field is added in the **Fields** section of the display information tab.
3. **Configure the Task List View:**
   - Go to the Task List View tab and ensure the new field is included in the list of displayed fields (if the table view option is enabled). Enable the **Tree View** checkbox, where you will set the following fields:
     - **Reference Field** = Parent Task
     - **Main Title** = Title
     - **Subtitle** = Description
     - **Image/File** = Icon
4. **Set Tree View as Default:**
   - Enable the tree view as the default display so that tasks are displayed in a tree format by default.
5. **Save the Changes:**
   - Click **Finish** in the upper corner. A green message will confirm the save.

### Reactivating Obsolete Entries {#obsolete-entries-and-upgrading-them}

Adding a mandatory field to the entity will affect old entries, making them obsolete. Follow these steps to reactivate the data:

1. **Navigate to Tasks Entity:**
   - Go to the Tasks entity from Applications, then Entities, and open the Entries tab.
2. **Display Obsolete Entries:**
   - Ensure that the status list allows the display of obsolete entries.
3. **Update Obsolete Entries:**
   - Select the obsolete entry (marked with a red triangle), open its details.
   - A message will appear indicating that the entry is obsolete and needs to be updated.
   - Click on "Update Task" in the upper corner to open the entry in edit mode with a reminder message at the top.
   - Modify the entry to assign the appropriate parent task to the **Parent Task** field.
   - Click on "Update", confirm any changes, and a green message will confirm the successful update.
4. **Repeat for Other Entries:**
   - Follow the same steps for the remaining obsolete entries.

### Adding a Subtask Relationship {#adding-a-relation}

To display subtasks in a dedicated tab, follow these steps:

1. **Navigate to Relationships:**
   - From the Applications sidebar, select Entities, then choose the Tasks entity.
2. **Add an Incoming Relationship:**
   - Select the Relationships tab, then go to the **Incoming** sub-tab.
   - Click on the **+** button to add a relationship.
   - Fill in the relationship details:
     - **Name:** Subtasks
     - **Icon:** Choose an appropriate icon.
     - **Description:** Example: "This relationship links main tasks to their related subtasks."
     - **Related Entity:** Choose Tasks from the drop-down list.
     - **Related Field:** Select Parent Task.
3. **Save the Relationship:**
   - Click on **Finish**, a green message will confirm the successful addition.
4. **Edit the  View:**
   - Go back to the view you created [here](../my-first-application/creating-the-application/creating-views.md) and click to edit it.
   - Scroll down to the **Relationship Display** tab and enable it, displaying all incoming and outgoing relationships.
   - Select the Subtasks relationship and choose this view's name from the dropdown list.
5. **Save the Changes:**
   - Click **Finish** in the upper corner. A green message will confirm the save.
6. **Test the Setup:**
   - Go to the Entries tab in the Tasks entity, open an entry, and the Subtasks tab should appear next to the task details.

### Creating a Query {#creating-a-query}

To meet the requested modifications, follow these steps to create and save a query, then use it directly or within the view.

1. **Create and Save a Query:**
   - From the Administration menu, go to Applications, then Entities, and select the Tasks entity.
   - Open the Queries tab and click on the **+** next to **All Queries** to add a new query.
   - In the pop-up window, set the following conditions:
     - Choose **All conditions are met**.
     - Select **Field** > **Entry Fields > Status** equals **New**.
     - Add another condition: **Field** > **Entry Descriptions > Created By** equals **@me**.
   - Save the query with a name, such as **My New Tasks**.
2. **Apply the Query:**
   - In the Queries tab, find the saved query and click on **Apply Query** to execute the conditions and display all new tasks created by you.
   - You can also use this query in interfaces by setting the view's **Source Display** to **Queries** and selecting this query.

### Adding a Counter {#adding-a-counter}

Counters serve as quick shortcuts to view task information from the top bar. To add counters, follow these steps:

1. **Edit the View:**
   - Go to the Interfaces tab and select the view you created [here](../my-first-application/creating-the-application/creating-views.md) and click to edit it.
2. **Add the New Field:**
   - Ensure the new field is added in the **Fields** section of the display information tab.
3. **Enable Small Cards:**
   - In the Task List View tab, enable the **Small Cards** checkbox. Configure the following fields:
     - **Main Title** = Title
     - **Subtitle** = Description
     - **Icon**: Leave it blank.
     - **Date** = Completion Date.
4. **Save the Changes:**
   - Click **Finish** in the upper corner. A green message will confirm the save.
5. **Add a Counter:**
   - From the Administration sidebar, go to **Interfaces > Counters**.
   - Click **Add Counter**, and fill in the following details:
     - **Name:** My Tasks
   - Configure the conditions to display the count of tasks created by you.
6. **Save the Counter:**
   - Click **Finish** to save the counter.

Following these steps, you should see a counter displaying the number of tasks created by you in the top bar.