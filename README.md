# json-server-todo

このリポジトリは、Dockerコンテナ内でJSONサーバーを使用してシンプルなToDoアプリケーションを提供します。

## 構成ファイル

- `Dockerfile`: JSONサーバーをセットアップするためのDocker設定ファイル。
- `docker-compose.yml`: マルチコンテナDockerアプリケーションを定義するためのComposeファイル。
- `db.json`: ToDoデータを保存するJSONデータベースファイル。

## セットアップ

### 必要条件
- Docker
- Docker Compose

### 手順

1. リポジトリをクローンします:
   ```sh
   git clone https://github.com/Masssa33/json-server-todo.git
   cd json-server-todo
   
2. Docker Composeを使用してコンテナを起動します:  
   ```sh
   docker compose up -d

3. ブラウザで以下のURLにアクセスして、ToDoアプリケーションを確認します:
   ```url
   http://localhost:3000

## データベースの使用方法
ToDoの作成、読み取り、更新、削除（CRUD）操作をAPIエンドポイントを通じて行います。
エンドポイント例:  
取得: GET /todos  
作成: POST /todos  
更新: PUT /todos/:id  
削除: DELETE /todos/:id  

## 停止
コンテナを停止するには以下を実行します:
   ```sh
   docker compose down
