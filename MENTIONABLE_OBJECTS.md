# Mentionable Objects

### Note

- Do not include `{}`. _Do_ include `<>`. Replace `{ID}` with the ID of the object you wish to mention.
- You can turn any of these objects back into their raw `<...>` form with `\#OBJECT`, `\@OBJECT`, `\:emoji:` etc.

## Channels

### Format

- `<#{ID}>`

### Explanation

- Works for every type of channel: Text, Voice, Forum, Stage, Thread, DM, etc.
- Can be used everywhere on Discord. Use this to mention a channel from a server in another server or in a DM!
- Mentioning a category technically works, but it will not be clickable.

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
- The second format (`@!`) is basically equivalent, I'm not really sure what it's for. The `!` is not required but will still work.

## Emojis

### Format

- `<:{EMOJI_NAME}:{EMOJI_ID}>`
- `<a:{EMOJI_NAME}:{EMOJI_ID}>`

### Explanation

- _Technically_ works everywhere, but without Nitro, emojis will convert to `:{EMOJI_NAME}:`.
- The `a` in front of the second format means "animated." Using an animated emoji without this will break it.
- There's a fun quirk where you put in the `{EMOJI_NAME}` section doesn't matter; only the ID matters - with the caveat that the name can only include letters, numbers, and underscores. This only works on mobile; PC automatically converts to the correct name.
- To get the emoji as an image, use this format: `https://cdn.discordapp.com/emojis/{EMOJI_ID}.png`. On desktop, right-click "Copy Link."
