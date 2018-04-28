# Guide

Description for use Ruby on Rails

----------------------------------------

закинуть с локалки на Хероку:

git init

heroku git:remote -a recruitingtime

git add .

git commit -am "make it better"

git push heroku master

----------------------------------------
 
 Стереть БД, но потом снова надо создать

1. heroku pg:reset DATABASE - стереть БД, но потом снова надо создать

2. heroku addons:create heroku-postgresql:hobby-dev
 
3. heroku run rails db:migrate  

----------------------------------------
 
Как создать БД на Хероку

1. heroku addons:create heroku-postgresql:hobby-dev - создаем Базу Данных на Хероку

2. heroku run rails db:migrate                      - сделать миграцию 

3. git push heroku master

--------------------------------------------

Если делаем scafold, то делаем в папке assets/stylesheets/scaffolds.scc -> &:hover{//background-color: #000;} ; body {//margin: 33px;}

--------------------------------------------

heroku pg:psql                                      - зайти в базу данных на Хероку

SELECT * FROM users;

UPDATE candidates SET name = 'Ремень' WHERE ID = 1;

DELETE FROM table_name WHERE condition;

---------------------------------------------

чтобы зайти в БД sqlite3

rails dbconsole

SQLite>.tables

SQLite> select * from posts

bundle exec rake assets:precompile - Если не работает Автокомплит после Деплоя на Хероку, то вводим это в консоль

---------------------------------------------

Если при запуске будет - A server is already running. Check /mnt/c/Evtushenko/tmp/pids/server.pid.

rm /your_project_path/tmp/pids/server.pid
