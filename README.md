# PinBot

メッセージの管理権限を付与しなくてもピン留めを利用できるようにします。

## Use

このリンクから招待できます

[このBOTを招待する](https://discord.com/api/oauth2/authorize?client_id=1171376502990962731&permissions=10240&scope=bot)

### セルフホスト

1. `[TOKEN]` にDiscordAPIトークンを設定します

```yml
version: "3"

services:
  app:
    image: .
    environment:
      - DISCORD_API_TOKEN=[TOKEN]
```

2. コンテナを起動します

```sh
docker compose up -d
```

## Dev

`config.ts`の`DEBUG`に開発用サーバーのIDを設定してください

開発モードではより詳細なアプリケーションコマンドの即時更新が使用できます
