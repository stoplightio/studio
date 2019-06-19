---
tags: [01. Using Markdown]
---

# Stoplight Flavored Markdown (SMD)

### The Two Laws

1.  SMD is human readable. A human with a simple text editor can easily read and write smd.
2.  SMD degrades gracefully. SMD documents rendered on `github.com` should be clean and readable.

### The Approach

1.  Stoplight flavored markdown extends github flavor markdown with inline comment annotations.
2.  The value inside of the annotations is a yaml object, and the annotation affects the markdown block that directly follows it in the document.

By leveraging comments to store annotations, Stoplight flavored markdown degrades gracefully to any other markdown renderer (Github, for example).

## Callouts

A callout is a md block quote with an optional annotation that indicates intent.

<!-- theme: danger -->

> ### **Danger Will Robinson!**
>
> Here is my danger callout!

<!-- theme: warning -->

> ### **Watch Out!**
>
> Here is my warning callout!

<!-- theme: success -->

> ### **Mission Accomplished!**
>
> Here is my success callout!

<!-- theme: info -->

> ### **A thing to know**
>
> Here is my info callout

## Code Blocks

A smd code block is md code fence with an optional annotation to tweak the presentation of the code block.

<!--
title: "My code snippet"
lineNumbers: true
highlightLines: [[1,2], [4,5]]
-->

```javascript
function fibonacci(num){
  var a = 1, b = 0, temp;

  while (num >= 0){
    temp = a;
    a = a + b;
    b = temp;
    num--;
  }

  return b;
}
```

## JSON Schema

The smd json schema block is a md code block with an additional `json_schema` language tag. The contents of the code fence should be the json schema object to be rendered. The primary language tag can be `yaml`, `yml`, or `json`.

```json json_schema
{
  "title": "User",
  "type": "object",
  "properties": {
    "id": {
      "type": "string"
    },
    "name": {
      "type": "string",
      "description": "The user's full name."
    },
    "age": {
      "type": "number",
      "minimum": 0,
      "maximum": 150
    }    
  },
  "required": [
    "id",
    "name"
  ]
}
```

## Tables

Use a type annotation to add a title to a table.

<!-- title: My Table Title -->

| Tables        |      Are      |  Cool |
| ------------- | :-----------: | ----: |
| col 3 is      | right-aligned | $1600 |
| col 2 is      |    centered   |   $12 |
| zebra stripes |    are neat   |    $1 |

## Tabs

A smd tab container is a `tab` annotation, followed by the tab content, and closed by a final `tab-end` annotation.

<!-- theme: danger -->

> Tab containers cannot be nested.

<!--
type: tab
title: My First Tab
-->

The contents of tab 1.

<!--
type: tab
title: My Second Tab
-->

The contents of tab 2.

<!-- type: tab-end -->

---

*FIN.*