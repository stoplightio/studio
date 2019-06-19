---
tags: [01. Using Markdown]
---

# Markdown Basics

All of the notes, descriptions, and content fields in the Stoplight editors support use of [Stoplight Flavored Markdown](./stoplight-flavored-markdown.md).

### What is Markdown?

> Markdown is a text-to-HTML conversion tool for web writers.
> 
> Markdown allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML).

For example, this entire page was created using Markdown and HTML!

Below is a quick reference of all the Markdown syntax that is supported by Stoplight.

### Table of Contents

- [Headers](#headers)
- [Emphasis](#emphasis)
- [Lists](#lists)
- [Images](#images)
- [Code and Syntax Highlighting](#code-and-syntax-highlighting)
- [Tables](#tables)
- [Blockquotes](#blockquotes)
- [Inline HTML](#inline-html)
- [Horizontal Rule](#horizontal-rule)
- [Line Breaks](#line-breaks)
- [Videos](#videos)

## Headers

# H1

## H2

### H3

#### H4

##### H5

###### H6

## Emphasis

Emphasis, aka italics, with _asterisks_ or _underscores_.

Strong emphasis, aka bold, with **asterisks** or **underscores**.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~

## Lists

1. First ordered list item
2. Another item
    - Unordered sub-list
3.  Actual numbers don't matter, just that it's a number
    1.  Ordered sub-list
4.  And another item

    You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

## Links

There are two ways to create links:

[I'm a basic link](https://www.google.com)

[Hover over me to see my link title](https://www.google.com "Google's Homepage")

[I'm a relative link to the ./stoplight-flavored-markdown.md file](./stoplight-flavored-markdown.md)

## Images

Here's our logo (hover to see the title text):

![Stoplight Logo](https://pbs.twimg.com/profile_images/641056907474538498/qIbg0pZP_bigger.png "Stoplight Logo")

## Code and Syntax Highlighting

Inline `code` has `back-ticks` around it.

Blocks of code are either fenced by lines with three back-ticks, or are indented with four spaces. We recommend only using the fenced code blocks -- they're easier to use and support syntax highlighting.

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

Use language tags to change the syntax highlighting:

```json
{
  "JSON": "Syntax Highlighting"
}
```

## Tables

Colons can be used to align columns.

| Tables        |      Are      |  Cool |
| ------------- | :-----------: | ----: |
| col 3 is      | right-aligned | $1600 |
| col 2 is      |    centered   |   $12 |
| zebra stripes |    are neat   |    $1 |

There must be at least 3 dashes separating each header cell. The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown.

| Markdown | Less      | Pretty     |
| -------- | --------- | ---------- |
| _Still_  | `renders` | **nicely** |
| 1        | 2         | 3          |

## Blockquotes

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can _put_ **Markdown** into a blockquote.

## Inline HTML

You can also use raw HTML in your Markdown, and it'll mostly work pretty well.

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

## Horizontal Rule

Three or more asterisks or hyphens...

* * *

### Credits

Most of this information was pulled from [Adam Pritchard's Mardkown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). Thank you Adam for putting together this cheatsheet!