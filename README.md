[Ссылка на проект]( http://deveri.serveblog.net/redoc/)
# Проект YaMDb
![Github actions](https://github.com/NakiriEri/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)  
Проект YaMDb собирает отзывы пользователей на различные произведения такие как
фильмы, книги и музыка.

## Описание проекта:

API YaMDb позволяет работать со следующими сущностями:

* JWT-токен (Auth): отправить confirmation_code на переданный email, получить
  JWT-токен
  в обмен на email и confirmation_code;
* Пользователи (Users): получить список всех пользователей, создать
  пользователя,
  получить пользователя по username, изменить данные пользователя по username,
  удалить
  пользователя по username, получить данные своей учётной записи, изменить
  данные своей учётной записи;
* Произведения (Titles), к которым пишут отзывы: получить список всех объектов,
  создать
  произведение для отзывов, информация об объекте, обновить информацию об
  объекте, удалить произведение.
  пользователя по username, получить данные своей учётной записи, изменить
  данные своей учётной записи;
* Категории (Categories) произведений: получить список всех категорий, создать
  категорию, удалить категорию;
* Жанры (Genres): получить список всех жанров, создать жанр, удалить жанр;
* Отзывы (Review): получить список всех отзывов, создать новый отзыв, получить
  отзыв по id,
  частично обновить отзыв по id, удалить отзыв по id;
* Комментарии (Comments) к отзывам: получить список всех комментариев к отзыву
  по id, создать
  новый комментарий для отзыва, получить комментарий для отзыва по id, частично
  обновить комментарий к отзыву по id, удалить комментарий к отзыву по id.

## Стек технологий:

* [Python 3.7+](https://www.python.org/downloads/)
* [Django 2.2.16](https://www.djangoproject.com/download/)
* [Django Rest Framework 3.12.4](https://pypi.org/project/djangorestframework/#files)
* [Pytest 6.2.4](https://pypi.org/project/pytest/)
* [Simple-JWT 1.7.2](https://pypi.org/project/djangorestframework-simplejwt/)
* [pytest 6.2.4](https://pypi.org/project/pytest/)
* [pytest-pythonpath 0.7.3](https://pypi.org/project/pytest-pythonpath/)
* [pytest-django 4.4.0](https://pypi.org/project/pytest-django/)
* [djangorestframework-simplejwt 4.7.2](https://pypi.org/project/djangorestframework-simplejwt/)
* [Pillow 9.2.0](https://pypi.org/project/Pillow/)
* [PyJWT 2.1.0](https://pypi.org/project/PyJWT/)
* [requests 2.26.0](https://pypi.org/project/requests/)

## Как запустить проект:

* Клонировать себе репозиторий и перейти в него через командную строку

```
cd api_yamdb
```

* Cоздать и активировать виртуальное окружение:

```
python -m venv venv
```

```
source venv/scripts/activate
```

* Установить зависимости из файла ```requirements.txt```:

```
pip install -r requirements.txt
```

* Выполнить миграции:

```
python manage.py migrate
```

* Запустить проект:

```
python manage.py runserver
```


## Документация для YaMDb доступна по адресу:

```http://127.0.0.1/redoc/```
## Авторы:
[Антон Молчанов](https://github.com/antxrest)
[Андрей Грушевский](https://github.com/gruand69)
[Павел Туголуков](https://github.com/NakiriEri)
