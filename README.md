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

Как создать БД на Хероку

1. heroku addons:create heroku-postgresql:hobby-dev - создаем Базу Данных на Хероку

2. heroku run rails db:migrate                      - сделать миграцию 

3. git push heroku master

4. heroku psql                                      - зайти в базу данных на Хероку
