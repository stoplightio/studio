# Getting Started

## Creating Your First Project

The quickest way to get up and running with Studio is to clone an existing Git repository. If you're running Studio Desktop then this could be choosing a location on your computer where a repository already exists. If you're running Studio Web you could copy the URL to any GitHub, Bitbucket, GitLab, Gitea, or other Git repository. 

Give it a shot with our sample project: 

```
https://github.com/stoplightio/studio-demo
```

Paste the URL above into the "Open Git Project" form when you open Studio, and click "Clone".

![Start from an existing Git repo](../assets/images/studio-open-git-project-pre-filled.png)

Assuming everything went to plan, you should now see a page resembling the one below.

![Overview of the Studio landing page](../assets/images/studio-web-landing.png)

> Note that the screenshot above is of Studio Web, so there may be some slight differences if you are using Studio Desktop.

You have just created your first project! Be sure to review the [UI Overview](./ui-overview.md) for quick highlights on the Studio user interface.

## Creating an API

To create a new API, use the menu immediately next to the project name and select "API".

![How to create an API from the Studio UI](../assets/images/studio-web-create-api.png)

From there you can name your API, and then optionally set the specification version (OpenAPI v2 or v3) and storage format (JSON or YAML).

![New API menu](../assets/images/studio-new-api.png)

After clicking "Create", a new API description document will be created and added to the project. From there you can then set the global information about the API and get started adding your first operation.

Continue on to the [API Design Guide](./Design-and-Modeling/01-getting-started.md) to get started designing APIs.
