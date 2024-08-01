# Discord Markdown Formatting Tutorial

## Inline formatting

Items in this section can be used anywhere in the middle of a line (except for within code/codeblocks).

### Inline Raw Format

<pre>
`single line code`
``single line code``
*italics*
_italics_
**bold**
__underline__
||spoiler||
~~strikethrough~~
[hyperlink text](https://link-address.com)
</pre>

### Inline Text Preview

`single line code`  
``single line code``  
*italics*  
_italics_  
**bold**  
<ins>underline</ins>  <!-- This uses <ins> for visualization as GitHub does not support the __underline__ syntax -->  
||spoiler|| (Spoilers don't work on GitHub, see [Discord Screenshot below](#inline-discord-screenshot))  
~~strikethrough~~  
[hyperlink text](https://link-address.com)

### Inline Discord Screenshot

![Inline formatting preview](https://github.com/user-attachments/assets/b3e0fae8-667c-4246-8bd5-b07fe7d1afb8)

## Full-line formatting

Items in this section must be used at the beginning of a line, and will affect the entire line. They require a space after the format character, as shown.

### Full-line Raw Format

<pre>
> quote

- list item
  - sub-item
* list item
  * sub-item
1. numbered list item

# Header 1
## Header 2
### Header 3

-# subscript
</pre>

### Full-line Text Preview

> quote  

-   list item
    -   sub-item
*   list item
    -   sub-item
1. numbered list item

# Header 1
## Header 2
### Header 3

<sub>subscript</sub> <!-- This uses <sub> for visualization as GitHub does not support the -# syntax -->

### Full-line Discord Screenshot

![Full-line formatting preview](https://github.com/user-attachments/assets/bee7ab55-37f6-4d38-9c50-caabe754191e)

## Multline formatting

Items in this section can be used to format multiple lines at once.

### Code Blocks Raw Format

Code blocks can be started and ended anywhere - even in the middle of a line.  
Spaces surrounding the backticks are arbitrary; aka not required, but also not disallowed.  
A programming language can be specified after the opening backticks to enable syntax highlighting. It must be immediately after the opening backticks, and it must be the only text on that codeblock line. There can be no spaces between the opening backticks and the language specifier, or between the language specifier and the new line.  
These, and any combination thereof, are all valid on Discord:

<pre>
```
codeblock text
```

(replace 'py' with any language)
```py
import codeblock
await codeblock.highlight('python')
```

```codeblock ```

Text ```codeblock``` text

Text```code block
more code block
``` more text
</pre>

### Code Blocks Text Preview

Since GitHub code block syntax is not quite the same as Discord code bock syntax, text code block previews have been omitted. See [the screenshot instead](#code-blocks-discord-screenshot).

### Code Blocks Discord Screenshot

![Code block preview](https://github.com/user-attachments/assets/c4ea71e8-0cb0-4267-ac76-a694a14d6f77)

### Block Quote Raw Format

Block quotes will cause all text following to be quoted, until you explicitly exit the quote block. On PC, you must press Backspace to exit the block quote. On mobile, you cannot exit the block quote - all text following the `>>>` is quoted.

<pre>
>>> Block quote
this text is still quoted

etc
</pre>

### Block Quote Text Preview

> Block quote  
this text is still quoted
> <!-- There are extra > here because GitHub doesn't support Discord's block quote syntax -->
> etc  

### Block Quote Discord Screenshot

![Block quote preview](https://github.com/user-attachments/assets/5b297647-38c3-4f1c-9e86-d46649d27e52)

## Hyperlinks

Links have enough variations that they're worth making a separate section for.

To make a link clickable, it _must_ begin with `http://` or `https://`. For instance, some apps will make `discord.com` clickable, but Discord requires `https://discord.com`.

To hide a link's embed, wrap it in `<` and `>`. For example, `https://discord.com` shows the below embed, but you can hide it with `<https://discord.com>`

![discord.com embed](https://github.com/user-attachments/assets/a594afac-67b3-4550-91a9-5fd6ee6fe447)

To use different display text, use this format: `[display text](URL)`. For example, `[Discord](https://discord.com)` will show as [Discord](https://discord.com). Keep in mind that the embed will still show, so if you'd like to hide it, use `[Discord](<https://discord.com>)`.

To change the alt (hover) text, use this format: `[display text](URL "alt text")`. For example, `[Discord](https://discord.com "alt text")` will show as [Discord](https://discord.com "alt text") (Hover to see alt text). Note that quotes are required, and you can use either single or double quotes.  
Interestingly enough, `'using an apostrophe? it's totally valid'` shows up properly, even though the apostrophe should technically end the quotation. This works for double quotes as well (only the very first and very last quotes are actually registered).

Side note: You can actually hyperlink other forms of markdown as well. For example, using code formatting, ``[`Discord`](https://discord.com)`` will show as [`Discord`](https://discord.com).  
You can also put a link on a timestamp: `
[<t:1420070400:F>](<https://discord.com> 'Discord's birthday!')` will appear as in the image below. See more on timestamps [here](MENTIONABLE_OBJECTS.md#timestamps).

![Discord Birthday Timestamp](https://github.com/user-attachments/assets/9f85a622-306a-443a-92f9-e5421c91215c)

## Notes

Putting `\` before any format character will escape it, causing it to show the format character instead changing into formatted text, ie
`\_hi\_` will show up as \_hi\_

fun trick: numbered lists work dynamically; this means you can use `1.` for the first item and `-`, `*`, or even `1.` again for every subsequent one and they'll be numbered automatically. this is helpful if you ever need to reorder, add, or remove an item.

![Dynamic numbered list chatbox](https://github.com/user-attachments/assets/2307b649-798d-47bc-839f-a0b74a897013) ![Dynamic numbered list message](https://github.com/user-attachments/assets/616ff3c9-482f-4a2c-838f-d48c997360b5)
