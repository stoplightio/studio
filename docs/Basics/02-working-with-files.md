---
tags: []
---

<!-- Ready for platform migration -->

# Work with Files

Once you create a project, add files to start designing APIs and documentation. 

Studio supports files in multiple formats:

- **API**: API description documents (YAML or JSON)
- **Endpoint**: Individual paths and operations (YAML or JSON)
- **Model**: Reusable API components (YAML or JSON)
- **Article**: Supplemental Markdown files (Markdown)
- **Image**: Supplemental images (JPEG, JPG, PNG, and GIF)
- **Style Guides**: For customizing the [validation and linting](../Design-and-Modeling/08-validation-style-guide.md)
- **Configuration Files**: For Stoplight project configuration and table of contents

<!-- theme: Warning -->
>**Warning**: You can upload other file types, but they may not be rendered in Studio or in published documentation.

## Directory Structure

Projects use a default file directory structure. 

- `/reference` - Where API descriptions documents (OpenAPI and JSON Schema) are stored
- `models` - Where shared modles are stored
- `/docs` - Where articles (Markdown files) are stored
- `/assets/images` - Where images are stored

If you have an existing repository with Markdown, image, or API description documents that do not adhere to the format above, you will need to move the files to their corresponding directories for Studio to recognize them, or create a [Stoplight Configuration file](../Basics/03-stoplight-config.md) to change them.

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
If your project is connected to a public Git repository, use the **Import File** option to add images. Otherwise, drag-and-drop images onto Markdown files to add them to Stoplight. See [Add Images](https://meta.stoplight.io/docs/platform/ZG9jOjc3MTg0NjE-add-images) for details.

### Stoplight Config
Used to control file locations and exclude locations from being analyzed by Stoplight. See [Configure Projects](https://meta.stoplight.io/docs/platform/ZG9jOjE4ODEyNA-configure-projects).

### Table of Contents
Used to configure the project sidebar. See [Project Sidebar](https://meta.stoplight.io/docs/platform/ZG9jOjIxOTkxNTkz-project-sidebar).

### File
Adds a generic file to the tree. Unsupported file types will not be rendered in published documentation, but you can add information that may be useful to your project.

### Folder
Adds a folder that you can use to organize content. This is especially useful for documentation files. Keep in mind that if you want to use a custom folder structure, you must use a [project configuration file](https://meta.stoplight.io/docs/platform/ZG9jOjE4ODEyNA-configure-projects).

### Import File 
Use to add images and other files. Files are automatically organized by type. For example, Markdown files are automatically added to the `docs` directory; image files are automatically added to the `assets` folder. 

### Import Directory
Imports a directory of files to your project. This is useful for migrating content into Stoplight. 


