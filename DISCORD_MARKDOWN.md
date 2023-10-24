# Discord formatting tutorial

## Raw format
\`\`\`optionalLanguage  
codeblock  
\`\`\`
```
`single line code`
``single line code``
*italics*
_italics_
**bold**
__underline__
||spoiler||
~~strikethrough~~
> quote¹
- list item¹
 - sub-item¹
* list item¹
 * sub-item¹
1. numbered list item¹
# Header 1¹
## Header 2¹
### Header 3¹
```

## Preview
```optionalLanguage
codeblock
```
`single line code`  
``single line code``  
*italics*  
_italics_  
**bold**  
__underline__ (Underline is inconsistent across Markdown implementations, so this syntax appears bold. See [Discord Screenshot below](#Discord-Screenshot))  
||spoiler|| (Spoilers don't work on GitHub, see [Discord Screenshot below](#Discord-Screenshot))  
~~strikethrough~~  
> quote¹
- list item¹
  - sub-item¹
* list item¹
  * sub-item¹

1. numbered list item¹
# Header 1¹
## Header 2¹
### Header 3¹

## Discord Screenshot
This is a preview of what you will see in Discord, since it's not exactly the same as on GitHub.  
![Discord Screenshot](https://github.com/clari7744/DiscordFormatting/assets/73483912/f0d37fe4-c94e-432c-a6de-805f250c18ef)

## notes
Putting `\` before any format character will escape it, causing it to show the format character instead changing into formatted text, ie
`\_hi\_` will show up as \_hi\_

Use `<link>` to hide the embed that shows up when you post a link

fun trick: numbered lists work dynamically; this means you can use `1.` for the first item and `-` or `*` for every subsequent one and they'll be numbered automatically. good if you ever need to reorder, add, or remove an item
¹ space is required & only works at beginning of line