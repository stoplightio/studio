---
tags: []
---

# Work with Files

Studio supports API design and documentation files in multiple formats:

- **API**: API description documents (YAML or JSON)
- **Endpoint**: Individual paths and operations (YAML or JSON)
- **Model**: Reusable API components (YAML or JSON)
- **Article**: Supplemental Markdown files (Markdown)
- **Image**: Supplemental images (JPEG, JPG, PNG, and GIF)
- **Style Guides**: For customizing the [validation and linting](../Design-and-Modeling/08-validation-style-guide.md)
- **Configuration Files**: For Stoplight project configuration and table of contents. 

<!-- theme: Warning -->
>**Warning**: You may be able to upload other file types, but they may not be rendered in Studio or in published documentation.

## Directory Structure

Projects are organized into three areas:

- **APIs**: Lists API descriptions and models.
- **Docs**: Lists Markdown and image files.
- **Files**: List all files.

## Add a File

1. Edit a project.
2. Select **Add ( + )**, and then select the type of file to add.

### API
Provide a name and the OpenAPI version. Choose YAML or JSON format or select **Import Existing** to add an existing YAML or JSON OpenAPI file.

### Endpoint
Select the API to add the endpoint. Select or create a tag to group similar endpoints together. Provide a path. 

### Model
Provide a name, then select or create a tag to group similar models together. Select a scope. (Common models are accessible to all APIs within your project.) Choose YAML or JSON format or select **Import Existing** to add an existing YAML or JSON OpenAPI file.

### Article
Provide a short title and a tag to group similar articles together.

### Image
If your project is connected to a public Git repository, use the **Import File** option to add images. Otherwise, drag-and-drop images onto Markdown files to add them to Stoplight. See [adding images](https://meta.stoplight.io/docs/platform/ZG9jOjc3MTg0NjE-add-images) for details.

### Stoplight Config
Used to control file locations and exclude locations from being analyzed by Stoplight. See [Configure Projects](https://meta.stoplight.io/docs/platform/ZG9jOjE4ODEyNA-configure-projects).

### Table of Contents
Used to configure the project sidebar. See [Project Sidebar](https://meta.stoplight.io/docs/platform/ZG9jOjIxOTkxNTkz-project-sidebar).


### File
Create a generic file. 
- **Folder**: Use to organize content. 
- **Import File**: Use to add images and other files.
- **Import Directory**: Import a directory of files to your project.  


