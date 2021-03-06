# API для блога на Node.js

Приложение представляет собой страницу, на которой могут делать записи любые авторизованные пользователи.

## Возможности

1) Реализована регистрация и авторизация пользователя, а также проверка JWT-токена при внесении записей на страницу
2) Запись блога содержит:
    -  Дату записи
    -  Сообщение: может содержать как текст, так и медиа
    -  Автора сообщения
3) На странице с записями реализована пагинация, на каждой странице (пагинации) отображается по 20 записей
4) Автор записи может редактировать или удалять запись
5) Написана документаця к эндпоинтам (Swagger/OpenAPI)

## Технологии

- Express
- MongoDB
- Mongoose
- TypeScript

## Начало работы

Скопируйте репозиторий и установите зависимости

```shell
git clone https://github.com/nblackninja/blog-nodejs
cd blog-nodejs
npm install
```

Создайте файл .env в папке src и установите переменные среды

```shell
# development или production 
NODE_ENV=development

# Порт HTTP соединения, default = 5000
PORT=5000

# Server address
BASE_URL=http://localhost

# Адресс для подключения к MongoDB
MONGO_URI=

# Путь к папке сохранения изображений при загрузки на сервер
FILE_PATH=

# Секретная строка для генерации токена доступа
JWT_SECRET=
```

Запустите сервер

```shell
# development
npm run server:watch

# production
npm run start
```

### Лицензия

MIT
