# Ben 10 API
Esse projeto tem como objetivo desenvolver uma API que retorne informações sobre o desenho animado [Ben 10](https://pt.wikipedia.org/wiki/Ben_10), o projeto é baseado no [pokeapi](https://pokeapi.co/) e é uma iniciativa de desenvolvimento para fins didáticos e de apoio a comunidade. Com esse projeto será possível desenvolver sites capazes de resgatar e visualizar as informações mapeadas.

## Estrutura base do projeto
O projeto vai contar com quatro controllers, uma para cada grupo de informações mapeadas do desenho, que são: aliens do ominitrix, filmes, jogos e personagens. Cada controller terá os métodos de resgate de todas os dados, resgate por id e resgate por nome.

## Definições técnicas
A API será desenvolvida com [.NET](https://dotnet.microsoft.com/en-us/) na versão 8

As informações serão persistidas em uma base no [MongoDb](https://www.mongodb.com/)

### Estrutura das entidades
```json
{
    "omnitrix": {
        "id": ObjectId,
        "name": "",
        "originalName": "",
        "body": "",
        "planet": "",
        "species": "",
        "imageUrl": [
            ""
        ],
        "abilities": [ // List<string>
            ""
        ]
    },
    "movie": {
        "id" ObjectId,
        "name": "",
        "releaseDate": "",
        "duration": 123, // minutes
        "sinopse": "",
        "imageUrl": ""
    },
    "game": {
        "id" ObjectId,
        "name": "",
        "releaseDate": "",
        "imageUrl": "",
        "platforms": [ // List<string>
            ""
        ],
        "mainStoryTimeAvg": 300 // minutes
    },
    "characters": {
        "id": ObjectId,
        "name": "",
        "age": 10,
        "planet": "",
        "species": "",
        "imageUrl": [
            ""
        ],
        "abilities": [ // List<string>
            ""
        ]
    }
}
```


## Referências
https://ben10.fandom.com/wiki/Ben_10

https://pt.wikipedia.org/wiki/Ben_10

https://howlongtobeat.com/?q=ben%252010
