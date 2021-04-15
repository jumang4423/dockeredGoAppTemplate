# golang docker environment

注意：環境によっては以下のコマンド全てにsudo権限が必要かも

## 初回環境構築

### イメージを作成

```
docker-compose build
```

## 開発時

### （もしコンテナが立ち上がってなかったら）コンテナを起動

```
docker-compose up -d
```

### （もしコンテナが立ち上がっててコンテナを終了したいなら）コンテナを終了

べつにいちいちコンテナ終了しなくてもいいっぽいけどw
```
docker-compose down
```

### コンテナの環境に対してコマンドを叩く方法

```bash
docker-compose exec goapp go run main.go
# docker-compose exec サービス名 コマンド
```