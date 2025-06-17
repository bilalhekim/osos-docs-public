---
title: "Workflow"
sidebar_position: 14
---

# Workflow 

## Creating a Workflow {#creating-workflow}
To add a workflow in the platform, follow these steps:

1. Log into the system.
2. Navigate to the entity for which you want to create a workflow.
3. Select "Edit Entity."
4. Go to the "Workflow" tab.
5. Click on "Add Workflow."
6. By default, two steps will appear: Start and End.
7. Add the required steps.
8. Click "Save."

## Adding a Step {#adding-a-step}
To add steps to a workflow in the platform, follow these steps:

1. After clicking on "Add Workflow," an icon to add a step between the Start and End steps will appear.
2. Click the icon.
3. A form to add step details will appear.
4. Enter the following details:
    - Name: Step name (mandatory field).
    - Description: Step description.
    - Primary Action: Choose the primary action for the step to transition to.
    - Enable Return Action (optional): A return action moves the step back to the previous step.
    - Enable Reject Action (optional): A reject action transitions the workflow to the end step, ending the workflow.
    - Select Step Owner:
        1. User
        2. Group
        3. Combination
    - Select User Type:
        1. Fixed
        2. Variable
        3. Previous Step Owner (only appears if the owner is a user).
    - Select the user name, group, or combination if the user type is fixed.
    - Select the field if the user type is variable.
    - Select the step name if the owner is a user and the type is previous step owner.
    - Select the user type if the owner is a group and the type is fixed:
        1. Single User
        2. All Users
    - Determine selection type:
        1. First User
        2. Take Ownership
    - Determine alternative assignment using the same steps.
    - Relative Option: Appears only if the step owner is a user:
        1. Enabling it transfers step ownership to the direct manager of the specified owner.
        2. Relationship Field: Its value is the manager.
        3. Relationship Degree: Its value is 1 (currently non-changeable).
    - Allow Custom Step Addition Option: Enabling this allows the end user to add a step to the workflow, affecting only the entry it is added to, not all entries.
5. Click "Finish."

## Adding an Action {#adding-an-action}
To add actions to workflow steps in the platform, follow these steps:

1. Click the add icon on the step.
2. Click it.
3. A form to add action details will appear.
4. Enter the following details:
    - Name: Action name (mandatory field).
    - Description: Action description.
    - Target Step: Choose the step to transition to upon executing the action:
        1. Fixed Target
        2. Relative Target
    - Primary Action Option: Enabling it shows the action as a clear button at this step (only one primary action can be enabled per step).
    - Display Message Option: Enable this option if you want to display a custom message for this action.
    - Conditional Display Option: Add a conditional expression so that this action only appears if the condition is met.

### Fixed Target {#fixed-target}
Specify a step by name from the added steps, such as direct manager approval.

### Relative Target {#relative-target}
Specify an unknown step by name:
   - First Step
   - Previous Step
   - Current Step
   - Next Step
   - Last Step

### Conditional Visibility of Action {#action-conditional-visibility}
Enable the conditional display option to add a conditional expression so that this action only appears if the condition is met.

# Step Owner Types
A workflow step owner is responsible for monitoring and performing tasks associated with a particular step in the overall workflow. This person has the authority to make decisions, take actions, and move the workflow forward at the assigned step. The role involves managing assigned tasks, ensuring their completion, and often making decisions or approvals according to workflow rules and requirements.

## Primary and Alternative Step Owner (If Variable or Relative) {#previous}

### Primary Step Owner
In this section, the primary step owner is selected at the start of executing the workflow step. The primary step owner can be chosen from the following options:
1. User
2. Group
3. Combination

#### Step Owner as a User

##### Fixed User Type:
When the primary step owner is chosen as a "User" with a fixed type, the step owner is determined in a specific and fixed manner, and the user can be selected from all available users in the system.

**To set the step owner as a "User" with a fixed type:**
1. Go to the step settings.
2. Select the step owner as "User."
3. In the "User Type" field, choose "Fixed."
4. In the "User Name" field, select the user from the dropdown list.

##### Variable User Type:
When the primary step owner is chosen as a variable user type, the step owner is determined from another field within the same entity structure being handled.

**To set the step owner as a "User" with a variable type:**
1. Go to the step settings.
2. Select the step owner as "User."
3. In the "User Type" field, choose "Variable."
4. Another field titled "Field Name" will appear, displaying a list of available fields in the entity structure (of type User or linked to the Users entity).
5. Select one of the displayed fields to be used as the primary step owner.

##### Previous Step Owner:
When the step owner is chosen as a user type "Previous Step Owner," the user can assign the step owner based on the owner of a previously executed step in the workflow.

**To set the step owner as a "User" with a previous step owner type:**
1. Go to the step settings.
2. Select the step owner as "User."
3. In the "User Type" field, choose "Previous Step Owner."
4. Another field "Step Name" will appear to select the previous step whose owner will be used for the current step.

#### Step Owner as a Group

##### Fixed Group Type:
When the primary step owner is chosen as a group with a fixed type, the user can select the group type.

**To set the step owner as a "Group" with a fixed type:**
1. Go to the step settings.
2. Select the step owner as "Group."
3. In the "Group Type" field, choose "Fixed."
4. In the "Group Name" field, select the group from the dropdown list containing all defined groups in the system.
5. Select the user type as "Single User" to assign only one user as the step owner from the selected group members.
6. Choose a value for the selection type field:
   - **First User:** The first user to join the group will be the step owner.
   - **Take Ownership:** A user within the "Single User" group can take ownership by clicking the "Take Ownership" button in the current entry's details view.
7. After selecting the selection type, choose a value for access permissions:
    - **Single User:** The user owning the step is the only one who can see the step.
    - **All Users:** All users in the group can see the step.

##### Variable Group Type:
When the primary step owner is chosen as a group with a variable type, the step owner is determined from another field within the same entity structure being handled.

**To set the step owner as a "Group" with a variable type:**
1. Go to the step settings.
2. Select the step owner as "Group."
3. In the "Group Type" field, choose "Variable."
4. Another field titled "Field Name" will appear, displaying a list of available fields in the entity structure (linked to the Groups entity).
5. Select one of the displayed fields to be used as the primary step owner.
6. Select the user type as "Single User" to assign only one user as the step owner from the selected group members.
7. Choose a value for the selection type field:
   - **First User:** The first user to join the group will be the step owner.
   - **Take Ownership:** A user within the "Single User" group can take ownership by clicking the "Take Ownership" button in the current entry's details view.
   - **Organizational Unit Manager:** Selecting this option makes the organizational unit manager the step owner.
8. After selecting the selection type, choose a value for access permissions:
    - **Single User:** The user owning the step is the only one who can see the step.
    - **All Users:** All users in the group can see the step.

##### All Users Type:
When creating a step owned by all group users, a specific approval condition for transition can be defined. The transition to the next step will not occur unless the minimum number of users, according to the specified threshold, perform the primary action.
The approval condition is displayed as a dropdown list containing:
1. Approval from all users.
2. Approval from some users (default option).

###### Transition Condition "All Users" in a Step Owned by All Users in a Group
1. When creating or modifying a step in the workflow.
2. Go to the step settings.
3. Choose "Group" as the step owner.
4. Choose "All Users" as the user type.
5. Choose "Approval from all users" as the primary action condition.
6. A list titled "Action on Failure" will appear, specifying secondary actions to be executed if the primary

 condition fails. This list contains the options:
    - **Most Chosen Secondary Action:** The system executes the most chosen secondary action by users if the primary condition fails.
    - **Primary Action**
    - **Return**
    - **Reject**

###### Transition Condition "Some Users" in a Step Owned by All Users in a Group and Setting a Follow-up Threshold

1. When creating or modifying a step in the workflow.
2. Go to the step settings.
3. Choose "Group" as the step owner.
4. Choose "All Users" as the user type.
5. Choose "Approval from some users" as the primary action condition.
6. Choose "Action on Failure" from the list.
7. Set the follow-up threshold type to "Fixed Value."
8. Enter the follow-up threshold value (default is 1).

**Note:**
Follow-up Threshold: The minimum number of users required to perform the action for the transition to occur. If the threshold is met, the action is not sent to the remaining users in the group. If the transition condition fails and there is no valid failure action, the system executes the first secondary action chosen by the first user.

### Examples

| Transition Condition          | Users Performing Primary Action  | Executed Action          |
|-------------------------------|-----------------------------------|--------------------------|
| Approval from all users       | Some users only                   | Failure action           |
| Approval from all users       | All users                         | Primary action           |
| Approval from some users      | Minimum or more users             | Primary action           |
| Approval from some users      | Less than the threshold of users  | Failure action           |

##### Previous Step Owner as a Group:
When the step owner is chosen as a group with a previous step owner type, the user can assign the step owner based on the owner of a previously executed step in the workflow.

**To set the step owner as a "Group" with a previous step owner type:**
1. Go to the step settings.
2. Select the step owner as "Group."
3. In the "Group Type" field, choose "Previous Step Owner."
4. Another field "Step Name" will appear to select the previous step whose owner will be used for the current step.
5. After selecting the step name, choose the assignment type:
   - **By Definition:** The new step will be assigned to the owner specified in the definition of the previous step.
   - **By Execution:** The new step will be assigned to the user who executed the previous step. Detailed cases for assignment by execution:
      - **Previous Step Owner is a Group - Single User - First User:** The definition is ignored, and the action is sent to the executing users. This may occur in the following cases:
         1. The manager intervened and took the action.
         2. The group changed, and the first user was modified.
         3. The primary assignment failed, and the alternative assignment was executed.
      - **Previous Step Owner is a Group - All Users:** The definition is ignored, and the action is sent to the executing users. This may occur in the following cases:
         1. The manager intervened and took the action.
         2. The group changed, and the group members were modified.
         3. The primary assignment failed, and the alternative assignment was executed.
      - **Previous Step Owner is a Group - All Users with Reassignment Option Enabled:** The definition is ignored, and the action is sent to the executing users. This may occur in the following cases:
         1. The manager intervened and took the action.
         2. Reassignment to a specific user within the group.
         3. The primary assignment failed, and the alternative assignment was executed.
      - **Previous Step Owner is a Group - All Users with Change of Ownership Option Enabled:** The definition is ignored, and the action is sent to the executing user. This may occur in the following cases:
         1. The manager intervened and took the action.
         2. Ownership of the step was taken.
         3. The primary assignment failed, and the alternative assignment was executed.

#### Step Owner as a List

##### Fixed List Type:
When the primary step owner is chosen as a list with a fixed type, the user can select the list type.

**To set the step owner as a "List" with a fixed type:**
1. Go to the step settings.
2. Select the step owner as "List."
3. In the "List Type" field, choose "Fixed."
4. In the "Assignment Type" field, choose a list from the dropdown list displaying the defined lists in the system.
5. Select the user type as either:
   - **Single User** to assign only one user as the step owner from the list members.
   - **All Users** to assign all users in the list as step owners.
6. If the user selects the "Single User" type:
7. Choose the selection type:
   - **First User:** The first user to join the combination will be the step owner.
   - **Take Ownership:** A user within the "Single User" list can take ownership by clicking the "Take Ownership" button in the current entry's details view.
8. After choosing the selection type, set the access permissions:
    - **Single User:** The user owning the step is the only one who can see the step.
    - **All Users:** All users in the group can see the step.

##### Variable List Type:
When the primary step owner is chosen as a list with a variable type, the step owner is determined from another field within the same entity structure being handled.

**To set the step owner as a "List" with a variable type:**
1. Go to the step settings.
2. Select the step owner as "List."
3. In the "List Type" field, choose "Variable."
4. Another field titled "Field Name" will appear, displaying a list of available fields in the entity structure (of type User or linked to the Users entity).
5. Select one of the displayed fields to be used as the primary step owner.
6. Select the user type as either:
   - **Single User** to assign only one user as the step owner from the list members.
   - **All Users** to assign all users in the list as step owners.
7. If the user selects the "Single User" type:
8. Choose the selection type:
   - **First User:** The first user to join the combination will be the step owner.
   - **Take Ownership:** A user within the "Single User" list can take ownership by clicking the "Take Ownership" button in the current entry's details view.
9. After choosing the selection type, set the access permissions:
    - **Single User:** The user owning the step is the only one who can see the step.
    - **All Users:** All users in the group can see the step.

##### Previous Step Owner as a List:
When the step owner is chosen as a list with a previous step owner type, the user can assign the step owner based on the owner of a previously executed step in the workflow.

**To set the step owner as a "List" with a previous step owner type:**
1. Go to the step settings.
2. Select the step owner as "List."
3. In the "List Type" field, choose "Previous Step Owner."
4. Another field "Step Name" will appear to select the previous step whose owner will be used for the current step.
5. After selecting the step name, choose the assignment type:
   - **By Definition:** The new step will be assigned to the owner specified in the definition of the previous step.
   - **By Execution:** The new step will be assigned to the user who executed the previous step. Detailed cases for assignment by execution.

### Alternative Step Owner
When the primary step owner is chosen as a variable user type or a user related to a previous step, or when the primary step owner is chosen as a group or a combination of users, an additional section called "Alternative Assignment 1" appears. This section appears with the same structure for selecting the step owner and can be repeated until the alternative step owner is chosen as a fixed user.

## Relative to Another User {#relative-to-other-user}
When this feature is enabled, two additional fields will appear: "Relationship" and "Degree of Relationship." This feature only appears when the primary step owner is chosen as "User," meaning that the owner will be another user with a relationship to the specified primary step owner.

1. **Relationship Field:**
   - After enabling the relative option, choose the relationship on which to base the relative ownership.
   
2. **Degree of Relationship Field:**
   - Determine the degree of the relationship.

**Example:**
If we have a task entity and want to choose the employee's manager as the owner for the "Assign New Task" step in the workflow, we can use the relative option. For example, if "Mohammad" is the primary owner, select "Manager" as the relative relationship with a degree of "1," making "Salma," Mohammad's direct manager, the owner of the step.

## Ad Hoc Step {#ad-hoc-step}
When this feature is enabled, the step owner at this stage of the workflow can create a temporary custom step and assign it to another user for approval before proceeding with their original step.

**Ad Hoc Step Actions:**
1. When the feature is enabled, the step owner gets permission to add an "Ad Hoc Step."
2. The step owner can choose the type of ad hoc step from two options:
   - Additional Information.
   - Additional Approval.
3. After selecting the ad hoc step type, a popup form "Create New Step" is displayed.
4. In the popup step form, the same steps previously explained for selecting the step owner (user, group, group of users

) are applied.
5. After selecting the step owner for the ad hoc step, the current step owner must click the "Create" button to add the ad hoc step as a sub-step under the current step.
6. After creating the ad hoc step, the workflow view will be updated to include the ad hoc step as a sub-step of the current step.
7. The workflow will be paused at this point until the ad hoc step owner performs the required action (such as reviewing a document and leaving a comment for the original step owner).
8. Once the ad hoc step is successfully completed, the workflow resumes automatically to continue with the original step.

## Managing Workflow Automatically Through Reactions {#workflow-automation}
The "Workflow Automation through Reactions" feature allows setting up automated actions that are executed automatically on the workflow based on reactions built within the entity.

1. Transitioning the workflow to a specific step: Assign reactions to move the workflow from one step to another based on defined criteria.
2. Executing additional actions in the workflow: Assign reactions to perform additional actions such as sending notifications or changing field values in the structure.
3. Activating exceptional actions: Use reactions to activate exceptional actions in specific cases, such as skipping certain steps based on specified requirements.

Read more about [Reactions](../../guide/information-structures-concepts/basic-concepts/reactions-and-automation).

## Workflow Requirements {#workflow-requirements}

### Compiling Model and Workflow Requirements {#compiling-requirements}
**Workflow Requirements:**
In each workflow step, a list of available fields appears, and for each field, you can select the appropriate display option from four options:
1. **Hidden:** The field will not appear at this step at all.
2. **Locked:** The field will appear at this step but cannot be modified.
3. **Editable:** The field can be modified during this step.
4. **Mandatory:** This field must be filled out before proceeding with the workflow.

**Workflow Requirements Example:**
Let's say we have a workflow for creating a report, with three steps: "Data Entry," "Data Review," and "Review Confirmation."
1. In the first step "Data Entry," choose "Hidden" for the field "Creation Date" and "Editable" for the field "User Name."
2. In the second step "Data Review," choose "Locked" for the field "Creation Date" and "Editable" for the field "User Name."
3. In the third step "Review Confirmation," choose "Locked" for the field "Creation Date," "Locked" for the field "User Name," and "Mandatory" for the field "Submit Report."

### Who Sees What? {#who-sees-who}
1. **Step Owner:**
   - Sees the item details, including its fields (based on options set in the workflow settings).
   - Sees the workflow, with the current step clearly highlighted.
   - Sees the current step details, such as the current step owner's name and the time taken to close this step.
   - Sees the previous step owners and the time taken to close those steps.
   - Sees the following steps without the ability to view their details.
   - Sees the "Primary Action for the Current Step" button with a downward arrow to view "Alternative Actions."
   - Sees the "Edit" button to edit the allowed fields in this step.
   - Sees the "Return" button to return to the previous view.

2. **Non-Owner of the Step:**
   - Sees the item details based on options set in the workflow settings.
   - Sees the workflow, with the current step highlighted.
   - Sees the previous steps and their details.
   - Sees the current step and its details.
   - Sees the following steps without the ability to view their details.
   - Sees only the "Return" button to return to the previous view without any impact on the current workflow.
