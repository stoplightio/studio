---
tags: []
---

# Using Markdown in Documentation  

All of the notes, descriptions, and content fields in the Stoplight editors supports the use of [GitHub flavored Markdown](https://github.github.com/gfm/) and raw HTML. You can use Markdown to easily format your text content into beautiful documentation. 

### What is Markdown? 

> Markdown is a text-to-HTML conversion tool for web writers. Markdown allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML). 

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

```
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Emphasis 

```
Emphasis, aka italics, with *asterisks* or _underscores_. 

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~
```

Emphasis, aka italics, with *asterisks* or _underscores_. 

Strong emphasis, aka bold, with **asterisks** or __underscores__. 

Combined emphasis with **asterisks and _underscores_**. 

Strikethrough uses two tildes. ~~Scratch this.~~

## Lists 

(In this example, leading and trailing spaces are shown with dots: ⋅⋅⋅)

```
1. First ordered list item
2. Another item 
⋅⋅⋅* Unordered sub-list 
1. Actual numbers don’t matter, just that it’s a number 
⋅⋅⋅1. Ordered sub-list 
4. And another item 

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we’ll use three here to also align the raw Markdown). 

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this lien is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered lists can use asterisks 
- Or minuses 
+ Or pluses 
```
1. First ordered list item 
2. Another item 
   * Unordered sub-list
1. Actual numbers don’t matter, just that it’s a number 
   1. Ordered sub-list 
4. And another item

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we’ll use three here to also align the raw Markdown). 
   To have a line break without a paragraph, you will need to use two trailing spaces.    

* Unordered list can use asterisks 
- Or minuses
+ Or pluses 

## Links 

There are two ways to create links 

```
[I’m an inline-style link](https://www.google.com)

[I’m an inline-style link with title](https://www.google.com “Google’s Homepage”)

[I’m a reference-style link](Arbitrary case-insensitive reference text)

[I’m a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions](1)

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes example.com (but not on GitHub, for example). 

Some text to show that the reference links can follow later. 

[arbitrary case-insensitive reference text] : https://www.mozilla.org 
[1] : https://slashdot.org 
[link text itself] : http://www.reddit.com
```

[I’m an inline-style link](https://www.google.com)

[I’m an inline-style link with title](https://www.google.com “Google’s Homepage”)

[I’m a reference-style link](Arbitrary case-insensitive reference text)

[I’m a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions](1)

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes example.com (but not on GitHub, for example). 

Some text to show that the reference links can follow later. 

[arbitrary case-insensitive reference text]:https://www.mozilla.org 

[1] : https://slashdot.org 

[link text itself] : http://www.reddit.com

## Images 

```
Here’s our logo (hover to see the title text) : 

Inline-style :
![alt text](https://pbs.twimg.com/profile_images/641056907474538498/qIbg0pZP_bigger.png)
```
Here’s our logo (hover to see the title text) : 

Inline-style : ![alt text](https://pbs.twimg.com/profile_images/641056907474538498/qIbg0pZP_bigger.png)


## Code and Syntax Highlighting 

```
Inline ‘code’ has ‘back-ticks around’ it. 
```
Inline ‘code’ has ‘back-ticks around’ it. 

Blocks of code are either fenced by lines with three back-ticks, or are indented with four spaces. We recommend only using the fenced code blocks -- they’re easier to use and support syntax highlighting. 

```
```javascript 
var s = "JavaScript syntax highlighting";
alert(s);
```

```json
{
  "JSON": "Syntax Highlighting"
}
```

```
No language indicated, so no syntax highlighting.
```
```

```javascript 
var s = "JavaScript syntax highlighting";
alert(s);
```

```json
{
  "JSON": "Syntax Highlighting"
}
```

```
No language indicated, so no syntax highlighting.
```

## Tables
```
Colons can be used to align columns. 

| Tables        | Are             | Cool   |
| ------------- | :-------------: | -----: |
| col 3 is      | right-aligned   | $1600  |
| col 2 is      | centered        |   $12  |
| zebra stripes | are neat        |    $1  |

There must be at least 3 dashes separating each header cell. The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown. 

Markdown | Less | Pretty 
--- | --- | ---
*Still* | 'renders' | **nicely**
1 | 2 | 3 
```
Colons can be used to align columns. 

| Tables        | Are             | Cool   |
| ------------- | :-------------: | -----: |
| col 3 is      | right-aligned   | $1600  |
| col 2 is      | centered        |   $12  |
| zebra stripes | are neat        |    $1  |

There must be at least 3 dashes separating each header cell. The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown. 

Markdown | Less | Pretty 
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3 

## Blockquotes 
```
> Blockquotes are very handy in email to emulate reply text. 
> This line is part of the same quote. 

Quote break. 

> This is a very lonbg line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote.
```
> Blockquotes are very handy in email to emulate reply text. 
> This line is part of the same quote. 

Quote break. 

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote.

## Inline HTML 
You can also use raw HTML in your Markdown, and it'll mostly work pretty well. 
```
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>
  
  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>
```
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>
  
  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

## Horizontal Rule 
```
Three or more...

---

Hyphens 

***

Asterisks

___

Underscores
```
Three or more...

---

Hyphens 

***

Asterisks

___

Underscores

## Line Breaks 
Our basic recommendation for learning how line breaks work is to experiment and discover -- hit return twice. You'll soon learn to get what you want. 

Here are some things to try out: 
```
Here's a line for us to start with. 

This line is separated from the one above by two new lines, so it will be a *separate paragraph*.

```
Here's a line for us to start with. 

This line is separated from the one above by two new lines, so it will be a *separate paragraph*.

---
### Credits 
Most of this information was pulled from [Adam Pritchard's Mardkown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). Thank you Adam for putting together this cheatsheet! 




