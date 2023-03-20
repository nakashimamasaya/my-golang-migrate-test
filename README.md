# 概要
golang-migrateを試しに使った＋とりあえずDBにデータを入れたいときに使う

# 検証環境
golang-migarate v4.15.2

# 使い方

```
# (db1の例)
# migration
migrate --path db1/migrations/ --database 'mysql://root:example@(127.0.0.1:3306)/test1' -verbose up

# rollback
migrate --path db1/migrations/ --database 'mysql://root:example@(127.0.0.1:3306)/test1' -verbose down
```
