---
title: "Data Stores"
sidebar_position: 25
---

# Data Store Management Procedures

## Creating a Shared Data Store
A shared data store can be created to be accessible to a specific group of spaces.

### Steps
1. Go to the **Entity Page**.
2. Open the **"Stores"** tab.
3. Click on **"Create Shared Data Store"**.
4. A window will appear containing the following fields:
   - **Name:** Store name (translatable text field).
   - **Description:** Store description (optional).
   - **Spaces:** Select the spaces that will have access to this store. *(At least two spaces must be selected)*.
   - **Store Weight:** A required numeric field to set priority.
5. After filling in the fields, click **"Save"** to create the store.


## Viewing Known Stores
The administrator can view all known stores (Public, Private, Shared) at the entity level.

### Steps
1. Go to the **Entity Page**.
2. Open the **"Stores"** tab.
3. The system will display a list of all known stores.
4. Click on the store name to view its details.


## Modifying Store Priority
**Priority:** Setting the weight allows control over storage priority when multiple stores exist.  
The administrator can adjust the **Store Weight** for Public, Private, or Shared stores to define their priority compared to others.
- End users and administrators can view and browse entries based on the stores available to their space.

### Steps
1. Go to the **Entity Page**.
2. Open the **"Stores"** tab.
3. Select the store whose priority you want to adjust.
4. Modify the **Store Weight** value to be higher than other stores (e.g., the Public Store).
5. Click **"Save"** to confirm the changes.


## Creating a New Entry Within a Shared Store
When creating a new entry, the system automatically stores it in the store with the highest priority.

### Steps
1. Ensure you are within a specific space.
2. Create a new entry at the entity level.
3. If the available stores include:
   - Public Store
   - Private Store
   - Shared Store with the highest weight  
   The system will automatically save the entry in the **Shared Store**.

## Viewing Stored Entries
Users can view all entries stored in the stores available to their space (Public, Private, Shared).

### Steps
1. Go to the **Entity Page**.
2. Browse entries from the **Entries List View**.
3. The system will aggregate entries from:
   - The **Public Store**.
   - The **Private Store**.
   - The **Shared Store**.
