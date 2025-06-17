---
title: "Buttons"
sidebar_position: 16
---

# Buttons and Navigation in the User Interface

Buttons are interactive elements in the user interface used to facilitate navigation between system pages and execute required actions quickly and easily.  
This guide explains how to create and modify buttons in the user interface, as well as the steps to define the actions executed when clicking those buttons for navigation or specific functions.

## Adding a Button Within an Entity

To define a button within an entity, follow these steps:

1. Access the entity:
   - Go to Administration > Applications > Units > Find the relevant unit > Entities tab > Find the entity.
   - Or go to Administration > Applications > Entities > Find the desired entity.

2. Click on the "Buttons" tab on the entity page.  
3. Click "Add New Button."  
4. A dialog box will appear with the following fields:  
   - **Name:** A required field, can be written in both Arabic and English, and represents the button name.  
   - **Icon:** Optional, choose an icon for visual identity.  
   - **Description:** Optional, can be written in both Arabic and English.  
   - **Action:** Choose the action the button will perform from the dropdown list:
     - **Custom Event:** Shows all custom event interactions defined in the entity.
     - **UI Event:** Shows UI-specific custom events with options like "UI-specific" and "Ask User."
     - **Navigation:** To define navigation behavior after button execution.
   - **Scope:** To define the scope of the button, select one of the following:
     - **Single Entry:** Executes on one entry.
     - **Multiple Entries:** Executes on selected entries.
     - **Both:** Executes on both a single and multiple entries.

### Save and Publish the Button

1. Click "Save" to store the settings.  
2. Return to the "Buttons" tab and click "Publish Button" to make it available for use.  
3. A confirmation message will appear; click "OK."

## Defining a Button That Executes a Custom Event

1. Follow the steps for adding a new button.  
2. Select the "Custom Event" action.  
3. The defined custom events in the entity will appear.  
4. Choose one of the interactions.  
5. **Optional: Customize navigation on a single entry:**
   - You can define actions for:
     - **Successful execution of the button:**
       - Select the navigation type from the dropdown list:
         - **Relationship:**
           - Choose an inbound or outbound relationship defined in the entity.
           - Then select one of the following navigation actions:
             - Display Entries List.
             - Create Entry.
             - Display Entry Details.
             - Update Entry.
         - **Current View:**
           - Select one of the navigation actions:
             - Display Entries List.
             - Create Entry.
             - Display Entry Details.
             - Update Entry.
         - **Custom Link:**
           - Choose the action and enter the desired link.
     - **Failed execution of the button:**
       - Select the navigation type the same way as above.

## Defining a Button That Triggers Navigation

1. Follow the steps for adding a new button.  
2. Select the "Navigation" action.  
3. Choose the type of navigation:
   - **Current View:** Then choose one of the following:
     - Display Entries List.
     - Create New Entry.
     - Display Entry Details.
     - Update Entry.
   - **Relationship:** Choose from inbound or outbound relationships in the entity, then select the appropriate navigation action:
     - Display Entries List.
     - Create New Entry.
     - Display Entry Details.
     - Update Entry.
   - **Custom Link:** Enter the desired link.

## Filtering Buttons

The system allows defining buttons that apply to specific entries based on a saved query or a manually defined filter in the button settings.  
The filter determines which entries the button can apply to.  
The button will only appear if the selected entries match the filter conditions.

For more information on creating a query, [click here](../my-first-application/my-first-app-modifying-the-tasks-system#creating-a-query).

Users can also use a previously saved query from the entity. Saved queries are displayed under the **Entry Source** option.
