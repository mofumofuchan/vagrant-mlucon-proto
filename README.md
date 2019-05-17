# vagrant-mlucon-proto

## Overview

[MLUCON prototype](https://github.com/mofumofuchan/mlucon-proto)の環境を構築するためのVagrantfileです。

## Usage

- vagrant実行環境を用意する
- このリポジトリ内のVagrantfileを手元に用意する
  - 必要に応じてVagrantfileを編集する
- Vagrantfileがあるディレクトリで`vagrant up`を実行する
  - ベンチマーク用サーバ(bench)と参加者用サーバ(image)が起動
- Ansibleによるプロビジョニングが完了したら`vagrant ssh`を実行する
```
vagrant ssh bench
vagrant ssh image
```
- ベンチマークを実行する
（追記します）
<!---
```
/opt/go/bin/benchmarker -t http://(imageのIPアドレス)/ -u /opt/go/src/github.com/catatsuy/private-isu/benchmarker/userdata
```
--->

## 動作確認

Ubuntu 18.04 + VirtualBox 5.2.22 + Vagrant 2.2.4で動作確認しています


