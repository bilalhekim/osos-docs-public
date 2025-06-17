---
title: "Timeline"
sidebar_position: 15
---

# Timeline

## Activating the Timeline {#activating}
To add a timeline, you must have an existing entity to display specific events for that entity. When creating an entity or if an entity already exists, enter this entity and select the "Edit Entity" button by clicking on the arrow next to the "Add Entry" button for the entity. Several options will appear in the top bar: (Details - Interactions - Structure - Workflow - Timeline). Choose "Timeline" to create a timeline related to this entity. An interface for adding a new timeline will appear; click in the middle of the screen on the add button to add the timeline. The timeline information will appear with default values named after the entity of the timeline and the icon of the same entity. Note: The name and icon of the timeline can be changed.

## Setting the Template - General {#template}
1. Enter the timeline interface as explained earlier.
2. Under "Post Settings," there is a "Post Template" field. Click on this field and select "General Posts."
3. The following fields will appear:
   - **Title**: Set the post title, which can be either fixed or variable. If you choose fixed, the post title will remain constant and cannot be changed with new entries. If you choose variable, the title can be linked to a field within the entity, making it automatically linked to the timeline.
   - **Description**: Provide a description for the post, which can also be either fixed or variable.
   - **Attachments**: Attachments can be added to the post, which can be either fixed or variable. Another option here is to make the type hidden so it does not appear in the post.

Note: Mandatory fields can only have fixed or variable values, with no hidden option, as users are required to select a value.

## Setting the Template - Events {#events}
1. Enter the timeline interface as explained earlier.
2. Under "Post Settings," there is a "Post Template" field. Click on this field and select "Calendar Posts."
3. The following fields will appear:
   - **Title**: Set the post title, which can be either fixed or variable.
   - **Description**: Provide a description for the post, which can be either fixed or variable.
   - **Start Date and Time**: Set the start date and time of the event, which can be either fixed or variable, linking it to the date and time field in the entity structure.
   - **End Date and Time**: Set the end date and time of the event, which can also be either fixed or variable.
   - **Cover**: Set a background for the post based on the type of value selected:
     1. Fixed type: Requires uploading an image that will be added to each new timeline entry.
     2. Variable type: Changes the timeline image according to the selected field in the entry.
     3. Hidden field: Disables the cover option in the timeline.
   - **Location**: Specify the event location, which can be a physical location or a link if the event is virtual.
   - **Attachments**: Add attachments such as files or images to the post, which can take values from fields if variable or can be fixed for all posts. This field can also be hidden.

## Publishing Settings {#publishing}
In this section, a set of settings related to the post is specified:
1. **Publishing Date**: Select a date field from the entity to automatically publish the post on this date, making it visible to users who should see it.
2. **Unpublishing Date**: Select a date field from the entity to automatically hide the post from users on this date.
3. **Publishing at Steps**: If there is a workflow, the post can be linked to publish upon reaching a specific step in the workflow.
   - Example: Publishing upon manager approval of an event.
   - The post can also be unpublished upon reaching a specific step in the workflow.

### Permissions
Specify the people who will see the post. There are two types of permissions:
1. **Authenticated**: Specific users or groups within the system.
2. **Anonymous**: The post is visible to everyone in the system or to outsiders if they have the post link.