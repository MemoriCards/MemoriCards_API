# MemoriCards API

<a href= "https://insomnia.rest/run/?label=memori-cards-api&uri=https%3A%2F%2Fmemori-cards-api.onrender.com" target="_blank"><img src="https://insomnia.rest/images/run.svg" alt="Run in Insomnia"></a>

<blockquote> Para importar o JSON no Insomnia é só clicar no botão "Run in Insomnia".
</blockquote>
<br>

A url base da API é https://memori-cards-api.onrender.com

## Endpoints que não necessitam de token

### Cadastro de usuário

`POST /signup - FORMATO DA REQUISIÇÃO`

```json
{
  "email": "kenzinho2@mail.com",
  "password": "$2a$10$inkMXFPw2KJWb.DbLA/I5ujgwZxQW5buCxUUxblE5OuMHPtDcSnnm",
  "image": "",
  "username": "teste",
  "id": 1,
}
```

POST /register <br/>
POST /signup <br/>
POST /users

<br>

### Login

`POST /signin - FORMATO DA REQUISIÇÃO`

```json
{
  "email": "kenzinho2@mail.com",
  "password": "$2a$10$inkMXFPw2KJWb.DbLA/I5ujgwZxQW5buCxUUxblE5OuMHPtDcSnnm",
}
```

POST /login <br/>
POST /signin

## Endpoints que necessitam de token

### Cards

`GET /flashcards - FORMATO DA REQUISIÇÃO`

```json
{
  Em construção...
}
```
