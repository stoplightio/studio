---
tags: []
---

# Linking Between Articles

Create hyperlinks to other Markdown files to create additional navigation within your documentation. All links are relative to the current file.

1. Select the **Markdown file** you wish to modify

2. Right click the file you're linking to and select "Copy Relative Path." To reference an element from within the API specification, first build the relative path to the `api.yaml` or `api.json` file (ie `../reference/api.yaml`) and then the path to the API endpoint call. *Note: copying the path does not include the HTTP request method. You will need to append that yourself.*


  ![image](https://user-images.githubusercontent.com/273880/151421911-63d8cc54-4407-493a-821d-d94ce07eaf13.png)


3. Input `[Display Text](Hyperlink URL/File Location)`

> Link to Markdown Example: `[API Design Quickstart Guide](../Design-and-Modeling/01-getting-started.md)`

> API Method Example: `[creating a verification](../reference/api.yaml/paths/~1verification-requests/post)`
