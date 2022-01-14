

立ち上げ
$ docker-compose build
$ docker-compose up -d

seed
$ docker-compose run api rails db:seed

controller作成
$ docker-compose run api rails g controller api/v1/todos

migrate関係
$ docker-compose run api bundle exec rake db:create
$ docker-compose run api rails db:migrate

$ docker-compose run api rails g model Todo title:string

yarn add 関係
$ docker-compose run front yarn add axios
$ docker-compose run front yarn add -D @types/axios

$ docker-compose run front yarn add react-router-dom
$ docker-compose run front yarn add -D @types/react-router-dom
