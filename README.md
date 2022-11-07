# Docker Playgorund - php

コンテナ上でphpの実行環境を構築しVisual Studio Codeから接続・実行できる環境を提供する

コンテナイメージのベースは
[php:cli-bullseye](https://hub.docker.com/_/php)
を利用。最新の環境としている。

Composerもインストール済み

追加で以下をインストールしている

* `git`
* `curl`
* `unzip`

実行ユーザ:`vscode`  
ワークスペース:`/workspace`  

ホスト側の`workspace`フォルダをコンテナ側の`/workspace`としてマウントしている

以下のVisual Studio Code 拡張をインストール

* EditorConfig.EditorConfig
* bmewburn.vscode-intelephense-client

## 使い方

[Docker Desktop](https://www.docker.com/products/docker-desktop/)を立ち上げる

[Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)に[Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)をインストール

後は Dev Containerで起動する
