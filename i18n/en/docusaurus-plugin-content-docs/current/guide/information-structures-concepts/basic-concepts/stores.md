---
title: "Stores"
sidebar_position: 26
---

# Stores
## Data Stores
**Data Stores** are dedicated units for storing inputs related to entities within the system. These stores are categorized by type to define the scope of sharing and permissions associated with each store. This provides a flexible and organized way to store and manage inputs, helping to efficiently organize data.

(For more on operations related to stores, refer to: [Store Management](../../data-management/stores.md))

## How Data Stores Work

**1. Priority**
- Storage priority is determined using the **weight field**.
- The store with the highest weight takes priority for data storage.
- If a shared store has a higher weight than a public or private store, new inputs are automatically stored in it.

**2. Automatic Configuration**
- The **public store** and **private store** are automatically created with each entity, reducing the administrative effort required from the user.

**3. Integration with Spaces**
- **Public Store**: Available to all spaces within the system.
- **Private Store**: Restricted to the entity's primary space.
- **Shared Store**: Available only to the spaces specified during its creation.

## Benefits of Data Stores

**1. Data Organization**
- Data stores allow inputs to be categorized based on sharing scope, making it easier to manage and filter data as needed (public, private, shared).

**2. Customization Flexibility**
- Administrators can adjust store weights to define storage priorities.
- It allows selecting participating spaces when creating a shared store.

**3. Enhanced Collaboration**
- The **shared store** provides a collaborative environment between different spaces while maintaining the independence of public and private stores.

**4. Priority Control**
- Through weights, storage priorities can be managed easily and flexibly, optimizing performance when handling multiple data sets.


## Data Stores Types
There are three main types of data stores within the system:

### 1. Public Store
- Automatically created with the entity.
- Allows data storage accessible from all spaces within the system.
- The administrator can only modify the **weight** to set storage priority compared to other stores.

### 2. Private Store
- Automatically created with the entity.
- Dedicated to storing data accessible only within the specified primary space.
- The administrator can only modify the **weight** to set storage priority compared to other stores.

### 3. Shared Store
- Defined by the administrator when needed.
- Allows data sharing between specific spaces selected during store creation.
- The administrator specifies the participating spaces and sets the **weight** to determine its priority compared to other stores.

## Related Concepts
- [Entities](./entities.md)
- [Views](./views.md)

**Note: For more on stores operations, see: [Stores Management](../../data-management/stores.md)**