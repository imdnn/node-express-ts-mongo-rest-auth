# node-express-ts-mongo-rest-auth

## Prerequisites
Не забудьте настроить .env файл по env.example, чтобы локально не поднимать свою БД, можно использовать [Atlas от mongodb.com](https://cloud.mongodb.com).

Postman-коллекция с предзаполненными данными находится в папке postman.

## General
**Built w/:**
- Node.js + Express + MongoDB (mongoose used) + Typescript 
- ESLint + Prettier + husky

**Authentication Controller:**
- POST "/auth/register"
- POST "/auth/login"

**Users Controller:**
- GET "/users"
- PATCH "/users/:id"
- DELETE "/users/:id"

**Middlewares:**
- isAuthenticated
- isOwner

**User Model:**
```json
{ 
    "username": {},
    "email": {},
    "authentication": {
        "password":  {},
        "salt": {},
        "sessionToken": {}
    } 
}
```

## Start

```bash
npm i
npm start
```
