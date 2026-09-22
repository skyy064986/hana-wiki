# Fun and Anime GIFs

## `/act <action>`

Send an Anime GIF for something you do yourself. Examples include `dance`, `wave`, `clap`, `laugh`, `shrug`, `cry`, `happy`, and `blush`.

## `/actwith <action> <user>`

Send an Anime GIF for an activity with someone else. You can choose whether to mention the recipient.

Examples: `dance`, `fistbump`, `welcome`, `highfive`, `hug`, `cuddle`, and `kiss`.

Closer actions require the recipient to accept before Hana sends the GIF.

### `givegift`

Use `/actwith givegift` to give a gift to someone.

1. Choose a recipient.
2. Add an optional gift message.
3. Add an optional `https://` gift link.
4. Review the preview and confirm before posting.

> **Think before sending:** the message and link are posted in the channel. Anyone who can see the channel may open the link or claim the gift first. Never post private links, passwords, or sensitive information.

## `/hanagame`

Open Hana's mini-game panel. Local prompts are used first where possible to reduce waiting and unnecessary AI calls.

## Speed and repeated GIFs

Hana fetches a fresh Anime GIF from the provider for every `/act` and `/actwith`; it does not cache GIFs. The provider can still occasionally return the same GIF.
