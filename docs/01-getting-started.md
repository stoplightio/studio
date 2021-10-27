# Getting Started

## Creating Your First Project

The quickest way to get up and running with Studio is to clone an existing Git repository. If you're running Studio Desktop, you can choose a location on your computer where a repository already exists. In Studio Web or Desktop, you can copy the URL to any GitHub, Bitbucket, GitLab, Gitea, or other Git repository. 

Give it a shot with our sample project:

1. In Studio Web, select the **Add Project** icon at the top of the left navigation pane. 
   ![](../assets/images/add-project.png)
2. Select **Add from GitHub**, add the studio-demo URL, and then select **Add Git Project**.
   ```
   https://github.com/stoplightio/studio-demo

   ```
   ![](../assets/images/add-demo-project-web.png)

   In Studio Desktop, paste the URL into the Open Git Project page, and then select **Clone**.
   ![](../assets/images/studio-open-git-project-pre-filled.png)

3. Explore the demo documentation, APIs, and schemas. 

   ![Overview of the Studio landing page](../assets/images/studio-web-landing.png)

> Note that the screenshot above is of Studio Web. There are slight differences in Studio Desktop.

4. Select **Edit** to begin working with API designs, documentation, models, and more.


## Creating an API

To create a new API:

1. Select the **Add** icon, and then select **API**.

![Create an API from Studio Web](../assets/images/studio-web-create-api.png)

From there you can name your API, and then optionally set the specification version (OpenAPI v2 or v3) and storage format (JSON or YAML).

![New API menu](../assets/images/studio-new-api.png)

After clicking "Create", a new API description document will be created and added to the project. From there you can then set the global information about the API and get started adding your first operation.

Continue on to the [API Design Guide](./Design-and-Modeling/01-getting-started.md) to get started designing APIs.
