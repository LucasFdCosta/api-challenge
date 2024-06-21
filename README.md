# en-US
## Project Challenge
This project is the solution to a challenge. The classes and methods names were named in portuguese because the initial source code and the challenge were provided by a brazilian tech organization.

## Context
You need to build a task manager system, where you can register a list of tasks that will allow you to better organize your routine.

This task list needs to have CRUD operations, meaning it should allow you to retrieve records, create, save, and delete these records.

Your application should be either a Web API or MVC type, feel free to implement the solution you find most appropriate.

Your main class, the task class, should be as follows:

![Diagrama da classe Tarefa](diagrama.png)

Don't forget to generate your migration for database updates.

## Expected Methods
You are expected to create your methods as follows:


**Swagger**


![Métodos Swagger](swagger.png)


**Endpoints**

| Method  | Endpoint               | Parameter | Body          |
|-------- |------------------------ |-----------|---------------|
| GET     | /Tarefa/{id}            | id        | N/A           |
| PUT     | /Tarefa/{id}            | id        | Schema Tarefa |
| DELETE  | /Tarefa/{id}            | id        | N/A           |
| GET     | /Tarefa/ObterTodos      | N/A       | N/A           |
| GET     | /Tarefa/ObterPorTitulo  | titulo    | N/A           |
| GET     | /Tarefa/ObterPorData    | data      | N/A           |
| GET     | /Tarefa/ObterPorStatus  | status    | N/A           |
| POST    | /Tarefa                 | N/A       | Schema Tarefa |

This is the Tarefa schema (model) used to pass to the methods that require it

**Obs.: here, the 'data' property refers to Date, because the schema was created in portuguese.**

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pending"
}
```

## Solution
The code is halfway done, and you should continue implementing it according to the rules described above, so that in the end, we have a functional program.


# pt-BR
## Desafio de projeto
Esse projeto é uma solução de um desafio.

## Contexto
Você precisa construir um sistema gerenciador de tarefas, onde você poderá cadastrar uma lista de tarefas que permitirá organizar melhor a sua rotina.

Essa lista de tarefas precisa ter um CRUD, ou seja, deverá permitir a você obter os registros, criar, salvar e deletar esses registros.

A sua aplicação deverá ser do tipo Web API ou MVC, fique a vontade para implementar a solução que achar mais adequado.

A sua classe principal, a classe de tarefa, deve ser a seguinte:

![Diagrama da classe Tarefa](diagrama.png)

Não se esqueça de gerar a sua migration para atualização no banco de dados.

## Métodos esperados
É esperado que você crie o seus métodos conforme a seguir:


**Swagger**


![Métodos Swagger](swagger.png)


**Endpoints**


| Verbo  | Endpoint                | Parâmetro | Body          |
|--------|-------------------------|-----------|---------------|
| GET    | /Tarefa/{id}            | id        | N/A           |
| PUT    | /Tarefa/{id}            | id        | Schema Tarefa |
| DELETE | /Tarefa/{id}            | id        | N/A           |
| GET    | /Tarefa/ObterTodos      | N/A       | N/A           |
| GET    | /Tarefa/ObterPorTitulo  | titulo    | N/A           |
| GET    | /Tarefa/ObterPorData    | data      | N/A           |
| GET    | /Tarefa/ObterPorStatus  | status    | N/A           |
| POST   | /Tarefa                 | N/A       | Schema Tarefa |

Esse é o schema (model) de Tarefa, utilizado para passar para os métodos que exigirem

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
```


## Solução
O código está pela metade, e você deverá dar continuidade obedecendo as regras descritas acima, para que no final, tenhamos um programa funcional.