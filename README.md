<h1 align="center">Api Rest para Gerênciamento de Pessoas</h1>
<p align="center">Api desenvolvida para registro de informações de pessoas, permitindo CRUD por meio de requests HTTP</p>

---

**<p align="center">Sumário:</p>**
<p align="center">
<a href="#sobre">Sobre</a> |
<a href="#funcionalidades">Funcionalidades</a> |
<a href="#tecnologias">Tecnologias</a> |
<a href="#serviços-usados">Serviços usados</a> |
<a href="#imagens">Imagens</a> |
<a href="#como-usar">Como usar</a> |
<a href="#pré-requisitos">Pré-requisitos</a> |
<a href="#links">Links</a> |
<a href="#autor">Autor</a></p>



## Sobre
Esse projeto foi criado com o objetivo de aprimorar técnicas de criaçao de Apis, bem como testes unitários utilizando mokito

## Funcionalidades
As principais funcionalidades do projeto são:

✅ Listar todas as pessoas cadastradas e suas informações;

✅ Cadastrar uma nova pessoa informando: primeiro nome, sobrenome, CPF, data de nascimento e telefones de contato;

✅ Consutar uma pessoa específica;

✅ Excluir uma pessoa e todos seus dados do sistema;


## Tecnologias utilizadas
* Java 17
* Spring Boot
* Spring Data
* JPA
* Hibernate
* MySQL
* JUnit, Mockito


## Serviços usados
* GitHub
* Heroku (hospedagem)

## Imagens
<p>No momento não há imagens</p>

## Como usar
<p>Após iniciar o sistema, a api disponibiliza os seguintes métodos request:</p>

1. RequestMethod <i>GET</i> para url: http://localhost:8080/api/v1/people - <b>Retorna lista de todas pessoas cadastradas</b>

2. RequestMethod <i>POST</i> Url: http://localhost:8080/api/v1/people - <b>Cria uma nova pessoa</b>

Exemplo:
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

3. RequestMethod <i>GET</i> Url: http://localhost:8080/api/v1/people/{id} - <b>Retorna uma pessoa específica conforme valor do "id"</b>


4. RequestMethod <i>PUT</i> Url: http://localhost:8080/api/v1/people/{id} - <b>Atualiza os dados de uma pessoa apartir do "id"</b>

Exemplo:
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

5. RequestMethod <i>Delete</i> Url: http://localhost:8080/api/v1/people/{id} - <b>Deleta uma pessoa específica, conforme valor do "id"</b>


## Pré requisitos
Para abrir o sistema, basta o uso de um navegador de sua preferência e conexão com internet.

## Links
* Repositório GitHub: https://github.com/rodrigogambarra/Api-GerenciamentoPessoas
* Deploy: https://personapi-livedio.herokuapp.com/api/v1/people

## Autor
✨ Feito por Rodrigo Gambarra!!

* rodrigo@gambarra.com.br
* <a href="linkedin.com/in/rodrigo-gambarra-2a195b151" target=”_blank”>LinkedIn</a>
* <a href="https://github.com/rodrigogambarra" target=”_blank”>GitHub</a>
