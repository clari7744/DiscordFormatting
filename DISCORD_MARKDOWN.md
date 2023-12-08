# Discord formatting tutorial

## Raw format

<pre>
```optionalLanguage  
codeblock  
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
</pre>

## Preview

```optionalLanguage
codeblock
```

`single line code`  
``single line code``  
*italics*  
_italics_  
**bold**  
__underline__ (Underline is inconsistent across Markdown implementations, so this syntax appears bold. See [Discord Screenshot below](#discord-screenshot))  
||spoiler|| (Spoilers don't work on GitHub, see [Discord Screenshot below](#discord-screenshot))  
~~strikethrough~~  
> quote[^1]

- list item[^1]
  - sub-item[^1]

* list item[^1]
  * sub-item[^1]

1. numbered list item[^1]

# Header 1[^1]

## Header 2[^1]

### Header 3[^1]

## Discord Screenshot

This is a preview of what you will see in Discord, since it's not exactly the same as on GitHub.  
![Discord Screenshot](https://github.com/clari7744/DiscordFormatting/assets/73483912/f0d37fe4-c94e-432c-a6de-805f250c18ef)

## notes

Putting `\` before any format character will escape it, causing it to show the format character instead changing into formatted text, ie
`\_hi\_` will show up as \_hi\_

Use `<link>` to hide the embed that shows up when you post a link

fun trick: numbered lists work dynamically; this means you can use `1.` for the first item and `-`, `*`, or even `1.` again for every subsequent one and they'll be numbered automatically. this is helpful if you ever need to reorder, add, or remove an item

[^1]: space is required & only works at beginning of line
