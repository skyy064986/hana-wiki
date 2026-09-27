# Private AI

`/privateai` creates a personal roleplay character using your own Gemini API keys. It is separate from Hana's persona, memory, keys, and quota. The character and memory follow your Discord User ID across supported RoomAI servers and DMs without affecting other members.

## Quick setup

1. Run `/privateai` and accept the Gemini Safety notice.
2. Select **1 · Create character** and enter a name, background, personality, and speaking style.
3. Select **2 · Add Gemini key** and paste at least one API key.

The system validates the key, discovers available models, selects a supported Flash Lite model, and enables Private AI automatically. You do not preconfigure your own name; introduce yourself in the story and let the relationship develop naturally.

## Gemini API keys

- Add up to 10 keys, five fields at a time.
- The first field is required; the rest are optional. Open the form again for keys 6–10.
- Duplicate and invalid keys are reported separately.
- Keys are encrypted before storage, excluded from ordinary logs, and never included in data exports.

Never post a key in chat. Enter it only through the panel. A separate Gemini key with an appropriate Google Cloud quota is recommended.

## How to play

| Format | Meaning |
| --- | --- |
| `normal text` | Contextual narration or conversation |
| `"text"` | Explicit player dialogue |
| `*instruction` | An out-of-character scene-director instruction, not dialogue |
| `\text` | Bypass all AI; neither the character nor Hana responds |

```text
*Move the scene to a café and advance time to the afternoon
*Timeskip one week
*Make it rain and cause a power outage
*Change Yami into a black dress and make her feel nervous
```

`*` instructions can update the date, time, location, character outfit, player outfit, mood, and event under **Advanced settings → Scene**. Normal roleplay can update scene state too. Discord shows a typing indicator while Gemini responds, and long replies are split with `Character name •` on every part.

## Advanced settings

- Character appearance, outfit, relationship premise, world, and boundaries
- Response length, point of view, detail, pacing, and action style
- Current scene, recent context, and long-term memory summary
- Select, test, or delete Gemini keys and models
- Export without API keys, clear history, or permanently delete all data

Gemini applies provider safety filters. Adult sexual content, violence, or other sensitive roleplay may be refused, and Hana does not bypass those controls. Do not submit passwords, addresses, financial or health information, or another person's secrets. See [Privacy and terms](../privacy-and-terms.md).
