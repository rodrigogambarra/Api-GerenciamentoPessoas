<h3>Especificação:</h3>

Sistema de gerenciamento de pessoas em API REST com Spring Boot

API desenvolvida com framework spring boot com utilização do banco H2

Operações disponibilizadas pela API:

<h4>RequestMethod *GET* - Retorna lista de pessoas</h4>
Url: http://localhost:8080/api/v1/people

<h4>RequestMethod *POST* - Cria uma nova pessoa</h4>
Url: http://localhost:8080/api/v1/people
####Exemplo:
{

    "firstName":"Rodrigo",

    "lastName":"Gambarra",

    "cpf":"000.235.680-21",

    "birthDate":"05-10-2022",

    "phones":[

        {

        "type":"COMMERCIAL",

        "number":"83738376687382"

        }

    ]

}

<h4>RequestMethod *GET* - Retorna uma pessoa por ID</h4>
Url: http://localhost:8080/api/v1/people/{id}

<h4>RequestMethod *PUT* - Atualiza os dados de uma pessoa apartir do Id</h4>
Url: http://localhost:8080/api/v1/people/{id}
####Exemplo:
{

    "id":1,

    "firstName":"Rodrigo",

    "lastName":"Gambarra",

    "cpf":"000.345.680-21",

    "birthDate":"05-10-2022",

    "phones":[

            {

                "id":1,

                "type":"COMMERCIAL",

                "number":"83738376687382"

            },

            {

                "id":2,

                "type":"MOBILE",

                "number":"83738378281182"

            }

    ]

}

<h4>RequestMethod *Delete* - Deleta uma pessoa apartir do Id</h4>
Url: http://localhost:8080/api/v1/people/{id}

