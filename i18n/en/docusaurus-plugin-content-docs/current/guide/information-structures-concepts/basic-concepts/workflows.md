---
title: "Workflows"
sidebar_position: 14
---

# Workflows
A workflow is a diagrammatic model used to describe the sequence of steps and processes that need to be followed to complete a specific task in an organized and logical manner. A workflow diagram is used to simplify the interaction with the application or system and guide users through certain processes smoothly to achieve their goals efficiently and easily. The workflow diagram illustrates the context and chronological sequence of activities, decisions, and various interactions within a specific task, helping to understand, analyze, and improve work processes.

## Important to Know
### Step
A step is a fundamental element within a workflow, representing a part of the sequential actions that must be followed to achieve a specific goal in a given context. A step can be defined as a specific process or action that must be performed during the interaction with the application or system. Generally, steps are linked to a specific chronological order, representing a sequential series of actions that must be followed in a specific order to successfully complete the task.

The importance of steps in a workflow lies in several points:

1. Simplifying Interaction: Steps break down a large task into small, sequential steps, helping to simplify the interaction with the application and making it more comprehensible and easier to follow.

2. Guiding the User: By clearly and logically defining the steps, users are guided through the application process by following the specified sequence of steps.

3. Reducing Errors: By clarifying the procedures to be followed, the likelihood of errors during the use of the application is reduced.

4. Increasing Efficiency: Organizing processes into logical steps helps to increase performance efficiency and facilitate smooth transitions from one stage to another.

In summary, steps form the backbone of a workflow diagram, contributing to organization, guidance, and efficiency during interaction with the application or system.

### Action
An action is a specific task or process that needs to be executed to achieve a particular goal within the application or system. It represents the actual interactive steps that the user performs within the application.

### Owner (Primary, Alternative, Variable, Relative)
- **Primary Owner**: The person or entity primarily responsible for executing the workflow and managing the task or process described in the diagram. If the user is not a fixed user, the step will be assigned to another owner known as the Alternative Owner.

- **Alternative Owner**: The person or entity responsible for executing the workflow and managing the task in the absence of the Primary Owner or their inability to perform the task, preventing workflow failure or stalling.

- **Variable Owner**: An owner not fixed within the workflow but determined based on the value of a field within the entity structure. When selecting a variable owner, the field value for each entry is read, and the step is assigned to the user chosen within the field.

- **Relative Owner**: An entity that owns the step based on a relationship with the specified user, which may be a fixed user, variable user, or a previous step owner.

### Initial Step
When creating a workflow, the initial step is a default step, with the owner of this step automatically assigned as the creator of the entry. This step cannot be deleted but can be modified to some extent:

- **Step Name**: A multilingual text field with a minimum of 3 characters and a maximum of 128 characters.
- **Step Description**: A multilingual text field containing a description of the step.
- **Requirements**: Options applied to the fields used within the entity structure.

### Final Step
When creating a workflow, the final step is a default step that cannot be deleted but can be edited for the step name and description.

### When the Entry Enters the Initial Step
When an entry is created in the workflow, it enters the initial step. Once the initial step is executed, the workflow moves to the next step.

### Main Action
The main action is the primary and most crucial action within the step that must be executed to complete the task or move to the next step in the workflow. Although a step may contain several sub-actions, the main action is the core task that cannot be deleted or bypassed without successfully completing the task.

Executing the main action is essential to ensure the successful completion of the step and transition to the next step. While the step may include several preparatory or verification sub-actions, the main action must be executed afterward to complete the step.

Defining the main action in the workflow diagram helps users identify the exact primary task they need to perform to achieve the required goal and successfully complete the task.

### Main and Sub-paths
- **Main Path**: A sequence of steps systematically followed to achieve a specific goal in the diagram. It represents the primary method intended to achieve the desired goal, seeing the main action and fulfilling the steps built upon it.

- **Sub-path**: An alternative sequence of steps that occurs under certain conditions or decisions during the workflow execution. The sub-path is followed if the conditions for the main path are not met or if a decision is made to switch to an alternative method. Essentially, the main path is the primary sequence of planned steps to achieve the goal, while the sub-path represents alternative options used as needed or based on circumstances. Choices for switching between paths are based on effectively guiding the work execution towards achieving the desired outcomes.

## Related Concepts
- [Entities](./entities.md)
- [Services](./services.md)
- [Reactions](./reactions-and-automation.md)
- [Entries](./entries.md)



**Note: For more information on workflows operations, see: [Workflows Management](../../data-management/workflows.md).**