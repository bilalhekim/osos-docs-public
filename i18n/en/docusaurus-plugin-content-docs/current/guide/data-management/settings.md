---
title: "Settings"
sidebar_position: 28
---

# Settings Operations

## Defining a New Language
Administrators can define a new language that can be selected for the organization, a specific space, or an individual user.

### Steps:
1. From the sidebar, go to **General**.
2. Click on the **Languages** tab.
3. Press the **Add Language** button.
4. A form will appear requiring the following information:
   - **Language Name:** Enter a localized name familiar to users of the language.
   - **Flag:** Select the appropriate flag for the language.
   - **Language Code:** Enter the standard language code (e.g., EN, AR).
   - **Direction:** Specify the text direction (Right-to-Left RTL / Left-to-Right LTR).
   - **Default:** Enable this option to set this language as the default.
   - **Web Translation File:** Upload the translation file for the web.
   - **Mobile App Translation File:** Upload the translation file for mobile apps.


## Defining a New Time Zone
Administrators can add a new time zone.

### Steps:
1. From the sidebar, go to **General**.
2. Click on the **Time Zone** tab.
3. Press the **Add Time Zone** button.
4. A form will appear requiring the following information:
   - **Time Zone:** Add the time zone.
   - **Zone Number:** Enter the unique zone number.
   - **Time Offset:** Specify the time difference.
   - **Winter Time:** Enable this option if needed.


## Managing Fonts
The **Fonts Entity** is used to define new fonts that can be selected within various system themes. The system supports adding multilingual fonts with different file types like WOFF and TTF to ensure compatibility across different use cases.

### Steps to Add a New Font:
1. From the sidebar, go to **General**.
2. Click on the **Fonts** tab, then press **Add New Font**.
3. A form will appear with the following fields:
   - **Font Name:** Mandatory field, supports multiple languages, must be unique.
   - **Language:** Select a language from the predefined list in the **Languages** tab.
   - **Font Files:**
     - WOFF: Required upload.
     - WOFF2: Required upload.
     - TTF: Required upload.
     - OTF: Required upload.
4. Fill in the required fields and upload the files.
5. Click **Save** to add the font to the system.
6. The new font will appear in the fonts list.


## Managing Themes
The system allows theme management to customize the user interface according to user needs. Administrators can add new themes, select available themes, and define the default theme for each scope (Space, Organization, or User).

### Steps:
1. From the sidebar, go to **General**.
2. Click on the **Themes** tab, then press **Add New Theme**.
3. A form will appear requiring the following information:
   - **Theme Name:** Mandatory, supports multiple languages, must be unique.
   - **Dark Mode:** Enable this option to set the theme to dark mode.
   - **Fonts Used:** Select a font from those defined in the **Fonts** tab.
   - **General Layout:**
     - **Day Mode Colors for Mobile:**
       - Primary Color
       - Secondary Color
       - Additional Color
       - Text Color
     - **Night Mode Colors for Mobile:**
       - Primary Color
       - Secondary Color
       - Additional Color
       - Text Color
     - **App Font**
4. Click **Save** to add the new theme.
5. The added theme will appear in the themes list.


## System Settings
The **Settings** tab allows configuration at the Space, Organization, or User level. These settings include default themes, languages, time zones, and date/time formats.

### Steps to Add a New Setting:
1. From the sidebar, go to **General**.
2. Click on the **Settings** tab, then press **Add New Setting**.
3. A form will appear with the following fields:
   - **Scope:** Choose one of the following:
     - **Space:** Settings apply only to the selected space.
     - **Organization:** Settings apply only to the selected organization.
     - **User:** Settings apply only to the selected user.
   - Additional fields will appear based on the selected scope:
     - **Space:** Select the space for the settings.
     - **Organization:** Select the organization for the settings.
     - **User:** Select the user for the settings.
   - **Available Themes:** Select available themes from the system-defined list.
   - **Default Theme:** Choose a default theme for the selected scope.
   - **Primary Language:** Select a language from the system-defined list.
   - **Time Zone:** Select a time zone from the predefined zones.
   - **Date & Time Format:** Choose from available formats.
   - **Date Format:** Choose from available formats.
   - **Time Format:** Choose from available formats.
4. Click **Save** to add the setting to the system.
5. The new setting will appear in the settings list.
