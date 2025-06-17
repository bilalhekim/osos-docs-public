---
title: "Links"
sidebar_position: 24
---

# Operations on the Links Entity

The **Links Entity** allows you to display and manage all entries with either manual ownership or system ownership. These entries are arranged in the sidebar based on the value of the **Order** field, sorted from smallest to largest.

## Manually Adding an Item to the Sidebar

To manually add an item to the sidebar using the **Links Entity**, follow these steps:

1. Log in to the platform with an admin account.
2. Navigate to the **Sidebar**.
3. Click on the **Entities** section.
4. Access the **Links Entity**.
5. Click the **"Create Entry"** button.
6. Fill out the form:
   - **Order Field:** Enter a numeric value; entries are sorted from smallest to largest.
   - **Parent Field:** A self-referencing field to define hierarchy within the sidebar.
   - **Published Field:** Enable this field to make the entry visible in the sidebar.
   - **Ownership Field:** Select "Manual".
   - **Type Field:** Choose the type of entry (Module, View, Page, Report, Uncategorized).
   - **Icon Field:** Select an icon to visually represent the entry.
   - **Name Field:** Enter the entry's name.
   - **Description Field:** Enter a description for the entry.
   
7. Fill out the second section **"Target"**:
   - **Link Field:** Enter a link if the type is "Uncategorized".
   - **Target ID:** This is auto-filled when the entry is system-owned.
   - **Target View Action:** Enter the view link if the type is "View".
   
8. Set **Permissions**:
   - **Type:** Choose one of the following (Authenticated, Anonymous, Restricted, Everyone).
   - **Users Field:** Select users who have access to the item.
   - **Groups Field:** Select groups that have access to the item.

**Note:**  
Entries with **system ownership** will inherit all their settings from the source.  
Example: If the type is a View, it will adopt its settings from the view configuration.

## Arranging Sidebar Items

To arrange items in the sidebar using the **Links Entity**, follow these steps:

1. Log in to the platform with an admin account.
2. Navigate to the **Sidebar**.
3. Click on the **Entities** section.
4. Access the **Links Entity**.
5. Adjust the **Order Field** values of existing entries as needed.

## Viewing Sidebar Items

Items will be displayed in the sidebar based on the **Order Field**, sorted from smallest to largest.

By following this guide, you can easily and effectively manage and organize items within the sidebar.
