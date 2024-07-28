# Laravelの始め方


<br>
1. ターミナルにてgit cloneを行う

```bash
git clone https://github.com/shuji0425/docker-test.git
```
<br>

2. コンポーザーのインストール
```bash
cd laravel-app
composer install
```
<br>

3. .envファイルの作成
```bash
cp .env.example .env
```
<br>

4. 環境構築を行う
<br>

+ Docker Desktopを開く
+ docker-compose.ymlがある階層で行う

```bash
docker-compose up -d --build
```
<br>

5. Dockerコンテナ内に移動
```bash
docker-compose exec app bash
```
<br>

6. アプリケーションキーの生成とキャッシュのクリア
```bash
php artisan key:generate
```
```bash
php artisan config:cache
```
<br>

6. DBにデータを入れる
```bash
php artisan migrate
```

<br>
Laravelの初期画面が表示できます。
