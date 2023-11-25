# Проект Kittygram - небольшая социальная сеть любителей котов и кошечек. 
### Описание
Динамический сайт с возможностью зарегистрироваться, публиковать фото котиков, их достижения, дату рождения и имя.
### Технологии
Python 3.10,
Django 3.2.3,
Django REST framework, 
React
### Запуск проекта в dev-режиме
- Клонируйте репозиторий и перейдите в него в командной строке:
```
git clone https://github.com/rest2011/kittygram_final.git
```
```
cd kittygram_final
```
- Запустите проект с помощью команды:
```
docker compose up
```
- Соберите статику Django с помощью команды:
```
docker compose exec backend python manage.py collectstatic
```
- Скопируйте статику командой:
```
docker compose exec backend cp -r /app/collected_static/. /static/static/
```
- По адресу http://127.0.0.1:9000/ сайт будет доступен.

### Автор
Ринат Хаматьяров (https://github.com/rest2011)

![badge](https://github.com/rest2011/kittygram_final/actions/workflows/main.yml/badge.svg?event=push)
