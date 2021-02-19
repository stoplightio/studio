---
tags: []
summary: "Using images in Stoplight is now easier than ever. Add images to your project to create beautiful documentation layouts that supplement text content."
---

# Using Images

<!-- theme: warning -->

> ### Limitations
>
> Currently Stoplight Docs only supports displaying images within public Git repositories. If you're working in a private Git repository, you'll need to host the images on a public cloud service such as Imgur or Amazon S3.
>
> If you'd like for us to prioritize this feature, please give it a vote on our public roadmap: https://roadmap.stoplight.io/c/100-display-images-from-private-git-repositories

## What

Using images in Stoplight is now easier than ever. Add images to your project to create beautiful documentation layouts that supplement text content.

## How

> If you already have image files stored in a cloned Git Repository, adhere to the [Studio Directory Structure](02-directory-structure.md) to access those files in Studio

### Add Images

![Create New Image](../../assets/images/images.png)

1. Select the **+** button in the top left
2. Select **Image** from the dropdown
3. Select the image you want to upload from the file explorer
4. Click **Open**

Alternatively, you can right click the Images folder and select **Import**. By default, images will be stored in the `assets/images` folder in your file tree.

### Place Images in Markdown Files

1. Select the markdown file you wish to add images to
2. Input `![Alt Text](File Location)` to place the image

> Example: `![Ref a model](../../assets/images/ref-customer.png)`
