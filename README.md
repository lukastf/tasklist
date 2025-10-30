# tasklist

## Rotas:

### POST /users

cadastra um novo usuario

```
{
  "name":"Exemplo",
  "email": "exemplo@mexemplo.com",
  "password": "123123"
}
```

### POST /sessions

autentica o usuario e recebe um token jwt

```
{
  "email": "exemplo@mexemplo.com",
  "password": "123123"
}
```

### PUT /users

edita um usuario, precisa usar jwt no header, Authorization `Bearer + ( JWT )`

```
{
  "name":"Exemplo",
  "email": "exemplo@mexemplo.com",
  "oldPassword": "123123" (campo opcional)
  "password": "123456" (campo opcional)
}
```
