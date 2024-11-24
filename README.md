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
limactl start --name=debian debian12-arm.yaml
```

```shell
limactl stop debian && limactl delete debian
```

```shell
limactl stop debian && limactl delete debian && limactl start --debug --name=debian debian12-arm.yaml && limactl shell debian
```

```shell
limactl start --debug --name=debian debian12-arm.yaml && limactl shell debian
```

# lima コマンド

## 開始

```shell
limactl start debian
```

## Linuxインスタンスを一覧

```shell
limactl list
```

# 削除

```shell
limactl delete debian
```

```shell
limactl stop debian
```

```shell
limactl shell debian
```