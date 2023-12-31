# API de Games 
Esta API é utilizada para cadastrar e editar games.
## Endpoints
### GET /games
Esse endpoint é reponsável por retornar a listagem de todos os games cadastrados no banco de dados.
#### Parametros
Nenhum
#### Respostas
##### ok! 200
Caso essa resposta aconteça você vai receber a listagem de todos os games.

Exemplo de resposta:
```
"User": {
        "id": 1,
        "email": "rafasennin@hotmail.com"
    },
    "games": [
        {
            "id": 23,
            "title": " Call of duty MW",
            "year": 2019,
            "price": 60
        },
        {
            "id": 65,
            "title": " Sea of thives",
            "year": 2018,
            "price": 40
        },
        {
            "id": 2,
            "title": " Minecraft",
            "year": 2012,
            "price": 20
        },
        {}
    ]
}
````
##### Falha na autenticação! 401
Caso essa resposta aconteça, isso significa que aconteceu alguma falha durante o processo de autenticação da rquisição. Motivos: Token inválido, Token expirado.

Exemplo de falha na autenticação:
```
{
    "err": "Token inválido"
}

```
