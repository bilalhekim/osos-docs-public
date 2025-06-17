---
title: "Entities"
sidebar_position: 2
---

# Entities
Entities represent the fundamental components of the system that contain data. This guide explains how to create, list, modify, delete, browse entities, and manage their inputs and associated fields.

## Creating an Entity

To create a new entity on the platform, follow these steps:

1. **Access the relevant module**:
   - Go to the "Entities" tab within the module.
2. **Navigate to Entities via the main menu**:
   - Go to the "Applications" section.
   - Select "Entities".
3. **Add Entity**:
   - Click on the "Add Entity" button.
4. **Enter the required information**:
   - **Entity Name**: Mandatory text field, translatable, and must be unique within the module.
   - **Normalized Field**: Automatically generated and can be modified later.
   - **Icon**: Choose an appropriate icon.
   - **Module**: Automatically filled with the name of the module where the entity is created. If the entity is created from the Entities section, you need to select the module where the entity will be created.
   - **Entity Type**: Mandatory dropdown list.
5. **Confirm the addition**:
   - Click the "OK" button.
6. **Ensure success**:
   - A green confirmation message indicating the success of the operation will appear.

## Listing Entities

You can access entities via the following methods:

1. **Access the module where you want to search**:
   - Go to the "Entities" tab to display available entities within the module.
2. **Administration section**:
   - Go to "Applications".
   - Select "Entities" to display all available entities on the platform.

Entities are displayed as cards containing:
- Entity icon.
- Name of the module where the entity was created.
- Entity name.
- Number of inputs contained in the entity.
- Three dots opening options to edit the entity, add a new input, or archive it.

## Browsing an Entity

To browse an entity in detail:

1. Click on the entity card.
2. A page showing the inputs along with all available tabs within the entity will appear, such as:
   - [Queries](./queries.md).
   - [Views](./views.md).
   - [Buttons](./buttons.md).
   - [Lists](./lists.md).
   - [Dashboard](./dashboards-and-summaries.md).
   - [Reports](./reports.md).
   - [Relations](./relations.md).
   - Templates.
   - [Permissions](./permissions.md).

## Modifying an Entity

To modify an existing entity:

1. **First method**:
   - Click the three dots on the entity card.
   - Select "Edit Entity".
2. **Second method**:
   - After opening the entity, click the arrow next to the "Add Input" button.
   - Select "Edit Entity".

**Modify the entity data as follows:**
- Entity name.
- Icon.
- Singular and plural names.
- Description.
- You can also modify reactions, structure, workflow, and timeline.

## Handling Version Impacts

New versions might change the status of old data based on modifications to the entity. If there is a workflow, it will stop, and the manager must decide on the old values, either to leave them or update them. In the case of a workflow, it will revert to the initial step.

### Changes that cause a new version

The following modifications might cause a new version of the entity:
1. Adding a mandatory field.
2. Deleting a mandatory field.
3. Adding a step to the workflow.
4. Deleting a step from the workflow.
5. Changing the target step of the event.
6. Changing the step owner.
7. Making a field multiple.
8. Cancelling field multiplicity.

## Entity Structure Settings

### Form Settings

To control the form display of the entity structure:

1. Open the entity.
2. Click the arrow next to "Add Input".
3. Select "Edit Entity".
4. Go to the "Structure" tab.
5. Click the "Form Settings" button at the top of the form.
6. A side window for form settings will open.

### Display Settings

You can control display settings in various ways:
1. **Key/Value Display**:
   - Only one field is displayed per row.
2. **Two Columns Display**:
   - Two fields are displayed per row, and if there is an additional field, the column space in the row is filled accordingly.
3. **Three Columns Display**:
   - Three fields are displayed per row, and if there is an additional field, the column space in the row is filled accordingly.
4. **Four Columns Display**:
   - Four fields are displayed per row, and if there is an additional field, the column space in the row is filled accordingly.

## Archiving an Entity

To archive an entity:

1. Click the three dots on the entity card.
2. Select "Archive".
3. Confirm the operation in the message that appears.
4. After confirmation, the entity will be moved to the archive.