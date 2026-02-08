# 開発環境テンプレート

MySQL・phpMyAdmin を含む Laravel 開発環境のテンプレート 

---

## 環境構築

```bash
1. git clone リポジトリURL
2. docker compose up -d --build

＊Mysqlは、OSによって起動しない場合があるのでそれぞれのPCに合わせてdocker-compose.ymlファイルを編集してください。

Laravel環境構築

  1. docker compose exec php bash
  2. composer install
  3. cp .env.example .env (.env.exampleから.envを作成し、環境変数を変更)
  4. php artisan key:generate
  5. php artisan migrate
  6. php artisan db:seed

---

## 使用技術

- php　8.1
- nginx 1.21.1
- mysql 8.0
- laravel 8.75

---

## URL

- 開発環境：http://localhost/
- phpMyAdmin：http://localhost:8080/
