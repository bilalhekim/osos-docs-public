---
title: "Pages"
sidebar_position: 9
---

# Pages

## Creating a Page {#creating-a-page}

To create a page within a unit in the Asas system, follow these steps:

1. Open the Modules from the sidebar.
2. Select the unit for which you want to design a page.
3. Click on the Pages tab.
4. Click on Add New Page.

When creating the page, two main tabs will appear: Details and Content.

## Page Settings {#page-configuration}

### Page Information

This section includes the following fields:
1. Name: A mandatory, multilingual field.
2. Description: An optional, multilingual field.
3. Icon: A mandatory field.

### Sidebar Settings

This section includes the following options:
1. Pin the page to the system sidebar.
2. Choose the default display method for the sidebar when opening the page (Keep, Open, Close).

### Display Options

In this section, you can select some display attributes for the page:
1. Transparent page.
2. Page padding.
3. Content padding.
4. Show page title.
5. Fixed width page.

## Adding Page Components {#building-a-page}

From the Content tab, users can design the page using drag-and-drop components, which will be detailed later.

1. You can control the width of the component on the page.
2. You can align the component on the page.
3. You can move the component on the page after creating it using drag-and-drop.

## Publishing and Unpublishing Pages {#publishing-and-blocking}

Once the page is created, settings are configured, and appropriate content is added and saved, the page will appear in the Pages interface but will not be visible to the designated audience until published.

## Conditional Visibility {#conditional-visibility}

Pages in the Asas system consist of several components, which can be tailored to a specific audience.

## Access Permissions {#access-permissions}

There are three access permission options for the page:
1. Authenticated: All users in the system have access to the page.
2. Restricted: Specific users or groups have access to the page.
3. Anonymous: The page is intended for visitors and can be accessed by anyone via an external link.

## Default Pages {#default-pages}

The concept of default pages is that when there is more than one page within a unit, one can be designated as the default page. Therefore:

1. An anonymous default page means that anyone entering the system before logging in or after logging out will be redirected to this page.
2. An authenticated default page means that upon logging into the system, this page will be displayed.

## Viewing Pages on Mobile App {#viewing-pages-from-mobile}

Pages in the Asas mobile app will be displayed in the same component order.

# Components 

Components are a set of tools that are arranged and organized in a specific way to create pages for the end user [click here](#building-a-page).

## Types of Components {#page-components}

There are many types of page components that we drag and drop to appropriately form pages for the end user.

**Note**: Most page components contain two sections within them (Content, General). I will first highlight the content as it varies between components, while General remains the same across all components.

1. **Section**: A tool that can contain multiple page components and is used to arrange and organize the page.
2. **Column**: A tool that contains multiple page components, which can be divided into various sizes to arrange columns side by side or sequentially to organize the page.
3. **Text**: A tool that displays fixed text content and is used to write multi-line text on the page and display it to the end user. It contains a single field:
   - Fixed Text Field: A mandatory field where text can be written in both Arabic and English.
4. **Heading**: A tool that displays text (main or subheading) at various levels and is used to add main and subheadings to page components and display them to the end user. It contains the following fields:
   - Text: A mandatory field where the heading is written in both Arabic and English.
   - Level: A mandatory field to choose the heading level, ranging from Heading 1 to Heading 6.
5. **Link**: A tool that displays a link on the page, allowing navigation to other pages either within the system or externally. It contains the following fields:
   - Title: The title of the link, which is mandatory and can be written in both Arabic and English.
   - Icon: A mandatory field to select an appropriate icon from the available system icons.
   - Type: A mandatory field to choose the link type (External, System Page, Unit Page, Data View).
   - Open In: A mandatory field to choose whether the link opens in the same window or a new tab.
6. **Link List**: A tool that displays a list of links on the page for easy navigation between them. It contains the same fields as the Link component, with an additional field to add more links.
7. **Media**: A tool to display media (image, video) on the page and is used to add and display specific media to the end user. It contains several fields:
   - Title: An optional title for the media, written in both Arabic and English.
   - Media: A field to upload an image or video to document a specific matter and display it to the end user.
8. **Media List**: A tool to display a list of media (images, videos) on the page. It contains the same fields as the Media component, with an additional field to add more media.
9. **File**: A tool to display a file (documents, images) on the page and is used to add and display documents and images to the end user. It contains several fields:
   - Title: The file title, which is mandatory and can be written in both Arabic and English.
   - File: A mandatory field to upload any type of file.
   - Image Preview: An optional field to upload a preview image.
10. **File List**: A tool to display a list of files to the end user. It contains the same fields as the File component, with an additional field to add more files.
11. **Timeline**: A tool to display certain posts in a timeline format on the page. It contains several fields:
   - Page Navigation: Options are Auto, Manual, and Page Numbers.
   - Number of Posts: The initial number of posts to display.
   - Show Pinned Posts: An option to show pinned posts with a pin icon.
   - Source: Options are Entity, Unit, or General, with additional fields appearing based on the selection.
12. **Summary**: A summary or statistical overview that provides a clear and quick idea about the system, program, or project. It contains the following fields:
   - Unit: A mandatory field to choose a unit within the system.
   - Entity: A mandatory field to choose an entity within the unit.
   - View: A locked field.
   - Choose Summary: Displays summaries for the selected entity to choose from.
13. **View**: A tool that displays a minimal view of a table view and is used to display some view information in a small format to the end user. It contains the following fields:
   - Source: A mandatory field to choose a view from one of the Modules.
   - View: A locked field, currently filled with Table view.
   - Number of Entries: A mandatory field to choose the number of entries (3, 5, 10), defaulting to 5 if not chosen.
14. **Navigation Tool**: A tool that displays shortcuts to pages or views for easy navigation. It contains several fields:
   - Title: An optional field for the navigation title, written in both Arabic and English.
   - Display Options: Includes options for the number of columns (1-12) and row height (Auto, Fixed 1 Row, Fixed 2 Rows, etc.).
15. **Timeline Viewer**: A tool that displays posts in a timeline format on the page. It contains several fields:
   - Post Template: Options are Calendar Posts and General Posts.
   - Number of Posts: The initial number of posts to display.
   - Show Pinned Posts: An option to show pinned posts.
   - Title: A mandatory field for the timeline viewer title, written in both Arabic and English.
   - Icon: A mandatory field to select an appropriate icon.
   - Type: A mandatory field to choose the link type (External, System Page, Unit Page, Data View).
   - Open In: A mandatory field to choose whether the link opens in the same window or a new tab.
16. **Main Timeline Viewer**: A tool that displays posts in a slideshow format. It contains the same fields as the Timeline Viewer component.
17. **Main Image Viewer**: A tool that displays images in a slideshow format. It contains several fields:
   - Title: An optional title for the media, written in both Arabic and English.
   - Media: A field to upload an image or video.
   - Add More Media: An optional field to add more media.
18. **Welcome Title**: A tool that displays a welcome message to the end user upon entering the page. It contains several fields:
   - Show Registered Username: An option to display the registered user's name.
   - Show Icon: An option to upload an icon.
   - Rotate Icon for RTL: An option to rotate the icon when switching to Arabic.
19. **Views and Summaries**: A tool that combines summaries and views. It contains the same fields as the View and Summary components.
20. **About Us**: A tool that provides a brief introduction about the company or organization. It contains several fields:
   - Mission: A mandatory field to describe the mission.
   - Vision:

 A mandatory field to describe the vision.
   - Values: A mandatory field to describe the values.
   - About the Organization: A mandatory field to give a brief description.
   - Title: A mandatory field for the link title.
   - Icon: A mandatory field to choose an appropriate icon.
   - Type: A mandatory field to choose the link type (External, System Page, Unit Page, Data View).
   - Open In: A mandatory field to choose whether the link opens in the same window or a new tab.
21. **Quick Links**: A tool that displays shortcuts to pages or views for easy navigation, displayed in either circular or grid format. It contains several fields:
   - Circular Display: An option to display arrows above the links for circular navigation.
   - Grid Display: An option to display links in a grid format.
   - Show Title: An option to display the title above the links.
   - Title: A mandatory field for the link title.
   - Icon: A mandatory field to choose an appropriate icon.
   - Type: A mandatory field to choose the link type (External, System Page, Unit Page, Data View).
   - Open In: A mandatory field to choose whether the link opens in the same window or a new tab.
   - Add More Links: An optional field to add more links.
22. **Quick Services**: A tool that displays shortcuts to services within the system for easy access. It contains two options:
   - Display Services Normally: An option to display services as normal cards.
   - Display Services as Business Cards: An option to display services as medium-sized business cards with Details and Request buttons.
23. **Static Content**: A tool that displays views such as advertisements, events, and timelines on the page. It contains several fields:
   - Advertisements: Contains fields to choose the source and number of entries.
   - Events: Contains the same fields as Advertisements.
   - Timeline: Contains the same fields as Advertisements.
   - Show Icon: An option to display an icon with additional fields for uploading and rotating the icon.
24. **Success Stories**: A tool that displays posts containing success stories of companies, organizations, or individuals. It contains several fields:
   - Source: A mandatory field to choose the view from one of the Modules.
   - View: A locked field, currently filled with Table view.
   - Number of Entries: A mandatory field to choose the number of entries (3, 5, 10), defaulting to 5 if not chosen.
25. **Wiki**: A tool to provide an introduction to the page content, with the option to upload a video. It contains several fields:
   - Source: A mandatory field to choose the view from one of the Modules.
   - View: A locked field, currently filled with Table view.
   - Number of Entries: A mandatory field to choose the number of entries (3, 5, 10), defaulting to 5 if not chosen.
   - Title: An optional field for the page title.
   - Media: A field to upload a video providing an introduction to the page.

## General Section {#general-section}

This section is common across all components and appears when dragging a component. It contains the following fields:

- Title: An optional field for the main title of the component.
- Description: An optional field to describe the component.
- Icon: An optional field to choose an icon for the component title.
- Custom Display: An optional toggle to choose specific users or groups who can access the component.
- Custom Style: An optional toggle to assign a custom name to the component for styling purposes.

**Note 1**: All tools contain a set of common settings:

- The default size is full width, which can be adjusted to one of the following options (4, 6, 8, 12).
- Delete tool: Click the delete button to remove the tool, with a confirmation message appearing before deletion.
- Edit tool: Modify the previous content of the tool.
- Drag-and-drop capability: Drag the tool to the page and drop it to add a tool.
- Change the position of the tool: Click the move icon to place the tool in the desired position.
- Rearrange elements within the tool: (Top, Bottom, Expand, Center).

**Note 2**: The Paragraph tool contains an additional setting:

- Edit Height: Specify the height of the paragraph.
