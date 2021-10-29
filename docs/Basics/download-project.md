# Downloading Projects

Download a zip file of the current project if you need to save the contents of your project without pushing to a Git repository. 

To download a project in Studio Web:

1. Open a project in Edit mode.
2. From the Project Options hamburger menu, select **Download Project Zip**.

To download a project in Studio Desktop:

1. Open a project.
2. From the Project Options hamburger menu, select **Open project folder**.
3. Select **Open** to navigate to the folder.
4. Create a zip file of the foder contents. 

> The download process resolves $ref's in OpenAPI or JSON Schema files, so users of the design library will still see references to the models in the design library. For that, the [Export API](https://meta.stoplight.io/docs/platform/c.troubleshooting.md) option might be more appropriate.
