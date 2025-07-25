# k8s-tn23-setup
Kubernetes setup ansible script for tuna2134

## 環境のセットアップ
```sh
uv venv
uv sync
```

## メインのセットアップ

### 1. inventory/hostsを編集
ここには設定対象のワーカー、マスターそしてロードバランサーが設置されています。
適時設定してください。

### 2. inventory/group_vars/all/network.ymlを編集
マスターIP、要するにk8sのapiを受信するIPを書いてください。

### 3. inventory/group_vars/all/version.ymlを編集
k8sのバージョンをここで指定してください。