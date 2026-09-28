# Private AI

`/privateai` creates up to five personal roleplay character slots using your own Gemini API keys. It is separate from Hana's persona, memory, keys, and quota. Your data follows your Discord User ID across supported RoomAI servers and DMs without affecting other members.

## Quick setup

1. Run `/privateai` and accept the Gemini Safety notice.
2. Select **1 · Create character** and enter a name, background, personality, and speaking style.
3. Select **2 · Add Gemini key** and paste at least one API key. If you do not have one yet, see [How to get a Gemini API key](../guides/get-gemini-api-key.md).

The system validates the key, discovers available models, selects a supported Flash Lite model, and enables Private AI automatically. You do not preconfigure your own name; introduce yourself in the story and let the relationship develop naturally.

## Character slots

- Create up to five characters and switch the active one from **Character slots**.
- All slots share your Gemini keys and selected model, so keys are entered only once.
- Character, scene, memory, history, and relationship data stay isolated per slot.
- Deleting a character requires entering `YES`. Deleting the last slot disables Private AI but preserves the keys and model.

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

## Private character relationship

Relationship tracking is enabled by default and is evaluated in the same successful Gemini response, without an extra API call:

| Score | Level |
| --- | --- |
| 0–50 | Acquaintance |
| 51–149 | Friend |
| 150–249 | Close friend |
| 250+ | Talking stage until dating is accepted |
| Accepted dating proposal | Partner |
| Accepted marriage proposal | Married |
| Married at 2,000 | Life partner |

A normal message adds 1, something the character likes adds 2–3, a dislike adds nothing, and a strong dislike removes 1–2. `*` director commands, duplicate messages, and failed API requests do not add points. If proposals are enabled, a character may ask to date at 500 and may propose marriage after dating at 1,000. Tracking and proposals can be disabled per slot. A disabled relationship keeps its score and is hidden from `/profile`.

## Clear versus reset

- **Clear memory** removes recent history and the long-term summary, but keeps the character, scene, and relationship.
- **Reset this character** also resets the scene, roleplay/memory settings, history, summary, score, relationship status, and proposal state while preserving the character identity and preferences.
- **Reset all (keep Gemini)** removes every character slot and disables Private AI while preserving keys and the selected model.
- **Delete all data** removes characters, memories, relationships, and Gemini keys from active storage.

Private AI uses a local SQLite database with up to three rotating recovery backups. API keys are encrypted with AES-256-GCM before storage.

Gemini applies provider safety filters. Adult sexual content, violence, or other sensitive roleplay may be refused, and Hana does not bypass those controls. Do not submit passwords, addresses, financial or health information, or another person's secrets. See [Privacy and terms](../privacy-and-terms.md).
