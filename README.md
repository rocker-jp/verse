# rocker-jp/verse

[![Build Status](https://travis-ci.org/rocker-jp/verse.svg?branch=master)](https://travis-ci.org/rocker-jp/verse)

## This repository is designed for Japanese only, sorry!

## 概要

このレポジトリには、日本のRユーザのための、
- RStudio
- tidyverse群パッケージ
- 日本語フォント(IPAexMincho, IPAexGothic)

があらかじめインストールされたR言語Dockerコンテナを提供します。

## 起動方法

まずは、[Docker](https://docs.docker.com/installation/)が正しくインストールされているかを確認してください。
以下のコマンドを実行することで、RStudioサーバのコンテナを起動することが出来ます。

```shell
docker run -d -p 8787:8787 rockerjp/verse
```

起動した後、`http://<サーバのアドレス(ローカルで実行している場合localhost)>:8787`にブラウザからアクセスすることでRStudioサーバを使用できます。
ユーザ名とパスワードは下記の通りです。

- username: rstudio
- password: rstudio

## ライセンス
このDockerfileは MIT によりライセンスされています。
