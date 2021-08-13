# laravel-docker

1.phpコンテナに入る
```
docker exec -it sns_app_php bash
```

2.laravelをインストール
```
composer global require laravel/installer
```

3.laravelのプロジェクト作成
```
composer create-project --prefer-dist laravel/laravel test_docker
```

.envを書き換える
```
DB_CONNECTION=mysql
DB_HOST=db
DB_PORT=3306
DB_DATABASE=sns_app
DB_USERNAME=docker
DB_PASSWORD=docker
```

sequelproのurl http://sequelpro.com/
