# Publishing in Studio

When changes are made to your API descriptions or Markdown documentation, whether that is done in Stoplight Studio or anywhere else, you want to get those changes reflected in Documentation, Mock Servers, Explorer, the Design Library, etc.

The publishing method you use depends on your project type:

* **Git Projects**: Use webhooks to trigger automatic publishing for projects using Git. You can push changes to the default branch set in Stoplight or to any other branch which has publishing enabled. 
* **Stoplight Projects**: Publish changes as soon as they are made in Studio Web. 
* **CLI Projects**: Use the Stoplight CLI to publish local projects, projects that do not use Git, or to facilitate continuous integration. You can also use the Stoplight CLI to automate publishing directly from GitHub.

Note that nodeJS version 12 or greater is required to run the CLI. You can
verify your version using the command: `node --version`

> **Learn More**
> 
> [Publish Overview](https://meta.stoplight.io/docs/platform/ZG9jOjQ1NTQxNA-publishing)
> 
> [Add Projects in Studio Web](https://meta.stoplight.io/docs/platform/ZG9jOjE4ODEyMw-add-projects)
> 
>[Add Projects in Studio Desktop](../Basics/01-working-with-projects.md)


