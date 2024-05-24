
`show dbs;`
`use hr;`
Colección->Tabla
Objeto(Documento)->Registro

Un documento está formado por un objeto llamado BSON (Binary String Object Notation).
- Cadenas de caracteres
- Enteros de 32 a 64 vuts
- Tipo de dato real de 64 bits IEEE 754
- Fecha
- Array de bytes
- booleano
- Null
- Objeto BSON
- Array BSON
- Código JS
- Expresiones regulares

Funciona con llaves clave valor.

Mongodb está orientado al big data, es decir almacenar grandes volúmenes de datos no estructurados.


### db
En todas las sentencias, db apuntará a la base de datos que se apuntó utilizando `use`.
```mongosh

db.employees.insertOne({"name":"Adrian", "last_name":"González"});

show collections

db.employees.find()

db.employees.insertMany([{"name": "Vanessa"},{"name":"Pamela"}, {"name":"Renata"}]);
```

### find()
Podemos usar find para encontrar 1 solo elemento, todos los elementos, o encontrar elementos por filtros.
```
db.employees.find({"name":"Adrian"});
```

#### Operadores comparativos 
- gt
- eq
- gte
- in
- lt
- lte
- ne
- nin

#### Operadores lógicos 
and
or
nor
nand

```
db.employees.updateOne(
    {"_id": ObjectId('66476d2c11b7f5d3782202dd')},
    {"$set": {"name":"Renata", "age":25}}
);
```
```
db.employees.deleteOne({"_id": ObjectId('66476d2c11b7f5d3782202dd')});
```