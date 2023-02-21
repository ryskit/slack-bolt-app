# Slack Bot App

Bolt入門ガイドをTypeScriptで試してみたリポジトリです。

https://slack.dev/bolt-js/ja-jp/tutorial/getting-started

アプリケーションを実行するにあたり、`SLACK_SIGNING_SECRET`と`SLACK_BOT_TOKEN`が必要です。

- `Signing Secret`
  - Settings > Basic Information > App Credentialsから確認できます。
- 'Bot User OAuth Access Token`
  1. Scopesを設定(`chat:write`)
  2. Install to WorkspaceでワークスペースにAppをインストールする
  3. Installを許可すると、`Bot User OAuth Access Token`が表示されます。

もし、`direnv`を利用している場合は `.env`ファイルを作成すると便利です。

```shell
$ touch .env
$ echo "SLACK_SIGNING_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
$ echo "SLACK_BOT_TOKEN=xoxb-000000000000-0000000000000-XXXXXXXXXXXXXXXXXXXXXXXXX"
```