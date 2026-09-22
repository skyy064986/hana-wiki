# Fun と Anime GIF

## `/act <action>`

自分で行うアクションの Anime GIF を送ります。例: `dance`、`wave`、`clap`、`laugh`、`shrug`、`cry`、`happy`、`blush`。

## `/actwith <action> <user>`

他のユーザーと行うアクションの Anime GIF を送ります。相手をメンションするかも選べます。

例: `dance`、`fistbump`、`welcome`、`highfive`、`hug`、`cuddle`、`kiss`。

親密なアクションは、相手が承認してから GIF が送信されます。

### `givegift`

`/actwith givegift` で相手にギフトを送れます。

1. 相手を選びます。
2. ギフトメッセージは任意です。
3. `https://` のギフトリンクも任意で追加できます。
4. プレビューを確認してから送信を確定します。

> **送信前に確認:** メッセージとリンクはチャンネルに公開されます。見える人なら誰でもリンクを開いたり、ギフトを先に受け取ったりできます。個人用リンク、パスワード、機密情報は送らないでください。

## `/hanagame`

Hana のミニゲームパネルを開きます。待ち時間と不要な AI 呼び出しを減らすため、可能な場合はローカルの問題を優先します。

## 速度と GIF の重複

Hana は `/act` と `/actwith` ごとに提供元から新しい Anime GIF を取得し、GIF をキャッシュしません。ただし提供元の抽選により同じ GIF が返ることはあります。
