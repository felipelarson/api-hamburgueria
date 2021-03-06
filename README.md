# react-atividade-s5-template-JSON-Server

## Base_URL

https://server-felipe.herokuapp.com/

## Users

### Cadastro

POST /register

```json
{
    "email": "felipelarson@gmail.com",
    "password": "123456",
    "name": "felipe",
    "age": 41
}
```

### Login

`POST /login`

```json
{
    "email": "felipelarson@gmail.com",
    "password": "123456"
}
```

## Products

### create new products

`Post /products`

header {
    Authorization: Bearer token
}

```json
{
    "name": "Hamburguer",
    "category": "Sanduíches",
    "price": 7.99,
    "userId": 2
}
```

### get products

`GET /products`

```json
[
 {
    "id": 1,
    "name": "Hamburguer",
    "category": "Sanduíches",
    "price": 7.99,
    "userId": 2
  }
]
```

### get only products

`GET /products/:id`

```json
[
 {
    "id": 1,
    "name": "Hamburguer",
    "category": "Sanduíches",
    "price": 7.99,
    "userId": 2
  }
]
```

### update products

`PATCH /products/:id`

header {
    Authorization: Bearer token
}

```json
{
    "name": "Hamburguer upgrade",
    "category": "Sanduíches",
    "price": 7.99,
    "userId": 2
}
```

### delete products

`DELETE /products/:id`

header {
    Authorization: Bearer token
}

## Cart

### create new cart

`Post /cart`

header {
    Authorization: Bearer token
}

```json
{
    "name": "Hamburguer",
    "category": "Sanduíches",
    "price": 7.99,
    "userId": 2,
    "quantity": 1
}
```

### get cart

`GET /cart`

```json
[
 {
    "id": 1,
    "name": "Hamburguer",
    "category": "Sanduíches",
    "price": 7.99,
    "userId": 2,
    "quantity": 1
  }
]
```

### get only cart

`GET /cart/:id`

```json
[
 {
    "id": 1,
    "name": "Hamburguer",
    "category": "Sanduíches",
    "price": 7.99,
    "userId": 2,
    "quantity": 1
  }
]
```

### update cart

`PATCH /cart/:id`

header {
    Authorization: Bearer token
}

```json
{
    "name": "Hamburguer upgrade",
    "category": "Sanduíches",
    "price": 7.99,
    "userId": 2,
    "quantity": 2
}
```

### delete cart

`DELETE /cart/:id`

header {
    Authorization: Bearer token
}