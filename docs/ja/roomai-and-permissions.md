# サーバー管理者ガイド

## AI Room の有効化と停止

| コマンド | 用途 |
| --- | --- |
| `/setroomai` | 現在のチャンネルで Hana AI を有効にする |
| `/unsetroomai` | 現在のチャンネルで Hana AI を停止する |
| `/guildbook` | Discord 内のガイドを開く |
| `/hanacontext` | サーバー情報・ルールを設定する（Premium） |

AI Room の有効化・停止はサーバー管理者向けです。

## 推奨権限

Administrator は不要です。次の権限を付与してください。

- View Channel
- Send Messages
- Read Message History
- Embed Links
- Attach Files
- Use Application Commands
- Thread を使う場合は Send Messages in Threads

## Hana が返事をしない時

1. `/setroomai` でチャンネルを有効にしたか確認します。
2. Hana がチャンネルを見て送信できるか確認します。
3. Channel Override や Thread の deny 権限を確認します。
4. メッセージがไทย語、英語、日本語か確認します。
5. AI キューが混んでいる、または API が一時的に遅い可能性を確認します。

## 写真が表示されない時

`/travelphoto` には `Embed Links` が必要です。この権限がないと Discord は Hana の画像添付を許可しません。
