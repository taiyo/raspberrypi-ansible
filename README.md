# raspberrypi-ansible

RaspberryPiの設定をAnsibleのタスクで実施。

## Dockerのインストール

docker、docker-composeをインストールする。

```
ansible-playbook -i hosts docker.yaml
```

## MESHのインストール

「MESH ハブ」アプリをインストールする。

```
 ansible-playbook -i hosts mesh.yaml --extra-vars="mesh_url=[MESHパッケージのダウンロードURL]"
```