---
title: "Reports"
sidebar_position: 10
---

# Reports

Reports are an essential tool provided by the platform for studying and analyzing data based on set criteria and parameters. They are crucial outputs that the end user needs in any system as they present the report data in a tabular format.

## Creating a Report {#creating-a-report}

To create a report, follow these steps:

1. Navigate to the sidebar in the application.
2. Select "Administration."
3. Select "Applications."
4. Choose "Modules" from the sidebar.
5. Select the unit where you want to create the report.
6. Select the entity you want to report on.
7. Go to the "Reports" tab.
8. Click the "+" button to add a new report.
9. A page will appear with several sections for the report:

### Report Information

- **Title**: A mandatory field that can be written in both Arabic and English, and it should be the name of the report.
- **Description**: An optional field that can be written in both Arabic and English, describing the report.
- **Icon**: Optional field to choose an icon for the report.
- **Fields**: A mandatory field to select the fields that will be displayed in the report.

### Report Design

Choose the layout for the report through the report components:

#### Report Components

- **Page Header**: If enabled, select the page header from the organization entity in the main unit.
- **Organization Header**: If enabled, select the organization header from the organization entity in the main unit.
- **Report Header**: If enabled, specify the content type (text or image) and select the appropriate header.
- **Page Footer**: If enabled, select the page footer from the organization entity in the main unit.
- **Organization Footer**: If enabled, select the organization footer from the organization entity in the main unit.
- **Report Footer**: If enabled, specify the content type (text or image) and select the appropriate footer.
- **Report Layout**: A mandatory field to choose the report layout (horizontal or vertical).

#### Preview Report Layout

You can preview the report layout by activating each button in the first column, which will display the layout divisions based on each activation.

### Report Permissions

Set user access permissions for the report, containing two fields:
1. **Users**: A list of users in the system, allowing you to select users who can access the report.
2. **Groups**: A list of groups created within the system, allowing you to select groups that can access the report.

### Sending Options

Divided into two sections:

#### Schedule

1. **Interval Type**: A mandatory field to choose one of the following options:
    - **None**: No specific time set, and the report is not sent.
    - **Recurring**: Specify the time for sending the report repeatedly. When this option is selected, several fields appear:
        - **Schedule Expression**: Write a script expression indicating the required repetition time for sending the report.
        - **Start Date**: The start time for sending the report.
        - **End Date**: The end time for sending the report.
    - **One-time**: A new field appears to specify the time and date when the report will be sent.

#### Channel

- **Channel Type**: Specify the method of sending the report, currently the available option is email.
- **Subject**: A mandatory field for the report subject.
- **Content**: The content of the email to be sent.

### Recipients

Individuals who will receive the email containing the report, divided into three sections:

#### Recipient

The user or group of users who will receive the email containing the report:
- **Source**: A mandatory field to choose the recipient category (User, Group, List, Static).
- **Type**: Currently, the only option is static.
- **Value**: Specify the value based on the selected source.
- **Add New Recipient Button**: To add another recipient.

#### CC

To send a copy to another person, contains an "Add New Field Button" to add another recipient.

#### BCC

To send a blind copy to another person without the knowledge of other recipients, contains an "Add New Field Button" to add another recipient.

### Sending the Report

- **Send Report Link Button**: When enabled, the report is sent as a link within the email.
- **Send File as Attachment Button**: When enabled, a field appears to specify the attachment file type (Excel, PDF).

### Finalize and Save the Report

- Click the "Finish" button to display a confirmation message for saving the changes, then click "Confirm" to save the report.
- Click the "Publish" button to display the report to the end user and send it according to the date and time via email to the specified recipients.

## Accessing a Report {#accessing-a-report}

Reports can be accessed in several ways:
1. **Through Administration**: Go to Applications, select a specific unit, then select an entity, and the reports will appear.
2. **Through the End User**: Go to the sidebar, select a specific unit, then select the report.
3. **Through the link sent to the recipient**: Open the email, click the link to access the report.

## Exporting the Report

### Exporting the Report as an Excel File {#exporting-data-report}

To export the report as an Excel file:
1. Navigate to the sidebar.
2. Select the unit, then the report.
3. Click the button at the upper left corner (shaped like a "V").
4. Choose the "Export Report as Excel File" option to download the report as an Excel file to your device.

### Exporting the Report as a PDF {#exporting-pdf-report}

To export the report as a PDF file:
1. Navigate to the sidebar.
2. Select the unit, then the report.
3. Click the button at the upper left corner (shaped like a "V").
4. Choose the "Export Report as PDF" option to download the report as a PDF file to your device.
