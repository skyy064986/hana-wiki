# How to get a Gemini API key

This guide shows you how to create your own Gemini API key for Hana's `/privateai`. It takes about 2–3 minutes.

> Treat an API key like a password. Never post it in chat, share it with another person, or include the full key in a screenshot. If it is exposed, delete it and create a new one immediately.

## 1. Open Google AI Studio

Open [Google AI Studio](https://aistudio.google.com/welcome) and sign in with your Google account.

If this is your first visit, select **Get started** and review Google's terms before continuing.

![The Get started button in Google AI Studio](../.gitbook/assets/gemini-api-key-01-get-started.png)

## 2. Open API Keys

Open the AI Studio Dashboard, then select the key-shaped **API Keys** icon in the left menu.

![The key-shaped icon that opens API Keys](../.gitbook/assets/gemini-api-key-02-menu.png)

## 3. Create a key

Select **Create API Key**.

![The Create API Key button](../.gitbook/assets/gemini-api-key-03-create.png)

- Google may have already created a default project and key for a new user. You can use that key or create a separate one.
- If prompted for a project, select an existing project or create one specifically for Hana.
- When the key is ready, copy it and keep it temporarily in a secure place.

## 4. Add the key to Hana

1. Return to Discord and run `/privateai`.
2. Select **2 · Add Gemini key**, or open **Gemini Text & Keys → Add key**.
3. Paste the key into `Gemini API key #1`, then submit the form.
4. Wait while Hana validates the key and loads the available text models.

The first field is required and the remaining fields may be left empty. Private AI supports up to 10 keys and encrypts each key before storing it.

## If you cannot create a key

- Make sure you have accepted Google's Terms of Service.
- A school or organization account may not have permission to create keys. Use a personal account or contact the Google Cloud administrator.
- If an existing project is missing, you may need to import it into AI Studio first.
- Some models may not offer a Free Tier or may have reached the project's quota even when the key itself is valid.

Google documentation: [Get started with the Gemini API](https://ai.google.dev/gemini-api/docs/get-started) · [Manage Gemini API keys](https://ai.google.dev/gemini-api/docs/api-key)
