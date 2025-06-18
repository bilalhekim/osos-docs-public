---
title: "Entity"
sidebar_position: 2
---

# Building a Support Tickets Entity
An entity is the primary element for storing data, similar to tables in databases. They are defined in each system to represent different sections or elements. For more information about entities, refer to [Entities](../../../guide/information-structures-concepts/basic-concepts/entities).

## Adding a Support Tickets Entity
To build an entity within the Customer Support module that includes operations on support tickets, follow these steps:

1. Click on the Customer Support module.
2. Click on the **Add Entity** button.

![Add Entity](../../../../../../../static/img/tutorial/customer-support-system/en/4--system%20building--entities--1.png)

A window for adding an entity appears, where you need to fill in the entity information:

1. **Name (Mandatory):** Name it "Support Tickets" in both Arabic and English.
2. **Icon (Mandatory):** The system administrator should select an icon for the entity; let's choose the "wrench" icon.
3. **Entity Type (Mandatory):** The system administrator should define the entity type. In this case, it will be "Natural Entity". For more information on entity types, refer to [Entities](../../../guide/information-structures-concepts/basic-concepts/entities).
4. **Model Field (Mandatory):** This field is generated automatically once the entity name is entered in Arabic or English, but the system administrator can modify this field. It cannot be left empty. For more information on the model field, refer to [Model Field](../../../guide/information-structures-concepts/basic-concepts/modules).
5. **Unit Field (Mandatory):** This is a locked field that cannot be modified, automatically filled with the unit name where the entity is created, "Customer Support System".
6. **Singular Name (Optional):** This is the singular name of the entity entries, which will be "Support Ticket" in both Arabic and English.
7. **Plural Name:** This is the plural name of the entity elements, which will be "Support Tickets" in both Arabic and English.
8. **Permissions Management (Optional):** The system administrator can control the entity's permissions as needed. For more information on permissions, refer to [Permissions](../../../guide/information-structures-concepts/basic-concepts/permissions).
9. Click the "Create" button to create the "Support Tickets" entity.

![Entity Details](../../../../../../../static/img/tutorial/customer-support-system/en/5--system%20building--entities--2.png)

## Adding Entity Structure
Once the entity is added, the user is directed to the entity details page. To build the entity structure, follow these steps:

1. Click on the **Structure** tab.
2. An empty page appears.
3. Drag and drop the structure fields into the empty area. The fields are as follows:

![Entity Structure](../../../../../../../static/img/tutorial/customer-support-system/en/6--system%20building--entities--3.png)

- Ticket Number (Sequential Field).
- Ticket Title (Multi-language Text).
- Ticket Description (Multi-language Text).
- Ticket Status (Classification): Status options (Open, In Progress, Responded, Duplicate, Closed).
- Assignee (User).
- Ticket Opening Date (Date and Time).
- Ticket Closing Date (Date and Time).
- Solution (Block).
- Solution (Multi-language Text).
- Service Rating (Block).
- Rating Score (Converter): Add rating options from 1-5.
- Comment (Multi-language Text).

4. Click the "Save" button to save the structure of the "Support Tickets" entity.

![Save Structure](../../../../../../../static/img/tutorial/customer-support-system/en/7--system%20building--entities--4.png)
![Save Structure](../../../../../../../static/img/tutorial/customer-support-system/en/8--system%20building--entities--5.png)
![Save Structure](../../../../../../../static/img/tutorial/customer-support-system/en/8--system%20building--entities--6.png)

## Adding Workflow:
To build a workflow for the entity, follow these steps:

1. Click on the Workflow tab.
2. The workflow page appears.
3. Click on "Click to activate the workflow" in the middle of the page to activate the workflow.

![Workflow Tab](../../../../../../../static/img/tutorial/customer-support-system/en/8--system%20building--entities--8.png)

4. Click on "Start" to change the step name.
5. Workflow step settings appear.
6. Change the name "Start" to "Open Ticket".

![Workflow Step](../../../../../../../static/img/tutorial/customer-support-system/en/8--system%20building--entities--9.png)

7. Change the action name "Start" to "Submit Request".

![Change Action Name](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(4).png)

8. Change the field settings in the step by clicking on "Open Ticket".
9. Click on "Editable" to display field options and select what you want to display.

![Field Settings](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(5).png)
![Field Settings](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(6).png)

10. Build the second step, "Support Desk", by clicking on "Add Step".

![Add Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(7).png)

11. A popup window appears to fill in the step information.
12. Click the "Finish" button to save the step.

![Save Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(8).png)
![Save Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(9).png)

13. To delete a step, click on "Delete Step".
![Delete Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow.png)

14. Change the name of the main action to "Send for Processing" as done in the first step.

![Change Action Name](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(10).png)
![Change Action Name](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(11).png)

15. Build a new step, "Ticket Processing", by following the same steps as before.

![Build New Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(12).png)
![Build New Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(13).png)

16. Change the name of the main action to "Review Solution".
17. Change the target step to "Previous Step".

![Change Target Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(14).png)

18. Add a new step, "Service Rating", by following the same steps as before.
19. Change the name of the main action to "Rated".
20. Change the target step to "Support Desk".
21. Change the field settings for the "Service Rating" step.

![Service Rating Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(15).png)
![Service Rating Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(16).png)

22. Change the target step in the "Send for Processing" action in the "Support Desk" step to "Ticket Processing".

![Change Target Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(18).png)
![Change Target Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(19).png)

23. Add a new action "Close Ticket" by clicking the **+** sign at the top of the step.
24. A popup window appears to fill in the action information.

![Add Action](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(20).png)

25. Add a new action "Send Solution".

![Add Action](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(21).png)
![Add Action](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(22).png)

26. Build a new step, "Manager Approval", by following the same steps as before.
27. Change the name of the main action to "Approve".
28. Change the target step to "Previous Step".

![Build New Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(24).png)
![Build New Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(25).png)
![Field Settings](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(26).png)

29. Add a new action for the "Manager Approval" step called "Reject" by following the same steps as before.

![Add Action](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(27).png)

30. Add a new action in the "Support Desk" step called "Manager Approval" as done before.
31. Click the **+** sign at the top of the step.

![Add Action](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(28).png)

32. Change the field settings of the "Support Desk" step.

![Change Field Settings](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(29).png)
![Change Field Settings](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(30).png)

33. Change the field settings of the "Ticket Processing" step.
34. You can also delete a step by clicking on the "Delete Step" button in the step settings.

![Delete Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(31).png)
![Delete Step](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(32).png)

35. Click the "Save" button to save the workflow.
36. To delete the workflow, click on the trash can icon at the top of the workflow.

![Save Workflow](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-workflow(35).png)

For more information about workflows, refer to [Workflows](../../../guide/information-structures-concepts/basic-concepts/workflows).

## Adding Reactions
Reactions allow you to set up notifications and send them to the concerned parties. To add a notification, follow these steps:

1. Click on the Reactions tab on the entity details page.
2. Click on the **+** sign.

![Add Reaction](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(1).png)

3. A popup window appears to fill in the reaction information.
4. Add a reaction called "Customer Response".

![Customer Response](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(2).png)
![Customer Response](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(3).png)
![Customer Response](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(4).png)

5. Add another reaction called "New Ticket Arrival" by following the same steps.

![New Ticket Arrival](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(5).png)
![New Ticket Arrival](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(6).png)
![New Ticket Arrival](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(7).png)

6. Add a new reaction called "Ticket Assigned to You" by following the same steps.

![Ticket Assigned](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(8).png)
![Ticket Assigned](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(9).png)
![Ticket Assigned](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(10).png)

7. Add a new reaction called "Solution Review" by following the same steps.

![Solution Review](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(11).png)
![Solution Review](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(12).png)
![Solution Review](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(13).png)

8. Add a new reaction called "Solution Reviewed".

![Solution Reviewed](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(14).png)
![Solution Reviewed](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(15).png)
![Solution Reviewed](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(16).png)

9. Add a reaction called "Request Solved".

![Request Solved](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(17).png)
![Request Solved](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(18).png)
![Request Solved](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(19).png)

10. Add a reaction called "Service Rating".

![Service Rating](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(20).png)
![Service Rating](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(21).png)
![Service Rating](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(22).png)

11. Click the "Save" button to save the reactions.

![Save Reactions](../../../../../../../static/img/tutorial/customer-support-system/customer-support-create-reactions(23).png)

For more information about reactions, refer to [Reactions](../../../guide/information-structures-concepts/basic-concepts/reactions-and-automation).