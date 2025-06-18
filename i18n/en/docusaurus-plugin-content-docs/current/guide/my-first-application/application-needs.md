---
title: "Application Requirements"
sidebar_position: 2
---

# Application Requirements

When building a Task Management Application on the platform, it requires some essential components and preparations before and during the development process. This document outlines these needs.

## Application Components from the Platform's Perspective

### Entities

**Task Entity**

| Field Name | Required | Type |
|------------|----------|------|
| Title | :white_check_mark: | Text |
| Description | :white_check_mark: | Long Text |
| Status | :white_check_mark: | Category (To Do, In Progress, Completed) |
| Assigned To | :white_check_mark: | User Group |
| Completion Date | :white_check_mark: | Date |

### Reactions

**Internal Notification for Assigned Task**
- Sends a notification to the employee via the platform to inform them of the new task.

**External Notification for Assigned Task**
- Sends a notification to the employee via email to inform them of the new task.

### Queries

**User Task Query**
- Allows users to view their assigned tasks.

### Statistics

**Graph Showing Number of Assigned Tasks**
- Provides a graphical representation of the number of tasks assigned to the employee.

### Views

**Add Task View**
- Allows managers to add and assign tasks to employees through this view.

**Tasks View**
- Enables employees to view their assigned tasks.

### Reports

**Weekly Task Report**
- Generates a weekly report summarizing the tasks assigned to the user.

## Preparations Required Before Building the Application

### Adding Users and Defining Their Permissions
- Users are added to the system by system administrators and assigned appropriate permissions.
- Detailed instructions on adding users can be found [here](../../guide/information-structures-concepts/basic-concepts/users).
