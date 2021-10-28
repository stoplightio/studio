# Project UI Overview

Use projects to manage APIs, documentation, and related files. Projects work and look the same in Studio Web and Studio Desktop. This topic describes projects in Studio Web. 

To open a project:

1. From the **Home** page:
   - Select the project from the side panel on the left

     Or

   - Select **Projects** from the tab.

2. Project owners, admins, and editors can select **Edit** to manage the project. Viewers can navigate and read project content. 

Once you are editing a project, there are three key areas of the interface:

1. Project sidebar
2. Project toolbar
3. Editor panel

![Projects Overview](../assets/images/ui-overview.png)

# Project Sidebar

Switch between three tabs to view project content:

- **APIs** lists APIs, endpoints, and models
-  **Docs** lists Markdown and image files
- **Files** lists all project files

Select an item on any tab to open it in the Editor panel. 

# Project Toolbar

**Project Options**: Select the hamburger menu to work with these options:

* **Back to Workspace**: Select to leave edit mode and return to the workspace home.
* **Preferences**: 
  - Autosave
  - Show empty directories
  - Theme (Dark, Light, or the default set in Workspace settings)
  - Git (Auto-pull and Auto-translate SSH URLs)
  - Reclone Project
  - Download Project zip
   <!-- issues created to better document above list at a later time -->

**Search**: Find anything in your project files. 

**Add to Project**: Select to add new assets to your project. This includes APIs, endpoints, dodels, articles, style guides, images, table of contents, files and directories. You can also import files and import directories.

**Project Actions**: Changes depending on your state:
  - **Back to workspace**: Shows when no changes have been made to the project.
  - **Publish**: When the project is not connected to a repository, shows when at least one change has been made in the project. Select the down arrow to discard changes. 
  - **Commit and Publish**: When the project is connection to a repository, shows when at least one change has been made in the project. Select the down arrow to discard changes. 

**Project Name**: Shows the name of the current project. If the project is connected to a repository, the name of the burrent branch is also shown. Select the down arrow to pull changes into your project or to switch branches. 

# Editor Panel

**Primary Panel**: Main editor panel. Can switch between different "views" via the toggle in the top right of the panel (not shown, must hover over panel for toggle to appear).

**Secondary Panel**: Additional editor panel, which is only available on larger screens (width > 1400px). Can switch between view types via the view toggle in the top right of the panel, just like the Primary panel.

6. **Mock Server**: Run mock servers (powered by [Prism](https://stoplight.io/prism)) and view mock server logs.

7. **Validation and Linting**: Displays issues related to your API Specification (powered by Spectral). Click to expand window and view error and warning details and locations.





## Customizing the Interface Panels

![Panel Overview](../assets/images/panel-overview.png)

1. **File tree Panel**: Displays API Specifications, Endpoints, & Models (APIs Tab), Markdown & Image Files (Docs Tab), All Files (Files Tab)
2. **Main Panel**: Displays Form View, Read View, or Write View
3. **View Toggle**: Switch between Form View, Read View, or Write View
4. **Secondary Panel**: Displays Form View, Read View, or Write View (Only available for larger screens)

### What

Studio provides a customizable two panel (smaller screens) or three panel (larger screens) layout to give you control over what information you would like to display and where. Expand windows when focused on a single task. Switch between Read, Write, and Form Views for individual panels to maximize efficiency.

### How

1. Select an endpoint, model, or Markdown file.
2. Hover over the **Main** or **Secondary Panel**
3. Switch between view modes via the **View Toggle** buttons in the top right of the panel
