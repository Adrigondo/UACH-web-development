# Bases de datos relacionales

Cuando la base de datos es relacional, tenemos una tabla que tiene campos.

A las bases de datos no les gusta que hayan nulls entre sus campos. Están diseñadas para procesamiento de transacciones online, es decir que congelarán el registro mientras se está realizando una operación sobre un registro. Así se mantiene la coherencia en la información de la base de datos.

El maestro las define como altamente "homogéneas". Están realizadas para que todos los registors sean similares.

Propiedades ACID. Atomicidad, coherencia, aislamiento y durabilidad. Hay información que se vuelve obsoleta.
Buscan que los datos sean durables

Normalmente el rendimiento depende del subsistema del disco

Las tablas sql no están diseñadas para sistemas distribuídos.

# Bases de datos no relacionales

Las bases de datos no relacionales son diseñadas para poseer datos más reales, es decir, permiten gran variedad de la información almacenada.

Estas bases de datos resuelven sus operaciones de manera atómica donde no congelan ningun movimiento.

Hacen concesiones al flexibilizar las propiedades ACID. Están dedicadas al BigData.

En la empresa primero generan la información no estructurada y luego la estructuran para su permanencia.

No dependen del disco, dependen del cluster, es decir, puedes tener más computadoras para permitir una expanción horizontal.

# Escalamiento
¿Cómo podemos aumentar la capacidad de un sistema?
Se llama escalamiento horizontal cuando aumentamos la eficiencia, es decir, aumentamos la cantidad de procesamiento.
Se llama escalamiento vertical cuando mejoramos la infraestructura tecnológica, es decír, cambiamos el procesamiento por algo mejor.
Mantener un equilibrio entre eficiencia e infraestructura conlleva al rendimiento óptimo

### Estrategias de replicación
Los datos entran a una base de datos y se replican en las demás.

### Estrategias de distribución
MongoDB hace una estrategia de sharding, permitiendo que la colección esté distribuída.

### Bases de datos NoSQL
Redis, mongoDB, neo4j, etc

Utilizaremos MongoDB.

#### Tarea:
- Completar la api del videoclub
- Traer un contenedor de mongo preparado para trabajar