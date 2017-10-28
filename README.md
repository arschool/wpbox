## docker-compose を用いたWordpress開発環境

### 1. How To Use ?

1. Dockerデスクトップツールをインストールする
   * [Macはこちら](https://www.docker.com/docker-mac)
   * [Winはこちら](https://www.docker.com/docker-windows)

1. クローンする。
   * `git clone https://github.com/arschool/wpbox.git` コマンドでリポジトリをクローンする

1. 仮想環境を実行する
   * クローンしたディレクトリの中で下記を実行する
   * `% cd wpbox/`
   * `% docker-compose up -d`

1. ブラウザで確認する
   * ブラウザで[http://localhost:8080](http://localhost:8080)を確認する

1. テーマを開発する
   * `wpbox/data/wordpress/themes` 以下にディレクトリを作成し、テーマをつくる。

### 2. 構成

* WordPress最新版
* MySQL最新版
* `./data/mysql` 以下にMySQLのデータを永続化
* `./data/wordpress` 以下のフォルダをマウントし、WordPress用に利用
