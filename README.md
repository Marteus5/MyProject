# Markdown for Git Documentation: A Practical Guide

> Good documentation is the part of a project that people actually read first.
>
> Markdown is how we write it quickly, in plain text, and have Git platforms render it nicely.

## Table of Contents

1. [What is Markdown?](#what-is-markdown)
2. [Basic Syntax](#basic-syntax)
3. [Adding Emphasis](#adding-emphasis)
4. [Block Quotes](#block-quotes)
5. [Lists](#lists)
6. [Code](#code)
7. [Links](#links)
8. [Tables](#tables)
9. [Task Lists](#task-lists)
10. [Quick Reference](#quick-reference)

---

## What is Markdown?

Markdown is a **lightweight markup language**. It is used to add formatting elements to plaintext documents.

When you create a Markdown-formatted file, you add Markdown syntax to the text to indicate which words and phrases should look different. A file such as `README.md` is plain text, but GitHub renders it as a formatted page.

Markdown is *platform independent*. You can create Markdown-formatted text on any device running any operating system. Websites like Reddit and GitHub support Markdown, and lots of desktop and web-based applications support it too.

## Basic Syntax

### Headings

Headings use the `#` symbol. One `#` is a level 1 heading, two is level 2, three is level 3.

# Heading Level 1: Hello World!

## Heading Level 2: Hello World!

### Heading Level 3: Hello World!

### Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text.

This is the first paragraph. It can span a single line or several lines of text.

This is the second paragraph. The blank line above is what separates it from the first.

## Adding Emphasis

Wrap text in two asterisks to make it **bold**, for example `**Hello World!**` renders as **Hello World!**.

Wrap text in one asterisk to make it *italic*, for example `*Hello World!*` renders as *Hello World!*.

You can combine them, for example `***Hello World!***` renders as ***Hello World!***.

## Block Quotes

To create a block quote, add a `>` in front of each line. A lone `>` on a blank line keeps the quote going across paragraphs.

> Hello World!
>
> World is a beautiful place!

## Lists

### Ordered Lists

Use numbers followed by periods. Indent items to nest them.

1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item

A simple ordered list without nesting:

1. First item
2. Second item
3. Third item
4. Fourth item

### Unordered Lists

Use dashes (`-`) in front of each item.

- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item

## Code

To denote a word or phrase as code, enclose it in backticks. For example, `This is a code` renders as inline code.

Inline code is handy for commands such as `git status` or `Install-Module -Name ImportExcel`.

For several lines, use a fenced block with three backticks:

```powershell
Install-Module -Name ImportExcel
Import-Excel "C:\Users\Administrator\Documents\Fruits.xlsx" -OutVariable fruit
```

## Links

To create a link, enclose the link text in brackets and follow it immediately with the URL in parentheses.

[Link to the Markdown Guide](https://www.markdownguide.org/basic-syntax/)

## Tables

To add a table, use three or more hyphens (`---`) to create each column's header, and use pipes (`|`) to separate each column. Colons in the divider row control alignment: `:---` left, `:---:` centre, `---:` right.

| Subnet | Network Address | Broadcast Address | Default Gateway |
|:-------|:---------------:|:-----------------:|----------------:|
| SN1    | 192.168.1.0     | 192.168.1.127     | 192.168.1.1     |
| SN2    | 192.168.1.128   | 192.168.1.255     | 192.168.1.129   |

## Task Lists

To create a task list, add a dash and brackets with a space (`- [ ]`) in front of task list items. Put an `x` in the brackets (`- [x]`) to mark one as complete.

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

## Quick Reference

| Element        | Syntax                        | Result                 |
|:---------------|:------------------------------|:-----------------------|
| Heading        | `# Title`, `## Title`         | Headings, levels 1 to 3 |
| Paragraph      | blank line between text       | Separate paragraphs    |
| Bold           | `**text**`                    | **text**               |
| Italic         | `*text*`                      | *text*                 |
| Block quote    | `> text`                      | Quoted text            |
| Ordered list   | `1. item`                     | Numbered list          |
| Unordered list | `- item`                      | Bulleted list          |
| Code           | `` `code` ``                  | `code`                 |
| Link           | `[title](https://example.com)` | Clickable link        |
| Table          | `\| a \| b \|` with `---` row | Table                  |
| Task list      | `- [x] done`, `- [ ] todo`    | Checkboxes             |

---

*Resources: [Getting Started | Markdown Guide](https://www.markdownguide.org/getting-started/).*