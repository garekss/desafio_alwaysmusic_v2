##### Desarrollo desafio Always Music Versión 2

###### 1. Hacer Todas Las Consultas Con Un Objeto Como Argumento Del MéTodo Query.
###### 2. Hacer Las Consultas Con Texto Parametrizado
###### 3. Capturar Los Posibles Errores En Todas Las Consultas E Imprimirlos Por Consola.
###### 4. Obtener El Registro De Los Estudiantes Registrados En Formato De Arreglos.

##### 1-Registrar Un Nuevo Estudiante:

Instalar npm i pg

`node server.js registrar 12345678-6 "Ignacio Dubo" G70 7`  

*Traerá como resultado por ejemplo un alumno que sea registrado:*


>*** Academy Always Music *****
Alumno Ignacio Dubo rut: 12345678-6 fue registrado con éxito!
Alumno Registrado:  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 7 }

##### 2-Obtener el registro de un estudiante por rut:
`node server.js rut 12345678-6`

>***** Academy Always Music *****
Alumno consultado:  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 7 }

**3-Consultar El Registro De Todos Los Estudiantes Registrados De La Base De Datos: En Forma De Arreglos**

`node server.js consulta`

*traerá como resultado alumnos registrados:*

>***** Academy Always Music *****
Alumnos registrados: [
  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 7 }]


##### 4-Actualizar el registro de un estudiante de la base de datos:

`node server.js actualizar 12345678-6 "Ignacio Dubo" G70 6`

*el resultado será el siguiente:*

>***** Academy Always Music *****
Alumno con rut 12345678-6 actualizado con éxito
Alumno Actualizado:  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 6 }

##### 5-Eliminar el registro de un estudiante de la base de datos por rut:

`node server.js eliminar 12345678-6`

>***** Academy Always Music *****
Alumno con rut 12345678-6 eliminado con éxito
Alumno Eliminado:  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 6 }

**Agradecimientos a Bianca Salcedo** :tw-1f64c:
