# docker volumeの実体のフォルダは、参照できるが難しい

```
postgresql % docker volume ls
DRIVER    VOLUME NAME
local     postgresql_postgres
postgresql % docker volume inspect postgresql_postgres
[
    {
        "CreatedAt": "2022-09-09T16:23:20Z",
        "Driver": "local",
        "Labels": {
            "com.docker.compose.project": "postgresql",
            "com.docker.compose.version": "2.10.2",
            "com.docker.compose.volume": "postgres"
        },
        "Mountpoint": "/var/lib/docker/volumes/postgresql_postgres/_data",
        "Name": "postgresql_postgres",
        "Options": null,
        "Scope": "local"
    }
]
postgresql % ls /var/lib/docker/volumes/postgresql_postgres/_data
ls: /var/lib/docker/volumes/postgresql_postgres/_data: No such file or directory
```

https://note.com/w0o0ps/n/n9bc1bcd9fa59
https://zenn.dev/isosa/articles/3a352341c43411

