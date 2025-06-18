---
title: "Views"
sidebar_position: 5
---

# Views
In the platform, a view serves as the main point of interaction between the user and the system. Through views, users can easily manage entries, including listing, displaying, adding, editing, and performing other tasks that will be explained later. These operations are carried out according to the permissions and settings predefined by the administrator. Each view is characterized by specific information and settings tailored to meet particular needs, which will be detailed in the following sections.


## Types of Views
The types of views in the platform include three different categories, which can be explained as follows:

1. **Authenticated:** An authenticated view in the platform is the interface that grants all users who have verified their identity (logged in) access to it, according to the settings defined by the administrator. This type of view is suitable for displaying content that is relevant to all registered users.

2. **Anonymous:** In this type of view, it is not necessary for the visitor to be an authenticated user on the platform. Anyone with the view link can access its content without the need to log in.

3. **Restricted:** This view is specifically created by the administrator for a specific user or group of users. Access to this view is restricted and granted only to those selected in the view's access permissions settings.

By providing these different types of views, users can customize and define the scope of content access according to their specific needs and requirements.

## Display Formats
### Table View {#table-face}
Displaying entries in a table format is one way to organize and arrange entries in the system. The table format is used to present information in an organized and easily readable manner, where entries are divided into rows and columns. Each row contains entry data, while columns represent the fields of the entry.

### Card View {#cards-face}
Displaying entries in a card format is an attractive way to organize and browse entries visually. Entries are shown in individual cards, with each card containing specific information (such as image, title, description, and creation or update information) and being independent of others.

### Calendar View {#calendar-face}
Displaying entries in a calendar format is an effective way to organize events and tasks over time. The calendar format is used to gather data related to dates and events in an organized and accessible manner. Entries can be viewed monthly, weekly, or daily.

### Kanban View {#kanban-face}
The Kanban view method is based on a visual display of work through a board that divides tasks into sections representing progress stages. For example, the progress stages in task management might include "Planning," "In Progress," and "Completed," with each stage containing the related entries.

### Tree View {#tree-face}
Displaying entries in a tree format organizes entries in a hierarchical structure resembling a tree. The tree view is used to gather entries into graded levels, classifying sub-entries under main elements or groups.

### Timeline View {#timeline-face}
Displaying entries in a timeline format is an effective and visual way to organize entries chronologically. The timeline shows events, tasks, and activities in a time sequence, presenting the temporal development of entries, with each entry containing an image, title, and description.

### Mini Cards {#mini-cards-face}
Displaying entries in a mini-card format provides a way to view entries through counters.

## Important to Know
### Default View
The default view principle allows us to designate one view as the automatic view displayed when there are multiple views in the entity. Thus, the system will automatically direct to this default view.

### View Constraints
1. **Cannot Assign Two Default Views:**
   This means that in this module or system, you cannot designate two default views simultaneously. Only one view should be selected as the one that is displayed automatically.

2. **Enable Entry List View Before Entry Details View:**
   To allow the display of specific entry details, the entry list view option must be enabled first. This is necessary to direct users to select entries before displaying their details.

3. **Cannot Enable Filters Without Search:**
   Enabling the search function is a prerequisite before enabling filters. This means that the search must be active before allowing detailed information display or filters.

4. **Enable Filters to Activate Current or Previous Step Filters or Save Queries:**
   This means that using filters in the module or system requires the filter function to be enabled first. Without enabling filters, current or previous step filters or saving queries cannot be performed.

## Related Concepts
- [Permissions](./permissions.md)
- [Queries](./queries.md)
- [Entries](./entries.md)
- [Dashboards](./dashboards.md)


**Note: For more information on views operations, see: [Views Management](../../data-management/views.md).**