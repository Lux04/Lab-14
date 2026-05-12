# SETUP

## Сонгосон API
DummyJSON API

## Brief
DummyJSON нь fake REST API бөгөөд CRUD endpoint, login, auth token, users, products зэрэг endpoint-үүдтэй.

## Base URL
https://dummyjson.com

## Auth
JWT token ашигладаг. Login request-ээс token авч environment variable болгон хадгалсан.

## Ашигласан Endpoint-үүд
- GET /users
- GET /users/1
- POST /auth/login
- POST /users/add
- PUT /users/1
- DELETE /users/1
- GET /users/999999
