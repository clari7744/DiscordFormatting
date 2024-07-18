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

## Hyperlinks

Links have enough variations that they're worth making a separate section for.  

To make a link clickable, it *must* begin with `http://` or `https://`. For instance, some apps will make `discord.com` clickable, but Discord requires `https://discord.com`.  

To hide a link's embed, wrap it in `<` and `>`. For example, `https://discord.com` shows the below embed, but you can hide it with `<https://discord.com>`  

![discord.com embed](https://github.com/user-attachments/assets/a594afac-67b3-4550-91a9-5fd6ee6fe447)  

To use different display text, use this format: `[display text](URL)`. For example, `[Discord](https://discord.com)` will show as [Discord](https://discord.com). Keep in mind that the embed will still show, so if you'd like to hide it, use `[Discord](<https://discord.com>)`.

To change the alt (hover) text, use this format: `[display text](URL "alt text")`. For example, `[Discord](https://discord.com "alt text")` will show as [Discord](https://discord.com "alt text") (Hover to see alt text). Note that quotes are required, and you can use either single or double quotes.  
Interestingly enough, `'using an apostrophe? it's totally valid'` shows up properly, even though the apostrophe should technically end the quotation. This works for double quotes as well (only the very first and very last quotes are actually registered).

Side note: You can actually hyperlink other forms of markdown as well. For example, using code formatting, ``[`Discord`](https://discord.com)`` will show as [`Discord`](https://discord.com).  
You can also put a link on a timestamp: `
[<t:1420070400:F>](<https://discord.com> 'Discord's birthday!')` will appear as in the image below.

![Discord Birthday Timestamp](https://github.com/user-attachments/assets/6416d00e-5d50-49f8-88b4-067f2b43b896)

## Notes

Putting `\` before any format character will escape it, causing it to show the format character instead changing into formatted text, ie
`\_hi\_` will show up as \_hi\_

fun trick: numbered lists work dynamically; this means you can use `1.` for the first item and `-`, `*`, or even `1.` again for every subsequent one and they'll be numbered automatically. this is helpful if you ever need to reorder, add, or remove an item

[^1]: space is required & only works at beginning of line
