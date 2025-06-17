---
title: "Summaries and Dashboards"
sidebar_position: 11
---

# Summaries and Dashboards

Summaries and dashboards are essential analytical tools provided by the platform. They offer various functions and graphical representations applied to data based on specific conditions and arrangements.

## Adding an Entity Summary {#adding-entity-summary}

After creating the entity, the "Dashboard" tab appears within the entity. Follow these steps to add a new summary:

1. Click on the "Add New Summary" button.
2. Add the summary information:
   - **Title**: The title of the summary.
   - **Icon**: An optional icon for the summary.
   - **Description**: An optional description for the summary.
   - **Source**: Either all entity entries or entries filtered via a query.
   - **Field**: The field on which the function will be applied.
   - **Function**: Select the appropriate function from the following options:
     - Count
     - Sum
     - Minimum
     - Maximum
   - **Group By**: You can group by entity fields or entry metadata.
   - **Order**: Ascending or descending.

**Note**: Enabling the "Show in Overview Tab" option displays this summary in a special tab that appears in the gallery, but gallery settings must be adjusted for the tab to appear. For more information on creating views, [click here](../../guide/information-structures-concepts/basic-concepts/views).

## Summary Types {#summary-types}

The appearance of summaries changes upon creation based on the display field chosen. Available display types include:

1. Result entries as a plain number.
2. Display as a list.
3. Display as a chart, which includes:
   - Column
   - Sidebar
   - Line
   - Pie

## Adding a Group {#summary-groups}

After creating several summaries, you can create a group to appear as a single block. Using drag-and-drop, multiple related summaries can be placed within one group, and the group can be given a distinctive name.

## Building an Entity Dashboard {#entity-dashboard}

The dashboard, which contains the summaries, will automatically appear in the "Dashboard" tab after adding summaries and grouping them. You can add, modify, or delete a summary or group from the dashboard. The dashboard is also displayed at the entity level from the gallery settings.

## Building a Module and System Dashboard {#system-and-module-dashboards}

### Module-Level Dashboard

A module-level dashboard aggregates information from all entities within the same module. To create it, follow these steps:

1. Go to the "Dashboard" tab at the module level.
2. Add summaries related to different entities.
3. When adding a summary, a field appears to select the entity from which you want to obtain a pre-built summary. This way, the dashboard is built.

### System-Level Dashboard

A system-level dashboard is created through pages and adding content to them. When configuring settings, choose the module, then select the entity, and then select the appropriate dashboard. For more information on creating pages, [click here](./pages.md).
