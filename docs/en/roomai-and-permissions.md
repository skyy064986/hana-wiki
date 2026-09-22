# Server owner guide

## Enable and disable AI Rooms

| Command | Purpose |
| --- | --- |
| `/setroomai` | Enable Hana AI in the current channel |
| `/unsetroomai` | Disable Hana AI in the current channel |
| `/guildbook` | Open the Discord guide |
| `/hanacontext` | Set server information or rules (Premium) |

AI Room enable/disable commands are for server administrators.

## Recommended permissions

Hana does not need Administrator if it has:

- View Channel
- Send Messages
- Read Message History
- Embed Links
- Attach Files
- Use Application Commands
- Send Messages in Threads, if the channel uses threads

## When Hana does not respond

1. Confirm the channel was enabled with `/setroomai`.
2. Confirm Hana can view and send in the channel.
3. Check channel overrides and thread permissions for denies.
4. Confirm the message is Thai, English, or Japanese.
5. Check whether the AI queue is busy or the API is temporarily slow.

## When photos do not appear

`/travelphoto` needs `Embed Links`. Discord prevents Hana from attaching the image if that permission is disabled.
