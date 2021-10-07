# WordPress Theme Kit

```bash
docker-compose up -d
npm install -g pnpm
pnpm install

# 開発
pnpm run dev

# ビルド
pnpm run build
```

## DB のダンプデータ取得

DBコンテナに入る

```bash
docker-compose run db bash
```

コンテナ内で以下を実行

```bash
mysqldump -uuser -ppass wpdb --no-tablespaces > /docker-entrypoint-initdb.d/dump.sql
```

`docker-entrypoint-initdb.d` に出力される

## お団子イラスト

https://jitanda.com/2018/01/05/j350_8/
