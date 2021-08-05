# Docker_practice
RailsアプリケーションをDockerに移行する手順を学習


##アプリケーション立ち上げまで
```
$ docker-compose build
$ docker-compose run --rm rails bundle install
$ docker-compose run --rm rails yarn install
$ docker-compose run --rm rails bundle exec rails db:create db:migrate db:seed
$ docker-compose up -d rails
```

##ログファイル見たい時
```
$ docker-compose ps
```

## アプリケーション終了まで
```
$ docker-compose down
```
