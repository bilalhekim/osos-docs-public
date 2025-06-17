---
title: "Templates"
sidebar_position: 22
---


# Templates
Templates allow you to export entity data in various formats, such as HTML, Word, or Excel. Below is a simplified guide on how to build these templates, with a clear separation of topics and steps.

## Building Templates
Before starting to build templates, you first need to set up the entity structure and add the required fields. You can then use specific expressions within the templates to display the values of these fields.



### 1. HTML Template

#### General Syntax
```html
<!DOCTYPE html>
<html>
<head>
    <title>HTML Template</title>
</head>
<body lang="en-US" dir="ltr">

    {{% for(entry of entries){ %}}
        <!-- Use entry.value.FIELD_NAME here -->
        {{%=entry.value.FIELD_NAME %}}
    {{% }; %}}

</body>
</html>
```

#### Example
```html
<!DOCTYPE html>
<html>
<head>
    <title>HTML Template Example</title>
</head>
<body lang="en-US" dir="ltr">

    {{% for(entry of entries){ %}}
        <h1>Title</h1>
        <p>{{%=entry.value.title %}}</p>
    {{% }; %}}

</body>
</html>
```
- In this example, the `title` field is used to display the heading.



### 2. Word Template

#### General Syntax
```text
<{{ALIAS FIELD_ALIAS INS $entry.value.FIELD_NAME}}>

<{{FOR entry in entries}}
{{* FIELD_ALIAS}}
{{END-FOR entry}}>
```
- **FIELD_ALIAS**: The alias name to be used later in the loop.
- **FIELD_NAME**: The identifier of the field within the entity (e.g., `title`).

#### Example
```text
<{{ALIAS title INS $entry.value.title}}>

<{{FOR entry in entries}}
{{* title}}
{{END-FOR entry}}>
```
- Here, a variable is defined to hold the value of the `title` field, which is then displayed within a loop.



### 3. Excel Template

#### General Syntax
```text
<${table:entries.value.FIELD_NAME}>
```
- **FIELD_NAME**: The identifier of the field (e.g., `title`).

#### Example
```text
<${table:entries.value.title}>
```
- This creates a table in the Excel file containing all values from the `title` field of existing records.



### General Notes
1. **FIELD_NAME** refers to the field name or its identifier (e.g., `title`).
2. Ensure that field names (or identifiers) match exactly between the entity and the expressions within the template.
3. These templates are executed within the system or tool that supports these formats, and upon export, the expressions will be replaced with actual field values.



## Adding the Template

Once you’ve created and prepared your template (HTML, Word, or Excel), you can add it to the entity by following these steps:

1. **Navigate to the Entity**  
   Go to the relevant entity page in the system.

2. **Open the Templates Section**  
   From the entity page, select the "Templates" tab or section.

3. **Add a New Template**  
   - Click the **"+"** icon to add a new template.  
   - A window will appear requesting the following information:

   1. **Name**  
      Enter a clear and descriptive name for the template.

   2. **Level**  
      Choose whether the template is intended to export:  
      - **Single Entry**: To export just one record.  
      - **Multiple Entries**: To export several records at once.

   3. **Type**  
      Select the file type for export:  
      - **Excel**  
      - **PDF**  
      - **Word**

      > **Note:**  
      > - If you select **Excel**, you must upload a pre-built Excel file.  
      > - For **PDF** or **Word**, you need to upload an **HTML** file (for PDF) or a **Docs** file (for Word).

   4. **Upload File**  
      Choose the template file you previously created.

   5. **Export Type**  
      - **Background Export**: The export runs in the background, and a notification is sent upon completion.  
      - **Immediate Export**: The export is triggered immediately when pressing the export button.

   6. **Advanced Settings**  
      Configure any additional settings related to the template type or data processing.

4. **Save Changes**  
   Click **"Save"** or the appropriate button to confirm and link the template to the entity.

> By following these steps, your new template will be available for use whenever you need to export entity data.

