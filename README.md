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
  "password": "$2a$10$inkMXFPw2KJWb.DbLA/I5ujgwZxQW5buCxUUxblE5OuMHPtDcSnnm"
}
```

### Login

`POST /signin - FORMATO DA REQUISIÇÃO`

```json
{
  "email": "kenzinho2@mail.com",
  "password": "$2a$10$inkMXFPw2KJWb.DbLA/I5ujgwZxQW5buCxUUxblE5OuMHPtDcSnnm",
}
```

## Endpoints que necessitam de token

### Flashcards

`GET /users/:usersId:?_embed=flashcards - FORMATO DA REQUISIÇÃO`

```json
[
 {
   "question": "Qual é a formulada água?",
   "answer": "H2O",
   "id": 1
 },
 {
   "question": "Qual é a capital do japão?",
   "answer": "Tokyo",
   "id": 2
 }
 
   {...}
]
```
###  Criar Flashcards

`POST /flashcards/:Id - FORMATO DA REQUISIÇÃO`

```json
{
  "question": "Qual é a formulada água?",
  "answer": "H2O",
}
```

###  Excluir Flashcards

`DELETE /flashcards/:Id - FORMATO DA REQUISIÇÃO`

```
  Não é necessário um corpo da requisição.
```

###  Editar Flashcards

`PATCH /flashcards/:Id - FORMATO DA REQUISIÇÃO`

```json
{
  "question": "Qual é a formulada água?",
  "answer": "H2O",
}
```
