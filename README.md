# tasklist

## execute os comandos com o node.js e o postgreSql instalado

`npm i` para instalar os pacotes

`npm run dev` para rodar o servidor

`npx sequelize db:migrate` para rodar as migrations do banco de dados

## Rotas:

### POST /users

cadastra um novo usuario, \*todos os campos são obrigatorios

```
{
  "name":"Exemplo",
  "email": "exemplo@mexemplo.com",
  "password": "123123"
}
```

### POST /sessions

autentica o usuario e recebe um token jwt, \*todos os campos são obrigatorios

```
{
  "email": "exemplo@mexemplo.com",
  "password": "123123"
}
```

### PUT /users

edita um usuario, precisa usar jwt no header, Authorization `Bearer + ( JWT )`

\*alguns campos são opcionais, mas se enviar oldPassword o campo password e confirmPassword ficam obrigatorios

```
{
  "name":"Exemplo",
  "email": "exemplo@mexemplo.com",
  "oldPassword": "123123",
  "password": "123456",
  "confirmPassword": "123456"
}
```
