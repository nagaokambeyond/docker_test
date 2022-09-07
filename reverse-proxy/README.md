# 実行方法
```
docker-compose up -d
```

インコ `http://localhost/parakeet` 
文鳥 `http://localhost/sparrow` 

# ハマったこと
## ポートがすでに使用されているため起動できない

```
[+] Running 3/4
 ⠿ Network reverse-proxy_default            Created                        0.0s
 ⠿ Container sparrow-container              Started                        0.5s
 ⠿ Container parakeet-container             Starting                       0.5s
 ⠿ Container reverse-proxy-reverse-proxy-1  Started                        0.5s
Error response from daemon: Ports are not available: exposing port TCP 0.0.0.0:7000 -> 0.0.0.0:0: listen tcp 0.0.0.0:7000: bind: address already in use
```
