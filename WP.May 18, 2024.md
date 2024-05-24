# Algoritmos de seguridad en el servidor

## Blow fish (Bcrypt)
**Simétrico**: A mismos valores mismos resultados
**No reversible**: De el resultado no podemos obtener el valor original.

El algoritmo tomará la contraseña original, y una cadena llamada *salt key* para generar una cadena criptada (hash), a partir del cual ya no podremos recuperar la contraseña ni el salt key.

## JWT. JSON Web Token
Se espera que un login devuelva un token de sesión. En todas las peticiones que se hagan posteriormente al login, se estará enviando el token de sesión.

Es una cadena conformada por 3 cadenas separadas por puntos.
- Header. Se envía el tipo de algoritmo que se utiliza para encriptar.
- Payload. Toda la información que se quiere almacenar en el token de manera encriptada.
- Signature. Agrega la información del header y del payload, los encripta y se envían al final.

Nuestro JWT requerirá una llave con la cual se generarán los tokens de autenticación.

Usamos el algoritmo `HS256`.


---
### Listas de control de acceso (ACL)
Se basa en que puede hacer o no un usuario dentro del sistema.

### Role Based Access Control (RBAC)
Es similar al ACL, pero entre los permisos y los usuarios se agrega una etapa de roles, entonces el usuario tendrá roles, y los roles tendrán permisos.

### Tarea:
Implementar un RBAC dentro de el proyecto del videoclub.