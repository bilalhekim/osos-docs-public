---
title: "Relations"
sidebar_position: 12
---

# Relations
Relations in the platform refer to the link or connection between two entities, where the parent entity acts as the main entity, and the child entity is the subordinate entity. This relationship is used to create a connection between entities, allowing the parent entity to contain multiple values of the child entity. This relationship is established through the use of a reference field included in the child entity.

Relations are used to build nested organizational structures that allow data to be organized hierarchically. For example, the parent entity could represent an organization, and the child entities could represent its various departments or projects. This pattern allows data to be organized according to the hierarchical relationships between them, enabling the user to understand the organizational structure of entities in the platform.

## Important to Know
### Types of Relations
The types of relations in the system include outgoing relations and incoming relations, and here are the details of each type:

#### Outgoing Relations
Outgoing relations are the connections that link the current entity to another entity. The current entity contains a reference field pointing to the other entity. When an outgoing relation is created, it is automatically added to each reference field in the entity. This facilitates tracking the relations conveniently and systematically within the current entity.

#### Incoming Relations
Incoming relations are the connections that link the current entity to another entity, where the other entity contains a reference field pointing to the current entity as the source of the relation. The manager or supervisor defines and modifies these relations from the administration section. Incoming relations appear in a separate group from outgoing relations, helping to clarify the connections between entities.

By using these different types of relations, the system can effectively track and organize the connections between entities, simplifying the process of analyzing and browsing the data and their associations.

## Related Concepts
- [Entities](./entities.md)
- [Views](./views.md)


**Note: For more information on relations operations, see: [Relations Management](../../data-management/relations.md).**