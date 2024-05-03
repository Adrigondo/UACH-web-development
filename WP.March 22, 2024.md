An aplication RESTfull is an aplication that uses a framework web and follows the rules of REST infraestructure.

A table RESTful

The model os derivated from HTTP Protocols, the URL and an action.

For a model `USER`
| CRUD   | HTTP Protocol | URL          | Action                                  |
| ------ | ------------- | ------------ | --------------------------------------- |
| Create | POST          | /`users`     | Creates an entity                       |
| Read   | GET           | /`users`     | Creates or display a list of entities   |
| Read   | GET           | /`users`/:id | Displays the entity with the id         |
| Update | PUT           | /`users`/:id | Replaces the entity with the id         |
| Update | PATCH         | /`users`/:id | Updates parts of the entity with the id |
| Delete | DELETE        | /`users`/:id | Deletes the entity with the id          |

# Group project

We have different dashboards by sprint.

A session of retrospective is when the sprint ends and all the team answer 3 questions:

| What did I good? | What did I bad? | What can I improve? |
| ---------------- | --------------- | ------------------- |


# Individual project: Videoclub

| Actions        | Entities        |
| -------------- | --------------- |
| Préstamo       | Movies          |
|                | Socios          |
|                | Fichas          |
|                | Copias          |
| Deposita       |                 |
| Pasa           |                 |
|                | Género          |
|                | Directores      |
|                | Actores         |
| Anotar, borrar | Lista de espera |

Entidad principal o entidad de dependencias

| Entidades simples | Entidades compuestas | Atributos |
| ----------------- | -------------------- | --------- |
| Genre             |                      |           |
| Director          |                      |           |
| Actor             |                      |           |
|                   | Movie                |           |
|                   |                      |           |

Las personas tienen nombre, las cosas tienen descripción.

> No hay que pensar en bases de datos.

Un **enum** tiene una lista de elementos limitada. Por ejemplo, los días de la semana, las estaciones del año, cosas que nos sirven para anclar el sistema y cosas que permiten una estructura dinámica, pero no tan dinámica. Se pueden agregar nuevos elementos, pero normalmente no cambian los que ya estaban.

Podemos **embeber** entidades dentro de otras, es decir estás solo existen dentro de una entidad. Por ejemplo, la dirección.

Los requisitos funcionales son todos aquellos que el cliente nos dice que el sistema debe hacer.

Los requisitos no funcionales son todos aquellos que el sistema debe tener, pero debemos hacer.

# Express
```sh
npm install -g express-generator
express --view=pug video-club
cd video-club
npm install
DEBUG=video-club:* npm start
```
| Flag   | Value | Description            |
| ------ | ----- |
| --view | pug   | Generador de proyectos |

### Middleware
When we have a client that does a request to our webapp. This request will be catched by the server and this one will send it to the web app. 

www->Server
app.js->App

Express start to call functions (Middlewares). When this one ends, call another function and this one call to another function...

  |-------------------------------------------------|<br>
  v                                                 |<br>
app.js->function1()->function2()->function3()->...->end()<br>
                |            |            |         ^
                ------------------------------------|<br>
Each function can call the next function or call end and end will tell the server to send a response.

The middleware of application are controllers. There are middlewares of static services (images, files, css).

Third-party middlewares.

The routing middlewares controls the method and the HTTP Method and direct it to an specific Aplication Middleware.

En el request, response, no solo viene la petición http si no que tmabién pueden venir la cookies por ejemplo el idioma.