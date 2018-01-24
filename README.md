# rocker-jp/verse

[![Build Status](https://travis-ci.org/rocker-jp/verse.svg?branch=master)](https://travis-ci.org/rocker-jp/verse)

## This repository is designed for Japanese only, sorry!

## 概要

このレポジトリには、日本のRユーザのための、
- RStudio server
- tidyverse群パッケージ
- 日本語フォント(IPAexMincho, IPAexGothic)

があらかじめインストールされたR言語Dockerコンテナを提供します。

## 起動方法

まずは、[Docker](https://docs.docker.com/installation/)が正しくインストールされているかを確認してください。

###  RStudio server
以下のコマンドを実行することで、RStudioサーバのコンテナを起動することが出来ます。

```shell
docker run -d -p 8787:8787 rockerjp/verse
```
起動した後、`http://<サーバのアドレス>:8787` にブラウザからアクセスすることでRStudioサーバを使用できます。
ローカルで実行している場合は、 [http://localhost:8787](http://localhost:8787) です。

ユーザ名とパスワードは下記の通りです。

- username: rstudio
- password: rstudio

### Shiny server
Shiny serverは3838ポートで起動しているので、RStudio server同様、
```shell
docker run -d -p 3838:3838 rockerjp/verse
```
というコマンドを実行することで、 `http://<サーバのアドレス>:3838` からアクセスすることができます。

## ライセンス
このDockerfileは MIT によりライセンスされています。
