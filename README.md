# Stoplight Studio 

[![Buy us a tree](https://img.shields.io/badge/Buy%20us%20a%20tree-%F0%9F%8C%B3-lightgreen)](https://offset.earth/stoplightinc)

<!-- markdown-link-check-disable -->
To report a bug, please go to https://support.stoplight.io/hc/en-us/requests/new.
<!-- markdown-link-check-enable -->

Studio is Stoplight's next generation application for API design, modeling, and technical writing. A primary goal of Studio is to enrich, not replace, your existing workflows. When running locally it works fully offline, with folders and files on your computer just like your favorite IDE. When running in the browser, the web-native Git support allows you to effortlessly work with your existing repositories safely and efficiently.

## Features

### Full Support for OpenAPI v2 and v3

Studio comes with full support for the OpenAPI versions 2 and 3 specification formats for all functionality. That means full validation, mocking, and modeling support for both versions of the OpenAPI specification.

![Studio loves Swagger + OpenAPI](assets/images/openapi_swagger_equal_heart.png)

### Graphical API Design

Form-based designing means you don't need to be an OpenAPI expert to get started. Studio has a "write" (code) mode with full OpenAPI autocomplete, and a "read" mode for visualizing HTTP operations and models.

![Graphical Design for OpenAPI](assets/images/form-editor.png)

To find out more about how you can quickly design and prototype APIs without writing a single line of JSON or YAML, see [here](https://meta.stoplight.io/docs/platform/ZG9jOjM2OTM3Mjg5-overview).

### JSON Schema Modeling

Studio is not just for APIs, you can also create and modify standalone JSON Schema files for storing data models. Did we mention that this is also powered by the graphical interface? No more searching for the matching bracket or the missing space, and no need to be familiar with the in's and out's of JSON Schema.

![](assets/images/jse-sample.png)

### Encourage Reuse, Avoid Duplication

When it comes to API modeling, avoiding duplication of effort can be the difference between success and failure. How can you enforce consistency if all of your endpoints re-create the same model in slightly different ways? (hint, you can't)

![Studio's graphical JSON schema editor allows you to quickly find models to reference](assets/images/jse-sample2.png)

Studio allows you to quickly and easily find and reuse the objects you need, as you need them. No more recreating models for different endpoints, no more having to update dozens of different endpoints because a new field was added.

To find out more about how you can leverage references to scale your API consistency, see [here](https://meta.stoplight.io/docs/platform/ZG9jOjIyNTY5MzIw-shared-components).

### Technical Documentation

Mix API Reference Documentation and Markdown-based guides, how-tos, getting started information, etc. All of your documentation can live together in the same project. Studio includes a built-in Markdown editor, image manager, and the ability to publish documentation to Stoplight's new documentation platform.

![Create beautiful and easy-to-use API reference documentation](assets/images/technical-documentation.png)

You can even host the files in your own Git repository, and then publish when you're ready to show off your latest and greatest.

To find out more about writing technical documentation in Studio, see our getting started guide [here](https://meta.stoplight.io/docs/platform/ZG9jOjU4NzU5Mg-types-of-documentation).

### Style Guides and Validation

Enforce correctness and best practices with Style Guides, powered by the native [Spectral](https://stoplight.io/spectral/) integration that alerts you to errors the moment they are created.

![Spectral validates and lints your APIs to ensure they are correct and functional](assets/images/spectral1.png)

Clicking on errors or warnings also brings you to exactly where they are located in the document, making it easy to fix errors at the source.

To find out more about Stoplight Style Guides and how validations can improve your API design workflow, see [here](https://meta.stoplight.io/docs/platform/ZG9jOjMwMDI3MjA2-overview).

### Built-in Mocking

When running locally, Studio will automatically start a local [Prism mock server](https://stoplight.io/prism/) for every API defined in your project, and keep that mock server up to date as you change your designs.

![Mocking allows you to quickly test the look and feel of your API before jumping into the code](assets/images/studio-mocking.png)

To find out more about Prism and how mocking can be used to streamline your API development process, see [here](https://meta.stoplight.io/docs/platform/ZG9jOjM2OTM3Mjg4-work-with-mock-servers).

### Bring Your Own Repository

Since Studio works with your local files ystem, you can open up your API projects and start adding docs and designs alongside the actual implementation they are meant to describe. Once you're done, check it all into Git with your favorite Git client!

## License

<a rel="license" href="https://creativecommons.org/licenses/by-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Stoplight Studio</span> by <a xmlns:cc="https://creativecommons.org/ns#" href="https://stoplight.io/studio" property="cc:attributionName" rel="cc:attributionURL">Stoplight.io</a> is licensed under a <a rel="license" href="https://creativecommons.org/licenses/by-nd/4.0/">Creative Commons Attribution-NoDerivatives 4.0 International License</a>.
