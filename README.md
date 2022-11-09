# Команды для работы с контейнерами

## Создание образа

docker build . -t greeting_html

## Запуск контейнера

docker run -d -p 7777:80 --name greeting greeting_html

## Просмотр запущенных контейнеров

docker ps

## Перейдем внутрь контейнера

docker exec -it greeting bash

## Переходим в папку

cd /usr/share/nginx/html

## Просмотр содержимого

ls -la

## Посмотрим содержимое файла index.html

cat index.html

## Остановка контейнера по имени

docker stop greeting

## Запуск контейнера по имени

docker start greeting

## Удаление контейнера по имени

docker rm greeting
