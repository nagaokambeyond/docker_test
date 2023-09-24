# コンテナを起動する
```bash
docker-compose up -d
```
# コンテナに入る
```bash
docker container exec -it cpp_cd /bin/sh
```

# コンテナでソースをビルド・実行する
```bash
cd /cpp_dev/src
g++ main.cpp -o main
./main
```

# コンテナから出る
```bash
exit
```

# コンテナ停止する

```bash
docker-compose down
```

# コンテナを削除する
```bash
docker-compose down --rmi all --volumes --remove-orphans
```
