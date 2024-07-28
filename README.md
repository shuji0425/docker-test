# Laravelの始め方


<br>
1. ターミナルにてgit cloneを行う

```git clone
git clone https://github.com/shuji0425/docker-test.git
```
<br>
2. 環境構築を行う
<br>
・Docker Desktopを開く
・docker-compose.ymlがある階層で行う

```
docker-compose up -d --build
```
<br>
3. DBにデータを入れる

```
docker-compose exec app bash
```

```
php artisan migrate
```

<br>
Laravelの初期画面が表示できます。
