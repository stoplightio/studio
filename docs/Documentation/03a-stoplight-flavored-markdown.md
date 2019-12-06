# Stoplight Flavored Markdown

Stoplight flavored markdown (SMD for short) was created with a couple of guiding principles in mind:

1.  SMD is human readable. A human with a simple text editor can easily read and write smd.
2.  SMD degrades gracefully. For example, SMD documents rendered by `github.com` should be clean and readable. No ugly templating syntax, etc.

**The Approach:**

1.  Stoplight flavored markdown extends github flavor markdown with inline comment annotations.
2.  The value inside of the annotations is a yaml object, and the annotation affects the markdown block that directly follows it in the document.

By leveraging comments to store annotations, Stoplight flavored markdown degrades gracefully to any other markdown renderer (Github, for example).

## Callouts

A callout is a md block quote with an optional annotation that indicates intent.

```md
<!-- theme: danger -->

> ### Danger Will Robinson!
>
> Here is my danger callout!

<!-- theme: warning -->

> ### Watch Out!
>
> Here is my warning callout!

<!-- theme: success -->

> ### Mission Accomplished!
>
> Here is my success callout!

<!-- theme: info -->

> ### A thing to know
>
> Here is my info callout
```

<!-- theme: danger -->

> ### Danger Will Robinson!
>
> Here is my danger callout!

<!-- theme: warning -->

> ### Watch Out!
>
> Here is my warning callout!

<!-- theme: success -->

> ### Mission Accomplished!
>
> Here is my success callout!

<!-- theme: info -->

> ### A thing to know
>
> Here is my info callout

## Code Blocks

A smd code block is md code fence with an optional annotation to tweak the presentation of the code block.

<!-- theme: warning -->

> In the examples below, remove the `\` that precedes the three backticks at the start and end of the javascript code fence before using.

````md
<!--
title: "My code snippet"
lineNumbers: true
highlightLines: [[1,2], [4,5]]
-->

\```javascript
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
\```
````

<!--
title: "My code snippet"
lineNumbers: true
highlightLines: [[1,2], [4,5]]
-->

```javascript
function fibonacci(num) {
  var a = 1,
    b = 0,
    temp;

  while (num >= 0) {
    temp = a;
    a = a + b;
    b = temp;
    num--;
  }

  return b;
}
```

## Tables

Use a type annotation to add a title to a table.

```md
<!-- title: My Table Title -->

| Tables        |      Are      |   Cool |
| ------------- | :-----------: | -----: |
| col 3 is      | right-aligned | \$1600 |
| col 2 is      |   centered    |   \$12 |
| zebra stripes |   are neat    |    \$1 |
```

<!-- title: My Table Title -->

| Tables        |      Are      |   Cool |
| ------------- | :-----------: | -----: |
| col 3 is      | right-aligned | \$1600 |
| col 2 is      |   centered    |   \$12 |
| zebra stripes |   are neat    |    \$1 |

## JSON Schema

A JSON schema block is a `json` code block with an additional `json_schema` language tag. The contents of the code fence should be the JSON schema object to be rendered. The primary language tag can be `yaml`, `yml`, or `json`.

<!-- theme: warning -->

> In the examples below, remove the `\` that precedes the three backticks at the start and end of the json code fence before using.

````md
\```json json_schema
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
\```
````

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
  "required": ["id", "name"]
}
```

## Tabs

A tab container is a `tab` annotation, followed by the tab content, and closed by a final `tab-end` annotation.

<!-- theme: danger -->

> Tab containers cannot be nested.

````md
<!--
type: tab
title: Schema
-->

\```json json_schema
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
\```

<!--
type: tab
title: Example
-->

\```json
{
"id": "xxx",
"name": "Chris",
"age": 27
}
\```

<!-- type: tab-end -->
````

<!--
type: tab
title: Schema
-->

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
  "required": ["id", "name"]
}
```

<!--
type: tab
title: Example
-->

```json
{
  "id": "xxx",
  "name": "Chris",
  "age": 27
}
```

<!-- type: tab-end -->

## HTTP Request Maker

The HTTP Request block allows you to embed example requests directly in your articles.

The HTTP Request block is a `json` or `yaml` code block with an additional `http` language tag. The contents of the code fence should be a HTTP request object (format described below). The Stoplight Studio markdown preview panel includes an embedded editor to help you put together

<!-- theme: warning -->

> In the examples below, remove the `\` that precedes the three backticks at the start and end of the yaml code fence before using.

````
\```yaml http
{
  "method": "get",
  "url": "http://todos.stoplight.io/todos"
}
\```
````

**Renders an embedded request maker!**

```yaml http
{ "method": "get", "url": "http://todos.stoplight.io/todos" }
```

**HTTP request object format:**

```json json_schema
{
  "title": "HTTP Request Object",
  "description": "This object describes the example request that you would like to embed.",
  "type": "object",
  "properties": {
    "method": {
      "type": "string",
      "enum": ["get", "post", "put", "patch", "delete", "options", "head"]
    },
    "url": {
      "type": "string"
    },
    "query": {
      "type": "object"
    },
    "headers": {
      "type": "object"
    },
    "body": {
      "type": ["object", "string"]
    }
  },
  "required": ["method", "url"]
}
```

---

_FIN._
