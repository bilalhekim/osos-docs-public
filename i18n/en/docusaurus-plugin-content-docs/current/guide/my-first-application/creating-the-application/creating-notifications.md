---
title: "Notifications & Report"
sidebar_position: 4
---

# User Notifications Setup

## Sending Internal Notifications {#internal-notifications}

After creating the Task Management Application [here](../../my-first-application), let's assume we received a request to add an internal notification for users when a new task is assigned to them. To implement this, follow these steps:

1. Navigate to the Task Entity
   Begin by navigating to the Task entity that was created [here](./creating-entity.md), where we will add the reactions.

2. Enter Edit Mode
   Switch to edit mode by clicking on the three dots or from the menu in the top corner, select **Edit Entity**.

3. Go to the "Reactions" Tab

4. Add a New reaction
   Click on the **"+"** or **"Add Reaction"** button to start adding a new reaction.

5. Fill Out the Reaction Form
   A new "reactions" form will appear on a popup screen. Fill in the following fields:

   - **Trigger Name:** Provide a name for your reaction to distinguish it from others, for example: **"Send Notification to User When a New Task is Assigned"**.
   - **Event:** Select the type of event that will trigger this reaction, in this case: **"On New Entry Created"**.
   - **Filter:** Optionally, if the reaction supports filters, you can specify conditions that determine when the reaction should be executed. **In this case, we don't need it**.
   - **Action:** Choose **"Send Notification"** as the action to execute when the event occurs.

6. Add Notification Details
   When selecting **"Send Notification"** as the action, additional fields will appear to input notification details.

   - **Module:** This field is locked and pre-filled with the current module's name.
   - **Icon:** You can change the icon displayed for the notification.
   - **Channel Type:** For this case, the channel type will be **"Internal"**.
   - **Title:** Enter the title of the notification you wish to send. For example: **"New Task Assigned"**.
   - **Content:** Enter the content of the notification you wish to send. For example: **"{{x}} has assigned a new task to you."**

   **Note:** You can add special variables in the title and content by placing the variable name within double curly braces {{}} (in this case: {{x}}). Then, a section below will allow you to choose a value field for the variable from the entity fields or metadata or the current step owner (if there is a workflow). Select the **"Created By"** option found under the metadata section in the list.

   **Note:** Don't forget to add translations for the title and content by clicking the icon at the end of the input field to display a popup window containing fields for entering text in Arabic and English.

7. Define Recipients
   The recipients section allows you to specify the recipients of the notification by filling in the following fields:

   - **Source:** You can select the source from options: User, Group, or Collection. In this case, select **"User"**.
   - **Type:** Choose either a fixed or dynamic recipient. In this case, select **"Dynamic"**.
   - **Value:** A list of entity fields and metadata will be available to choose the recipient. In this case, select **"Assignee"** as defined in the entity structure.

8. Add the reaction
   Once you have completed filling out the reaction form, notification details, and defining recipients, click the button at the end of the form to add the reaction. The reaction will be added to the reactions list but not yet saved.

9. Save the reaction
   To save the new reaction, navigate to the top of the edit page and click the "Save" button to save all changes you have made in the "reactions" section, including the new reaction.

## Sending External Notifications {#external-notifications}

After creating the Task Management Application [here](../../my-first-application), let's assume we received a request to add an external notification to send an email to the user when a new task is assigned to them. To implement this, follow these steps:

1. Navigate to the Relevant Entity
   Start by navigating to the Task entity [here](./creating-entity.md) where we will add the reaction.

2. Enter Edit Mode
   Switch to edit mode by clicking on the three dots or from the menu in the top corner, select **Edit Entity**.

3. Go to the "reactions" Tab

4. Add a New reaction
   Click on the **"+"** or **"Add reaction"** button to start adding a new reaction.

5. Fill Out the reaction Form
   A new "reactions" form will appear on a popup screen. Fill in the following fields:

   - **Trigger Name:** Provide a name for your reaction to distinguish it from others, for example: **"Send Email to User When a New Task is Assigned"**.
   - **Event:** Select the type of event that will trigger this reaction, in this case: **"On New Entry Created"**.
   - **Filter:** Optionally, if the reaction supports filters, you can specify conditions that determine when the reaction should be executed. **In this case, we don't need it**.
   - **Action:** Choose **"Send Email"** as the action to execute when the event occurs.

6. Add Notification Details
   When selecting **"Send Email"** as the action, additional fields will appear to input email details.

   - **Subject:** Enter the email subject you wish to send. For example: **"New Task Assigned"**.
   - **Content:** Enter the email content you wish to send. For example: **"{{x}} has assigned a new task to you."**

   **Note:** You can add special variables in the subject and content by placing the variable name within double curly braces {{}} (in this case: {{x}}). Then, a section below will allow you to choose a value field for the variable from the entity fields or metadata or the current step owner (if there is a workflow). Select the **"Created By"** option found under the metadata section in the list.

7. Define Recipients
   The recipients section allows you to specify the recipients of the notification by filling in the following fields:

   - **Source:** You can select the source from options: User, Group, or Collection. In this case, select **"User"**.
   - **Type:** Choose either a fixed or dynamic recipient. In this case, select **"Dynamic"**.
   - **Value:** A list of entity fields and metadata will be available to choose the recipient. In this case, select **"Assignee"** as defined in the entity structure.
   - **CC:** Optionally, you can use the "CC" field to add additional recipients to the email. These recipients will receive a copy of the email. **In this case, we don't need it**.
   - **BCC:** Additionally, you can use the "BCC" field to add recipients to the email in a hidden manner. These recipients will receive a copy of the email without any other recipient seeing them. **In this case, we don't need it**.

8. Add the reaction
   Once you have completed filling out the reaction form, email details, and defining recipients, click the button at the end of the form to add the reaction. The reaction will be added to the reactions list but not yet saved.

9. Save the reaction
   To save the new reaction, navigate to the top of the edit page and click the "Save" button to save all changes you have made in the "reactions" section, including the new reaction.

## Sending Regular Reports {#regular-report}

After creating the Task Management Application [here](../../my-first-application), let's assume we received a request to send regular reports on task assignments to users. To implement this, follow these steps:

1. Navigate to the Task Entity
   Begin by navigating to the Task entity that was created [here](./creating-entity.md), where we will add the report.

2. Create a Query to Gather All Tasks Assigned to the Current User
   - Add a New Query
      - Click on the "+" button to start creating a new query.

   - Fill Out the Query Form
      - A new query form will appear on a popup screen. Fill in the following fields:
      - **Field/Type:** A list of entity fields and metadata will be available to choose the recipient. In this case, select the **"Assignee"** option in the entry fields section of the list.
      - **Operator:** Select the **"Equals"** option from the available operators.
      - **Source:** Select the **"Pointer"** option in the list.
      - **Pointers:** Select the **"@me"** pointer from the available pointers.

   - Save the Query
      - Click the "Save" button at the bottom right of the popup screen.
      - A small window with a text field will appear, enter the name of the query, for example: **"Tasks Assigned to Me"**.
      - Enter the translation by clicking the translation icon at the end of the field.
      - Click the "Save" button at the top of the window.

3. Go to the "Reports" Section
   Navigate to the "Reports" tab, which contains all the reports associated with this entity.

4. Add a New Report
   Click

 the **"+"** or **"Add New Report"** button to start creating a new report.

5. Fill Out the Report Form
   A new report creation page will appear on the screen. Fill in the following fields:
   - **Title:** Enter the title of the report you wish to send. For example: **"Assigned Tasks Report"**.
   - **Query:** Select the **"Tasks Assigned to Me"** query that you created earlier in the queries section, which will be used to gather the data for the report.
   - **Icon:** You can change the icon displayed for the report.
   - **Fields:** Select the fields you wish to appear in the report, in this case **select all fields**.

6. Design the Report
   In the "Report Design" section, you will find a list of logical fields that allow you to choose different layout options for the report, as follows:
   - **Page Header:** Enable this field.
   - **Organization Header:** Enable this field.
   - **Report Header:** Enable this field.
     When enabling the "Report Header" option, another field will appear to enter the content type, which contains two options: "Text" or "Image". Select the text option, another field will appear to enter the text, then enter the following value: **"Weekly Assigned Tasks Report"**.
   - You can also enable the following options:
   - **Page Footer**
   - **Organization Footer**
   - **Report Footer**
     Similar to the report title, when you select these options, another field will appear to enter the content type, which contains two options: "Text" or "Image". When choosing one of them, another field will appear to enter the text or a field to drop the image depending on the option you selected before.
   - **Select Report Layout:** A dropdown menu containing two options: "Vertical" or "Horizontal". Select the **"Horizontal"** option.
   
   **Note:** You can preview the report layout based on the options you selected through the small preview that appears on the right side of the page.

7. Define Access
   After designing the report and selecting the layout options, scroll down to the "Access Permissions" section and select the users and groups that can access this report. **In this case, we will ignore it**.

8. Sending Settings
In the "Sending Settings" section, you can specify how to send your reaction. The settings section contains the following fields:
   - **Timer:** Since we want to send the report regularly every Sunday from 1/07/2023 to 1/08/2023, we will use the following settings:

      - **Interval Type:** Select the **"Recurring"** option, which allows you to repeat the reaction regularly according to a specific schedule.
      - **Set Schedule:** Enter the following Cron expression: **0 0 * * 0**, this expression means that the report will be sent at midnight every Sunday.
      - **Start Date:** Enter the following start date: **1/07/2023**.
      - **End Date:** Enter the following end date: **1/08/2023**.

   - **Channel Type:** Choose the channel type to send the reaction. Currently, there is one available option which is "Send Email".

   - **Email Sending Settings:** When choosing "Send Email", additional fields will appear to input email details, as follows:
      - **Subject:** Enter the email subject you wish to send. For example: **"Assigned Tasks Report"**.
      - **Content:** Enter the email content you wish to send. For example: **"Hello {{x}}, we are pleased to share with you the weekly report on tasks assigned to you."**

      
      **Note:** You can add special variables in the subject and content by placing the variable name within double curly braces {{}} (in this case: {{x}}). Then, a section below will allow you to choose a value field for the variable from the entity fields or metadata or the current step owner (if there is a workflow). Select the **"Assignee"** option found under the entry fields section in the list.

      - **Define Recipients:**
      The recipients section allows you to specify the recipients of the notification by filling in the following fields:
         1. **Source:** You can select the source from options: User, Group, or Collection. In this case, select **"User"**.
         2. **Type:** Choose either a fixed or dynamic recipient. In this case, select **"Dynamic"**.
         3. **Value:** A list of entity fields and metadata will be available to choose the recipient. In this case, select **"Assignee"** as defined in the entity structure.
         4. **CC:** Optionally, you can use the "CC" field to add additional recipients to the email. These recipients will receive a copy of the email. **In this case, we don't need it**.
         5. **BCC:** Additionally, you can use the "BCC" field to add recipients to the email in a hidden manner. These recipients will receive a copy of the email without any other recipient seeing them. **In this case, we don't need it**.
         6. **Enable Notification:** If you want to enable notifications for the reaction when it is executed, activate this option.
         7. **Attachments:** You can add attachments to the email if necessary. **In this case, we don't need to add attachments**.

   -  **Save:**
   After configuring the sending settings and defining the recipients, scroll to the bottom of the page and click the **"Save"** button.

9. Execute the Report
   After saving the settings, click the **"Execute"** button to start executing the report based on the schedule you configured.

10. Monitor Reports
   You can monitor the execution of the regular report by navigating to the "Reports" section and looking for your report to review the results upon execution.

These are the main steps for setting up and executing a regular report for tasks assigned to the user. You can modify the settings and content according to your specific needs.

