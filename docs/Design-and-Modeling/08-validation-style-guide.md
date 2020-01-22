---
tags: []
---

# Validation and Linting

Studio will let you know if you've written invalid YAML, JSON, Markdown, or let you know if your API descriptions are invalid OpenAPI, JSON Schema, etc. Beyond simply validating this content, Studio can lint any JSON/YAML data, with a built-in ruleset for OpenAPI v2 and v3.

![Stoplight Studio screenshot showing a bunch of warnings and erros, like invaid $ref and missing contact information](../../assets/images/spectral.png)

Linting your API description during the design process provides a practical method for enforcing API design rules over multiple APIs, making your APIs consistent before they even exist.

Validation and linting can trigger either a warning (denoted by a yellow exclamation icon) or an error (denoted by a red exclamation icon) if the rules conditions are not met.

### Validation Rules

Validation rules signify whether your generic JSON/YAML, API descriptions, etc are technically correct. An example of a validation rule would be requiring a unique `operationIds` for every operation. Validation rules are denoted by a green check mark icon and typically trigger errors.

### Style Rules

Style rules are more like opinions, they are not about your OpenAPI being valid, they offer suggestions about naming conventions, missing information which would improve the quality of documentation, etc. Style rules are denoted by a blue pencil icon and typically trigger warnings when enabled.

> The Style & Validation rule engine is powered by our open-source project [Spectral](https://stoplight.io/open-source/spectral), and [custom rulesets](./08a-configure-spectral.md) can be created to produce "style guides" for any sort of JSON or YAML data, like OpenAPI or JSON Schema.
