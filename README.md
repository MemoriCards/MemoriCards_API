# MemoriCards API

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

### AutoLogin

`GET /users/:usersId: - FORMATO DA REQUISIÇÃO`

```
Não é necessário um corpo da requisição.
```

### Busca todos os flashcards do usuário logado

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

### Busca flashcards por id

`GET /flashcards/:id: - FORMATO DA REQUISIÇÃO`

``` 
Não é necessário um corpo da requisição.
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
