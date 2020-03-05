# Publishing in Studio

Instantly Publish API Descriptions, Models, and supplemental Markdown files and images. One-click publish significantly reduces time to production and produces beautiful, modern, developer-centric documentation.

![Publishing Preview](../../assets/images/publishing.png)

## How

1. Open an existing **Git Project** or create a new Git Project
2. Click the **Publish** button on the top nav bar
3. Enable the **Show Preview** option to see how things will look (optional)
4. Click the **Publish** button

## Published Documentation URL

```
https://stoplight.io/p/docs/gh/{org}/{project}
```

## Documentation Hierarchy/Structure

How files in Studio will be displayed in your documentation.

### I. Markdown

```
1. Untagged Markdown files (ordered alphabetically by filename)
2. Markdown Groups (ordered alphabetically by tag name)
    a. Tagged Markdown files (ordered alphabetically by filename)
```

### II. API References

````
1. API Description Documents (ordered alphabetically by filename)
    a. Tagged Endpoint Groups (ordered alphabetically by tag name)
        i. Tagged Endpoints (Get, Post, Put, Patch, Delete, then additional operations as they occur in the spec)
        ii. Tagged Models (ordered alphabetically by filename)
    b. Untagged Endpoints (placed in ```Other``` Group, Get, Post, Put, Patch, Delete, then additional operations as they occur in the spec)
    c. Untagged Models  (placed in ```Other``` Group, ordered alphabetically by filename)
````

Read about [publishing via Continuous Integration](./07-publish-via-ci.md).
