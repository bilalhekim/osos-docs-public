---
title: "Reactions and Automation"
sidebar_position: 13
---

# Reactions and Automation
A reaction is a mechanism used to perform actions and automate processes on entries, triggering automatic responses in reaction to specific events. This mechanism operates by activating a series of actions within the system based on a predefined set of events. These events may include, for example, creating a new entry, modifying an entry, archiving an entry, reaching a certain step in a workflow, exiting a step in a workflow, time-based notifications, custom events, and more.

Reactions are created using specific contexts and are executed automatically when certain events occur or specified conditions are met. Examples of possible actions include: sending notifications, sending emails, calling APIs, executing workflow steps, and performing other custom actions.

This approach facilitates the workflow for users and increases the flexibility of working within the system. By executing actions and automatic responses based on events and conditions, workflow efficiency can be improved, and manual effort and time required to complete processes can be reduced.

## Important to Know
### Event
An event is a crucial concept that triggers reactions in the system. It specifies a certain action or process that meets defined conditions to execute specific actions. These events vary in types and include:
- "On new entry creation": Activated when a new entry is added.
- "On entry modification": Triggered when an existing entry is modified.
- "On entry archiving": Activated when an entry is moved to the archive.
- "On reaching a certain step in a workflow": Triggered when the process reaches a specific stage in the workflow.
- "On exiting a workflow step": Activated when a certain stage in the workflow is completed.
- "Timer": Activated based on a specified time interval.
- "Custom event": Activated based on a predefined custom event.

### Action
An action consists of a set of tasks that are executed when an event is triggered. These tasks include various operations such as "creating an entry," "modifying an entry," "sending a notification," "sending an email," "sending a text message," "calling an API," moving the workflow to a specific step, and executing defined steps in the workflow.

### Filtering
Filtering involves optional conditions that are applied to execute the reaction when a specific event occurs, according to a particular action. Filtering helps to narrow down the scope of the reaction based on specified conditions.

## Related Concepts
- [Entities](./entities.md)
- [Workflows](./workflows.md)
- [Dashboards](./dashboards.md)



**Note: For more information on reactions & automation operations, see: [Reactions and Automation Management](../../data-management/reactions-and-automations.md).**