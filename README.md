# README

## version

- Ruby: 3.2.2
- postgresql: 12

## 開発環境構築方法

### 1.プロジェクトをクローン

```cmd
$ git clone https://github.com/octopus12176/rails-docker.git
$ cd rails-docker-practice
```

### 2.docker image をビルド

```cmd
$ docker-compose build
```

### 3.docker-compose up で起動

```cmd
$ docker-compose up
```

### 4. DB 作成

```cmd
$ docker-compose run web rake db:create
```

### 5. migrate を実施

```cmd
$ docker-compose exec web bash
$ rails db:migrate
```

起動コマンド後、`http://localhost:3000`に接続すると web アプリが開きます。
