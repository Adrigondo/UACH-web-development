# 1 Modelos como servicios (Models as a service)

Hace referencia a como podemos contratar un servicio. Por ejemplo, el agua se paga mensualmente y se paga lo que utilizamos.

* Infraestructura. IAAS.
  Servidores, redes, firewalls, bloques. There are also a model as a service for infreestructure called nfraestructure as a service.

* Platform. PAAS.
  Plaform as a service. Over the infraestructure there exists platforms made to deploy and distribute aplications. For example there exists *back4app*, *Heroku* or *Vercel*.

* Software. SAAS.
  Software as a service. When we are renting the aplication to the final user, for example *Google* or *Netflix*.

# 2. ORM and ODM
Object relational mapper, Object document mapper.

### Relational Database Management System. 
Los modelos relacionales es una manera de expresar los datos desde el álgebra relacional.

MySql, Oracle, SQLServer, MariaDB.

El DML de SQL es una manera de realizar álgebra relacional.

Los lenguajes de programación es una expresión de un paradigma que tienen una gramática libre de contexto.

Si un lenguaje entiende orientado a objetos y la base de datos entiende algebra relacional, ¿Cómo se comunican?.

Un ORM transforma del lenguaje relacional al lenguaje orientado a objetos y viceversa mediante el patrón de diseño *DAO* (Data Access Object).

Para cada tabla requiere una clase, de manera que exista una equivalencia, y así podremos definir los elementos y reglas.

> Un ORM de Java poderoso es hybernate.

Los ORM son agnósticos del manejador que estemos usando.

Un ODM transforma un modelo basado en documentos a un lenguaje orientado a objetos y viceversa.

Siempre colocar un id entero autoincremental.

Donde está la patita de gallo es en la que se encontrará la llave foránea.

Si la linea es continua se lee como debe (forzosa). Si la linea es punteada, la relación es puede (opcional).

Convención de MVC. Modelos en singular, controladores en plural.