# lima

limaのDebian + Dockerなど開発環境の立ち上げ

Docker と go と rustが動作する環境を作っている
Silicon用で作成

| 名称   | 用途 |
|------|----|
| go   |    | 
| rust |    | 

| 名称         | 用途 |
|------------|----|
| Starship   |    | 
| eza        |    | 
| bat        |    | 
| procs      |    | 
| hexyl      |    | 
| tokei      |    | 
| bottom     |    | 
| du-dust    |    | 
| lazydocker |    | 
| lazygit    |    | 

https://github.com/lima-vm/lima

```shell
limactl start --name=default debian12-arm.yaml
```

```shell
limactl stop 
limactl delete
```

```shell
limactl stop default 
limactl delete default 
limactl start --debug --name=default debian12-arm.yaml 
```

```shell
limactl stop  
limactl start 
```

```shell
limactl shell default
```
```shell
ssh -F ~/.lima/default/ssh.config lima-default
````

# lima コマンド

## 開始

```shell
limactl start 
```

## Linuxインスタンスを一覧

```shell
limactl list
```

# 削除

```shell
limactl delete 
```

```shell
limactl stop 
```

```shell
limactl shell 
```

# Java
java -version

# Docker (ユーザー権限)
docker info

# Python
python3 --version

# Rust
rustc --version

# Go
go version

# Node.js
node -v

```shell
docker stop $(docker ps -a -q)
docker system prune
docker container prune
docker rm -f `docker ps -a -q`
docker image prune
docker rmi $(docker images -a -q)
docker volume prune
docker network prune

```


limactl show-ssh --format=config debian

limactl show-ssh --format=config default

ssh lima-debian

https://dev.classmethod.jp/articles/lima-using-vm-on-macos-without-parallels-vmware/
https://github.com/lima-vm/lima/discussions/1890
ssh -F ./ssh-config lima-default

ssh -F ~/.lima/debian/ssh.config lima-debian

https://github.com/lima-vm/lima/discussions/1221


https://qiita.com/mm_sys/items/28a0217256b56918fee4
https://qiita.com/shunk_jr/items/3528340ed5c37259b9ae
https://qiita.com/akinami/items/d38b9e7c7f37bd070f40

