# Front-end Challenge
Show us what you can do and how clean your code is! Write a JavaScript SPA using AngularJS that will allow a user to create and display units and customers from a fake REST API.

## Requirements

- Use best practices in writing JavaScript, SCSS, and HTML.
- Write clearly and use proper MVC structure to write the application.
- Use UI-Router for your app routing.
- Use Gulp as your task runner.
- Use NPM as your package manager.

## Bonus

- Make use of AngularJS directives and services.
- Use Twitter Bootstrap for design the user interface.
- Paginate units and customers lists.

<br>

# API

## Dependencies
- Node
- NPM

## Project setup
- Clone this repository inside your application folder.
- Run `npm install` inside the `/server` in your application.

## Run local server

- Run `npm run serve`


---

### API Default URL

```
http://localhost:3000
```

### Units

```
GET     /units      (plural)
GET     /units/:id  (singular)
POST    /units
PUT     /units/:id
DELETE  /units/:id
```

Object
```
{
  id: 1361805,
  general: {
    name: "Consultório Exemplo",
    cnpj: "48567709000108"
  },
  address: {
    street: "Rua Camila Alvares de Azevedo, 481",
    city: "Embu das Artes",
    state: "SP",
    zip: "06804-150"
  },
  contact: {
    email: "consultorio.exemplo@email.com.br",
    phones: [
      {
        type: "mobile",
        value: "11989885655"
      },
      {
        type: "fax",
        value: "1137025440"
      }
    ]
  }
}
```

---

### Customers

```
GET     /customers      (plural)
GET     /customers/:id  (singular)
PUT     /customers/:id
POST    /customers
DELETE  /customers/:id
```

Object

```
{
  id: 1361806,
  general: {
    name: "Gabriela Nicole Silva",
    cpf: "40270048928",
    birth_date: "1976-04-03",
    gender: "m"
  },
  address: {
    street: "Rua Doutor Geraldo Leite, 751",
    city: "Feira de Santana",
    state: "BA",
    zip: "44088-018"
  },
  contact: {
    email: "leandrodiegolucasaraujo@ohms.com.br",
    phones: [
      {
        type: "work",
        value: "7535253201"
      },
      {
        type: "custom",
        value: "7529955312",
        custom: "WhatsApp"
      }
    ]
  }
}
```

---

### Paginate

```
GET     /units?_page=7
GET     /units?_page=7&_limit=20
```