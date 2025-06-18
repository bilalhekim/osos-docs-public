---
title: "Pages"
sidebar_position: 5
---
# Building a Home Page for the Application

## Building the Visitor Page {#visitor-page}
This page will be displayed before logging into the system.

### Creating the Page
You can create a page in the platform by following these steps:
1. Go to the sidebar and click on **Administration**.
2. Click on **Applications** then **Modules**.
3. Select the **Task Management Application**.
4. Click on the **Pages** tab.
5. Click on **Add New Page**.

- **Details Tab**
   1. In the **Details** tab, do the following:
      - Fill in the **Name** field in both Arabic and English, for example: External Page. Complete the page settings as detailed [here](../../data-management/pages).
      - Set the **Access Permissions** to define whether the page is internal or external.
      - Select the **Anonymous** option to make the page external. A link will be generated, which can be accessed by clicking on it.
      - Optionally, set the page as the default. This means it will be displayed when a user logs out.
      - Multiple links can be created for a single page.

- **Content Tab**
   1. Add a **Text** component with a welcome message, such as: Welcome to the Task Management Application.
   2. Additionally:
      - Drag and drop the **Main Image Slider** component into the desired location.
      - Select an image from the media library, provide a suitable title in both Arabic and English (the title is optional).
      - You can add multiple images in the same manner to finalize the component.
      - Drag and drop the **About Us** component, and within it, add the mission, vision, and values in both Arabic and English.
   3. Save the changes by clicking the **Finish** button at the top of the screen.

After saving the changes, publish the page to make it accessible to visitors. When a user logs into the system, the main page will be the one they interact with.

## Building the User Page {#user-page}
### Creating the Page
You can create a page in the platform by following these steps:
1. Go to the sidebar and click on **Administration**.
2. Click on **Interfaces**.
3. Click on **General**.
4. Click on **Add New Page**.

#### Details Tab
1. In the **Details** tab, follow the same steps as mentioned in the previous section.
2. Set the **Access Permissions** to define whether the page is internal or external.
3. Select the **Authenticated** option and choose the groups allowed to access the page. This will make the page restricted.

#### Content Tab
1. In the **Content** tab, do the following:
   - Add a **Media** component to the header with one or more images.
     - Provide a title for the image in both languages.
     - Choose an image that represents the system's identity.
   - Add a **Welcome** component with a welcome message including the registered user's name.
     - Enable the option to display the registered user's name.
     - Upload a custom icon and enable its display.
     - Enable the option to reverse the icon's direction when the language changes.
   - Add a set of quick links or a link list to navigate to other pages and views using the **Links** or **Quick Links** component.
     - Add an unlimited number of links by clicking on **Add Another Link**.
     - For each link, provide the title, icon, link type, and how it opens.
   - Add a link to "Add New Task" that directs to the task view for adding new tasks using the **Link** component.
     - Provide a suitable title, e.g., Add New Task.
     - Choose an appropriate icon.
     - Select the type: Data View.
     - Select the opening method: Same window.
     - The module will be selected automatically.
     - Choose the **Task Entity**.
     - Finally, select the **Task View**.
   - Add a **View** component to display "My Tasks".
     - First, select the source: from the module list, choose the Task Management Application, and then choose the **Tasks Entity**.
     - The view will be selected automatically.
     - Then, select the number of entries, e.g., 5 entries.
   - Add a **Summary** component to display summaries available in the system.
     - The module will be selected automatically, which is the Task Management Application.
     - Select the entity from which you want to get the summary, e.g., Task Entity.
     - Choose one of the summaries to display on the page.
2. Save the changes by clicking the **Finish** button at the top of the screen.
3. Publish the page to make it available in the sidebar for users to access.

This main page will be displayed in the sidebar on the right side of the screen with the name assigned to the page. It can also be accessed via the top bar by clicking on the home icon.

## Default Pages {#default-pages}
To set a default page in the Task Management Application, follow these steps:

1. Go to the sidebar and click on **Administration**.
2. Navigate to **Applications** then **Modules**.
3. Select the **Task Management Application**.

#### To Set an Anonymous Default Page:
4. Click on the **Pages** tab.
5. Select the page you want to set as default.
6. Set the page type to **Anonymous**.

#### To Set an Authenticated Default Page:
7. Click on the **Pages** tab.
8. Select the page you want to set as default.
9. Set the page type to **Authenticated**.
10. Select the groups allowed to access this page.

This allows you to set a default page in the Task Management Application, choosing its type based on your needs, whether it’s an anonymous page shown upon logout or an authenticated page accessible through the home icon in the top menu.