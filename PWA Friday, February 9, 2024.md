# PWA
Progressive Web App

# MVC
## Model
Se encuentra en el servidor, es el que se encarga de obtener la información de la bases de datos y regresarla con sentido al controlador.

## Controller
Se encarga de procesar la información y realizar la lógica de negocio.

## Vista
Aplicación del lado del cliente. Se desarrolla o bien en javascript o utilizando un framework.


# OSCI
## HTTP
Se creo para manipular archivos en un servidor remoto.
Cuando se fue desarrollando aplicaciones para comunicación de datos, HTTP se dividio en 2 arquitecturas, SOAP y REST (actualmente existe también GraphQL pero no ha alcanzado la suficiente fuerza).
HTTP es una analogía a que nos podemos comunicar y la arquitectura elegida es el lenguaje utilizado para conectarnos.
- REST: Transferencia de estado representacional. Las peticiones y las respuestas estarán en formato JSON (Javascritp Serializable Object). Utilizará los metodos de comunicación de HTTP, es decir GET, POST, PUT, PATCH, DELETE, para comunicar datos mediante JSON. CoC (Convention over Configuration), REST forza como se compone el WSDL, todas las acciones de los metodos HTTP están definidas.

- SOAP: utiliza una definición basada en XML. XML es al final de cuentas una notación, y es un lenguaje de marcado como HTML. Se dice que XML es el padre de HTML. 

WSDL: Web Service Definition Languaje.

Un objeto descrito con JSON:
```JSON
[
    pedro: {
        name: 'pedro',
        cabello: {
            color: 'negro',
        },
        altura: 1.80,
        peso: 90,
        direccion: {
            calle: 'Av. Siempre Viva',
            numero: 300,
        }
    }
]
```
Un objeto descrito con XML:
```XML
<persona name="pedro">
<cabello
color="negro">
</cabello>
</persona>
```

HTTP funciona con una convención de poner el nombre del modelo en plural.
