# Kittygram 
Kittygram - это веб-приложение для публикации и просмотра фотографий котиков. Пользователи могут создавать и просматривать котиков, загружать их фотографии и присваивать им достижения.


## Описание проекта

Сайт с возможностью публикации фотографий котов и их достижений.

## Технологии

- Фронтенд: React
- Бэкенд: Django Rest Framework
- База данных: PostgreSQL
- Nginx
- Docker
- Gunicorn
- Github actions


## Запуск проекта локально
Создать .env с переменными по примеру .env.example.

Выполнить запуск:

```bash
sudo docker compose up
```

## После запуска: миграции, сбор статики



```bash
sudo docker compose exec backend python manage.py migrate

sudo docker compose exec backend python manage.py collectstatic

sudo docker compose exec backend cp -r /app/collected_static/. /backend_static/static/
```

Веб-приложение будет доступно по адресу:

```
http://localhost:9000/
```
## Автор:
Александр Русанов, shurik.82rusanov@yandex.ru, @shurikrusanov
