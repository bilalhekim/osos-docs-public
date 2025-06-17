---
title: "Reactions"
sidebar_position: 13
---
# Defining Entity Reactions {#defining-entity-reactions}

In the platform, entity reactions aim to perform a specific action when an event occurs at the entity level. To add a reaction, follow these steps:

1. Go to the Administration menu.
2. Select "Applications" then "Modules."
3. Find the relevant module, then go to the Entities tab and locate the specific entity.
4. Click on the menu icon (three vertical dots) at the top right of the entity card.
5. Choose "Edit Entity."
6. Navigate to the "Reactions" tab.
7. Click on "Add Reaction" to open the reaction settings screen.
8. Add a name for the reaction (a required field that supports translation).
9. Choose the event that will trigger the reaction. 
10. You can filter the event outputs using criteria.
11. Select the action to be executed when the event meets the filtering criteria. 

# Events

Events in the platform are changes that occur to entries within an entity. Based on these events, the system performs specific actions under certain conditions set by the administrator.

## Entry Created Event {#entry-created}

This event means that when a new entry is created in the entity where this reaction is defined, the system marks this creation as an event and automatically executes the programmed action.

## Entry Updated Event {#entry-updated}

This event means that when an entry in this entity is modified, the system marks this modification as an event and automatically executes the programmed action.

### Defining a Reaction with the "On Entry Update" Event

1. Define a new reaction.  
2. Select the event **"On Entry Update"**.  
3. The system will display a list of **fields** defined within the current entity.  
4. Select one or more fields from the list.  
5. When the end user changes the value of any of the selected fields, the system will trigger the reaction and execute the corresponding action.


## Entry Archived Event {#entry-archived}

This event means that when an entry in this entity is archived, the system marks this archiving as an event and automatically executes the programmed action.

## Timer Event {#timer}

The platform can link event generation to a specific time period. The timer can be:
- **One-time:** The event is generated when the timer condition is met, executing the action.
- **Repeat:** Within two time periods (daily, weekly, monthly) using a cron expression, the event is triggered whenever the condition is met.

## On Workflow Action Executed Event

This event is triggered when a workflow execution reaches a specific step that contains a predefined action selected within the reaction. Once this action is successfully executed, the associated reaction is triggered to perform the next action.

**Adding an "On Workflow Action Executed" Event:**

1. Log in as an administrator.  
2. Navigate to the desired entity > Entity Settings > Reactions tab.  
3. When adding a new reaction, select the event **"On Workflow Action Executed"**.  
4. Choose the step whose execution will trigger this event. All steps defined in the workflow of the current and related entities will be displayed.  
5. Select the specific action that should trigger the event when executed.


## On Workflow Step Reached Event {#arrival-event}

This event is generated when an entry reaches a specific step in the workflow defined by the user, executing a specific action in the system.

For more information, [click here](./workflows.md).

## On Workflow Step Exited Event {#exit-event}

This event is generated when transitioning from one step to another in the workflow, executing a specific action based on the transition option.

For more information, [click here](./workflows.md).

## Custom Event {#custom-event}

A custom event is linked to a button added to each entry's options. This event is generated when the button is pressed, triggering the programmed action.

For more information on creating the button, [click here](./buttons.md).

### Execution Indicator

The "Execution Indicator" option can be configured for a UI reaction to control how the loading indicator appears during reaction execution, improving the overall user experience.

**Steps:**

1. Log in as an administrator.  
2. Navigate to the desired entity > Entity Settings > Reactions tab.  
3. Create a new reaction and select "Custom Event".  
4. A section titled **"Execution Indicator"** will appear. Choose one of the following options:
   - **Block:** Displays a loading indicator and prevents the user from taking any action until the reaction finishes.
   - **Inform:** Displays a loading indicator but allows the user to navigate to another page.
   - **None:** No indicator is shown, and the user can freely navigate to other pages.
5. Choose the corresponding action for the selected event.  
6. Save the reaction and link it to a button.  
For more information about creating a button, [click here](../data-management/buttons.md).

### Setting Success and Failure Messages for Interface Reaction Execution

**Setting the Start Message for Reaction:**

1. Log in to the system as an administrator.  
2. Navigate to the desired entity > Entity Settings > Reactions tab.  
3. Create a new reaction and select **Custom Event** from the list of events.  
4. In the **Execution Indicator** section, select **Block**.  
5. A default message will appear under the **On Start Execution** section: "The reaction has been started successfully"  
6. Edit this message and enter the desired message to display to the end user when the reaction starts.

**Setting a Success Message for the Reaction:**

1. Follow the same steps above.  
2. A default message will appear under the **On Successful Execution** section: "The reaction has been started successfully"  
3. Edit the message and enter the desired message to display to the end user upon successful completion of the reaction.

## UI Event {#interface-event}

In this event, the system allows users to create custom UI reactions by adding UI Events that contain a set of predefined fields. When the reaction is triggered, the system displays a dialog box with the selected fields, allowing users to input the required values. This guide outlines the steps to define fields, customize their sources, and use them within actions.

**Steps**

1. Log in as an administrator.  
2. Navigate to the desired entity > Entity Settings > Reactions tab.  
3. Create a new reaction and select **Custom Event**.  
4. Enable the **Ask User for** option.  
5. Enter a title for the dialog box.  
6. Select the field source from the following options:
   - **Inline Entity:** Manually enter JSON data.
   - **View:** Select a view. Only views with "Ask the User" enabled will appear. The fields defined under that option will be shown in the dialog.
7. The user must select an action (such as Send an Email, Update Data Entry, etc.).

**Note:** The user can map the values of the fields chosen in "Ask User for" to the fields of the selected action.

**Example: Executing a Custom UI Reaction**

- A reaction (Reaction 1) is defined in the entity as a **Custom Event** with **Ask User for** enabled and the corresponding action set to **Create Entry**.
- The reaction is linked to a UI button.
- When the user clicks the button linked to Reaction 1, the system triggers the reaction.
- A dialog box appears showing the fields defined under the **Ask User for** section in the selected view.
- The user fills in the required (or optional) fields.
- Clicking "Submit" triggers the action.

**Result:** The specified action (Create Entry) is executed using the entered values.

## Reaction Success Event

This feature allows you to create sequential reactions that depend on the success of previous reactions. This guide explains how to set up a new reaction that executes when a previous reaction succeeds and how to use the results of this reaction in action settings.

### Defining a Reaction with an "Reaction Success" Event

**Defining Reaction 1:**

1. Create a new reaction named **"Reaction 1"**.  
2. Select a UI Event (e.g., Button Click).  
3. Select an action (e.g., Create Entry).

**Defining Reaction 2:**

1. Create a new reaction named **"Reaction 2"**.  
2. Choose the event **"Reaction Success"**.  
3. The system will automatically configure the reaction to align with the triggering reaction (i.e., the one whose successful execution triggers the current reaction) in terms of context.  
4. The system will display a list of all entities in the system. Select the entity that contains the triggering reaction.  
5. All defined reactions in the selected entity will be shown. Choose the desired reaction.

**Example:**

In an entity, Reaction 1 is defined, and Reaction 2 is configured to be triggered upon the success of Reaction 1.  
As an end user, when you perform an action that triggers **Reaction 1**, **Reaction 2** will automatically be triggered upon its success.

#### Results in Action Settings in Reaction 2:
1. While configuring actions in "Reaction 2," the user can choose the outputs or inputs of "Reaction 1" as a value for a field in the action within "Reaction 2."
2. Select the appropriate field from the outputs or inputs of "Reaction 1" to use in "Reaction 2."

## Export File by Template Event

This event allows users to define reactions that are triggered when files are exported. The appropriate template can be selected while defining the event. When the file is exported, the reaction is automatically triggered to execute the corresponding action.

**Example:**  
Reaction 1: The event is **"Export File"**, and the associated action is **"Send Notification"**.  
When the user exports Template "X", the system automatically sends a notification to the selected recipients to inform them that the export was completed.

## Execution Scopes

The **Execution Scopes** feature allows administrators to define where a reaction can be executed, providing greater flexibility in customizing behavior based on different contexts within the system.

**Available Options in the "Execution Scopes" List:**

- **Primary Scope:** The reaction is executed only in the primary scope.  
- **Triggering Scope:** The reaction is executed only in the scope that triggered it.  
- **Primary and Triggering Scopes:** The reaction is executed in both the primary and triggering scopes.  
- **All Except Primary Scope:** The reaction is executed in all scopes except the primary one.  
- **All Scopes:** The reaction is executed in all scopes, including the primary one.

## Filtering Reaction Inputs {#filter-reaction-input}

Filtering reaction inputs means applying a condition to the entries to which the reaction applies, executed similarly to queries. For more information on creating a query, [click here](./queries.md).
The user can use a previously saved query in the entity, and the saved queries will be displayed under the **Entry Source** option.

**Example:** If the event is creating an entry, a condition can be added so that the event is generated only when the entry is created by a specific number of users and not everyone.

## Loop Threshold

This feature allows administrators to create reactions that support conditional infinite loops, with the ability to set a loop threshold as a safety measure, based on specific conditions.

The condition is defined using a query within the reaction to determine the basis on which the loop will continue or stop.

# Actions

Platform reactions include actions that allow executing specific commands dynamically when reaction events and conditions are met.

## Action: Create Entry {#create-entry}

This action allows an admin user to automate the creation of a new entry in an entity dynamically under specific conditions. The user can select either the current entity or another entity in the system and assign values to the required fields.

### Steps to Create a Reaction That Performs a Create Entry Action:

1. Log in to the system as an administrator.  
2. Select the entity where you want to create the reaction.  
3. From the **Reactions** tab, create a new reaction or edit an existing one.  
4. Choose an event from the list of available events.  
5. Select the **"Create Data Entry"** action from the list of actions.  
6. The action name will default to the action type but can be renamed.  
7. Choose the entity in which to create the entry (current or another entity).  
8. Required fields in the target entity will appear and must be assigned values, Optional fields can be added as well.  
9. Assign values to these fields using fields from the current (source) entity.  
10. Select the value type:
    - **Manual:** The value is manually entered by the user.
    - **Pointer:** Available for reference fields pointing to users or user-type entities. Common indicators:
      - **"This Entry"**: Refers to the entry on which the reaction was triggered.
      - **"Current User"**: Refers to the user who performed the action that triggered the reaction. Useful for filling in fields like “Created By”.
    - **Field:** Select a compatible field from the source entity:
        - Optional target field → all compatible fields shown.
        - Required target field → only required compatible fields shown.
        - Repeated field with min/max → only repetition-matching fields shown.

#### If the Target Field Is a Repeated Multi-Value Field (Standalone or in Single Block):

Only fields that match the data type and repetition limits of the target field will appear.

| Scenario   | Source Field Type                                | Result                                                                                     |
|------------|--------------------------------------------------|--------------------------------------------------------------------------------------------|
| Scenario 1 | Single-value field (standalone/single block)     | Target field is filled directly with source field value.                                   |
| Scenario 2 | Single-value field in repeated block             | First block repetition’s value is used.                                                    |
| Scenario 3 | Repeated field (standalone/single block)         | First repetition of the source field is used.                                              |
| Scenario 4 | Repeated field in repeated block                 | First block → first field repetition used.                                                 |
| Scenario 5 | Multi-value field (standalone/single block)      | First value of the source field is used.                                                   |
| Scenario 6 | Multi-value field in repeated block              | First block → first value of source field used.                                            |
| Scenario 7 | Repeated multi-value field (standalone/block)    | First repetition → first value used.                                                       |
| Scenario 8 | Repeated multi-value field in repeated block     | First block → first repetition → first value used.                                         |

---

#### If the Target Field Is a Repeated Single-Value Field (Standalone or in Single Block):

Only multi-value source fields with a minimum equal to or greater than the target field’s minimum will be shown.

| Scenario   | Source Field Type                                | Result                                                                                     |
|------------|--------------------------------------------------|--------------------------------------------------------------------------------------------|
| Scenario 1 | Single-value field (standalone/single block)     | Single repetition filled using source field value.                                         |
| Scenario 2 | Single-value in repeated block                   | First block repetition’s value used for single repetition.                                 |
| Scenario 3 | Repeated single-value (standalone/block)         | All values from source are used.                                                           |
| Scenario 4 | Repeated single-value in repeated block          | First block's values used.                                                                 |
| Scenario 5 | Multi-value field (standalone/block)             | First value from source used for a single repetition.                                      |
| Scenario 6 | Multi-value field in repeated block              | First block → first value used.                                                            |
| Scenario 7 | Repeated multi-value field (standalone/block)    | First value from each repetition is used.                                                  |
| Scenario 8 | Repeated multi-value field in repeated block     | First block → first value from each repetition used.                                       |

---

#### If the Target Field Is a Required Single-Value Field (Standalone or in Single Block):

Only required source fields with exactly matching data types are shown. These must be:
- Standalone or in a single block.
- Not in a repeated block with a minimum repetition of zero.

| Scenario   | Source Field Type                                                          | Result                                                                                     |
|------------|---------------------------------------------------------------------------|--------------------------------------------------------------------------------------------|
| Scenario 1 | Required single-value (standalone/single block)                           | Source value copied directly to target.                                                    |
| Scenario 2 | Required single-value in repeated block                                   | First block's value used.                                                                  |
| Scenario 3 | Repeated field (standalone/single block)                                  | First repetition value used.                                                               |
| Scenario 4 | Repeated field in repeated block                                          | First block → first repetition value used.                                                 |
| Scenario 5 | Multi-value field (standalone/single block)                               | First value used.                                                                          |
| Scenario 6 | Multi-value field in repeated block                                       | First block → first value used.                                                            |
| Scenario 7 | Repeated multi-value field (standalone/single block)                      | First repetition → first value used.                                                       |
| Scenario 8 | Repeated multi-value field in repeated block                              | First block → first repetition → first value used.                                         |

## Update Entry Action {#update-entry}

This action helps the administration user automate the modification of an existing entry in the entity under specific conditions. The current entity or a related entity can be selected, and the fields and their values can be chosen.

## Archive Entry Action {#archive-entry}

This action helps the administration user archive a specific entry, linked entries, or entries resulting from a specific query when the reaction is triggered.

### Creating a Reaction that Archives an Entry

1. Log in to the system as an administrator.  
2. Navigate to the desired entity > Entity Settings > Reactions tab.  
3. Create a new reaction and select an event from the list of events.  
4. Choose the **"Archive Entry"** action from the list of actions:
   - The system will display a dropdown list titled **"Scope"**.
   - Select **"This Entry"**, which means the entry on which the reaction was triggered will be archived.


### Creating a Reaction that Archives a Linked Entry

1. Log in to the system as an administrator.  
2. Navigate to the desired entity > Entity Settings > Reactions tab.  
3. Create a new reaction and select **Custom Event** from the list of events.  
4. Choose the **"Archive Entry"** action from the list of actions:
   - The system will display a dropdown list titled **"Scope"**.
   - Select **"Related Entries"**.
   - The system will display a list of inbound relations defined at the entity level in the **Relation** field.
   - Select the relation whose related entries you want to archive. The system will archive the entries linked to the entry on which the reaction was triggered.


### Creating a Reaction that Archives Entries Resulting from a Query

1. Log in to the system as an administrator.
2. Select the entity where you want to create a reaction.
3. In the Reactions tab, create a new reaction or modify an existing one.
4. Select any event from the list of available events.
5. Choose the "Archive Entry" action from the list of actions:
    - The system will display a dropdown menu titled "Scope."
    - Select "Saved Query."
    - The system will display a list of saved queries defined at the entity level in the "Queries" field.
    - Select the query whose resulting entries will be archived.

## Send Notification Action {#send-notification}

This action helps the administration user send notifications within the system. It requires specifying the notification title and content and selecting the recipient from the available options (user, group, list).

## Send Email Action {#send-email}

This action helps the administration user send an email. It requires specifying the email subject and content and selecting the recipient from the available options (user, group, list, fixed).

### Sender

The system offers flexibility in defining the email sender when creating or editing reactions. The user can select the sender from several options (**System**, **Reaction Executor**, **Custom**), and the sender name will be displayed according to the selected setting.

**Steps:**

1. Select the **"Send Email"** action in the reaction settings.  
2. After defining the recipients, go to the **"Sender"** settings, where the following options will be displayed:
   - **System:** The system will be set as the default sender.
   - **Reaction Executor:** The email and username of the user who executed the reaction will be used.
   - **Custom:** Allows the user to define the sender source.

3. When **Custom** is selected, the system will display additional options to define the sender source:
   - **User:**  
     - **Static:** A list of users defined in the system will be shown. The user must select one user only.
     - **Variable:** A list of fields from the entity linked to the Users entity will be shown.
   - **Static:**  
     - **Static:** The email address is manually entered in a text field. It must be a valid email address according to standard email format.

### Attachments

The system allows sending emails with attachments that are read from fields as part of the email, enabling the end user to receive emails containing file field values as attachments.

**Steps:**

1. Select the **"Send Email"** action in the reaction settings.  
2. Enable the **Attachments** option for the email. The attachment can be either:
   - **Variable Value:** Select one of the file fields to attach its value.
   - **Static Value:** Upload a file from your device to be used as a static attachment.

## Send SMS Action {#send-sms}

This action helps the administration user send text messages. It requires specifying the message content and selecting the recipient from the available options (entity, list, fixed).

## Call External API Action {#call-external-api}

This action helps the administration user call external APIs and integrate external software by receiving and sending data. It includes various request types (GET, POST, PATCH, PUT, DELETE).

## Execute Workflow Step Action {#execute-workflow-step-action}

This action helps the administration user execute an action within workflow steps when a specific condition is met.

## Move Workflow to Step Action {#move-workflow-to-step}

This action helps the administration user move to a specific step in the workflow when a specific condition is met.

## Action: Generate File

This action allows creating reactions to perform the **"Generate File"** action based on predefined templates. The template, file retention period, and custom file name can be configured. When the reaction is triggered, the file is generated and downloaded, and the user receives a notification upon completion.

**Steps:**

1. Create a new reaction within the desired entity.  
2. Select an event from the list of events.  
3. Choose the **"Generate File"** action from the list of actions.  
4. Click the **"Template"** field. The system will display a list of all templates defined within the entity. Select the desired template from the list.  
5. Set the file retention period:
   - **Forever:** The file will be kept permanently.
   - **Specific Period:** Enter the number of days after which the file will be deleted if not used.
6. Once the template is selected, the system will display the **"Download Generated File"** option.  
7. Enable this option to customize the file name.
   - You can use placeholders to automatically generate the file name or enter a manual name.

**Example:**  
When an action triggers the reaction (e.g., a custom event), the file will be generated based on the selected template.  
Upon completion, the system will send a notification to the user indicating the file export is complete.  
The user can click the notification to download the file directly, using either the template name or the customized file name.
