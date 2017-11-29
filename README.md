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

heroku addons:create heroku-postgresql:hobby-dev - создаем Базу Данных на Хероку

heroku run rails db:migrate -                      сделать миграцию 

heroku psql - зайти в базу данных на Хероку
