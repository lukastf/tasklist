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

edita um usuario

```
{
  "name":"Exemplo",
  "email": "exemplo@mexemplo.com",
  "password": "123123"
}
```
