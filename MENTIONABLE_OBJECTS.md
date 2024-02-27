# Mentionable Objects

### Note

- Do not include `{}`. _Do_ include `<>`. Replace `{ID}` with the ID of the object you wish to mention.
- You can turn any of these objects back into their raw `<...>` form with `\#OBJECT`, `\@OBJECT`, `\:emoji:` etc.
- [Discord Official Documentation](https://discord.com/developers/docs/reference#message-formatting) (includes examples)

## Channels

### Format

- `<#{ID}>`

### Explanation

- Works for every type of channel: Text, Voice, Forum, Stage, Thread, DM, etc.
- Can be used everywhere on Discord. Use this to mention a channel from a server in another server or in a DM!
- Mentioning a category technically works, but it will not be clickable.

## Server Navigation

### Format

- `<id:customize>`
- `<id:browse>`
- `<id:guide>`

## Roles

### Format

- `<@&{ID}>`

### Explanation

- Works for every role in the current server.
- _Cannot_ be used to mention roles outside of the server they belong to.
- `<@&{SERVER_ID}>` will turn into the @\everyone mention.
- HOWEVER, mention permissions will still apply. Using `<@&{ROLE_ID}>` on a role that one does not have permission to @ normally will highlight the role, but not ping.

## Users

### Format

- `<@{ID}>`
- `<@!{ID}>`

### Explanation

- Works everywhere on Discord, similar to channel mentions.
- Most useful for mentioning a user in a channel they do not have access to, giving staff access to their profile.
- Also works in DMs, but Discord cache is sometimes tricky and it doesn't always show properly.
- The second format (`@!`) is basically equivalent, but it's deprecated, and is not recommended for use. The `!` is not required but will still work.

## Slash Commands

### Format
- `</{CMD_NAME}:{CMD_ID}>`
- `</{CMD_NAME} {SUBCMD_NAME}:{SUBCMD_ID}>`
- `</{CMD_NAME} {SUBGROUP_NAME} {SUBCMD_NAME}:{SUBCMD_ID}>`

### Explanation
- You can get the ID by right-clicking the command description on the chatbox when you start typing it and selecting `Copy ID`;
- These behave very strangely across devices in terms of rendering and selecting the correct bot.
- **PC/Browser** : Only renders if it's a valid command, and always selects the correct bot's command.
- **iPhone/iPad/Android** : Always renders, always selects the correct bot IF the command ID matches; shows a pop-up with options for the command arguments; if the command is invalid it will say so in the pop-up.

## Emojis

### Format

- `<:{EMOJI_NAME}:{EMOJI_ID}>`
- `<a:{EMOJI_NAME}:{EMOJI_ID}>`

### Explanation

- _Technically_ works everywhere, but without Nitro, emojis will convert to `:{EMOJI_NAME}:`.
- The `a` in front of the second format means "animated." Using an animated emoji without this will break it.
- There's a fun quirk where you put in the `{EMOJI_NAME}` section doesn't matter; only the ID matters - with the caveat that the name can only include letters, numbers, and underscores. This only works on mobile; PC automatically converts to the correct name.
- To get the emoji as an image, use this format: `https://cdn.discordapp.com/emojis/{EMOJI_ID}.png`. On desktop, right-click "Copy Link."


## Timestamps

### Format

- `<t:{UNIX_EPOCH}>`
- `<t:{UNIX_EPOCH}:{STYLE}>`

### Explanation

- `{UNIX_EPOCH}` is the number of seconds since 00:00:00 on January 1, 1970 (UTC).
- The `{STYLE}` determines how the formatted datetime appears. The following styles are available:
  - `t` : Short time
  - `T` : Long time
  - `d` : Short date
  - `D` : Long date
  - `f` : Short date/time
  - `F` : Long date/time
  - `R` : Relative time
- The timestamp will appear in the user's time zone and language-determined format (12 or 24 hour, month-day order etc).
- There are other examples of what it looks like out there, so I won't write my own here.
  - [Discord Docs](https://discord.com/developers/docs/reference#message-formatting-timestamp-styles)
  - [@LeviSnoot on GitHub](https://gist.github.com/LeviSnoot/d9147767abeef2f770e9ddcd91eb85aa#Formatting)