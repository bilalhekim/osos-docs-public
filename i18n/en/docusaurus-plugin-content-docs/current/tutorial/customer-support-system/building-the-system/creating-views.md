---
title: "Views"
sidebar_position: 4
---

# Building a Ticket Request View

To build views or interfaces, you need to access the "Support Tickets" entity and follow these steps:
For more information about views, you can refer to [Views](../../../guide/information-structures-concepts/basic-concepts/views).

## 1. Building the "Request Ticket" View

- Access the "Support Tickets" entity.
- Click on the "Views" tab.
- Click on the **+** sign next to the "New View" button on the far right to add a new view.

![Views Tab](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(1).png)

- The "View Information" page appears.
- Fill in the page with the information of the view you want to build.
  - Name (Mandatory): Enter the name of the view in both Arabic and English, which will be "Request Ticket".
  - Entity (Mandatory): This field will be automatically filled with the name of the entity, which will be "Support Tickets".
  - Icon (Optional): Select an icon that represents the view, here we will choose "megaphone".
  - Data Source (Mandatory): Select the inputs or query on which the view will be based, here we will choose "inputs".
  - Fields (Mandatory): Specify the fields of the view, here we will select the following fields (Ticket Number, Ticket Title, Ticket Description, Ticket Opening Date, Service Rating).
- Enable the "Pin to Sidebar" button so the view appears in the platform's sidebar.

![Pin to Sidebar](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(2).png)

### Access Permissions Section:

This section contains several fields:

- Enable the "Verified" button without specifying who can use it exactly, as it can be used by employees and customers.

### Display Ticket List Section:

Enable the "Display Ticket List" button to display a list of entries according to several formats that can be specified in this section:
- Specify the view type as "Table" and the default value.
- Columns of Fields (Mandatory): Specify the fields you want to display in the view list, which are (Ticket Number, Ticket Title, Ticket Description, Ticket Opening Date, Service Rating).
- Do not specify other view formats if not needed.

![Display Ticket List](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(3).png)

- Enable "Allow Search" and "Allow Filters" to enable searching or filtering.
- Leave the "Display Dashboard" button disabled for now.
- Enable the "Display Ticket Information" button.
- Several fields will appear after enabling it, including:
  - Specify the fields you want to display in the ticket information, which are (Ticket Number, Ticket Title, Ticket Description, Ticket Opening Date, Service Rating).

![Display Ticket Information](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(4).png)

- Enable the "Show Discussion" button and select all options within it.
- Enable the "Display Entry History" button and enable the first two options within it (Display Modifications, Display Who Made Modifications).

![Show Discussion](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(5).png)

- Leave "Display Relationships" disabled as it is not needed here.
- Enable the "Allow Adding New Tickets" button, and several fields will appear after enabling it:
  - Specify the fields that can be added, which are (Ticket Number, Ticket Title, Ticket Description, Ticket Opening Date, Service Rating).
  - After saving: Choose "Return to Entry Details View" to specify where to navigate after saving the entry.
- Enable the "Allow Editing Tickets" button and select the same options as for adding.

![Allow Adding New Tickets](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(6).png)

- Click the "Finish" button at the top left of the view page.

![Finish](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(7).png)

- A popup will appear, click "Save Changes" to save the changes made to the view.
- Click the "Publish" button to make the view accessible to users.

![Publish](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(8).png)


## 2. Building the Incoming Requests View

Follow the same steps as above.

![View Information](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(9).png)

- Here, we select the users (employee, responsible manager).

![Select Users](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(10).png)

![Display Ticket Information](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(11).png)

![Display Ticket Information 2](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(12).png)

![Add/Edit Tickets](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(13).png)

![Finish](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(14).png)

![Publish](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_views(15).png)