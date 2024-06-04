
1-Hacer todas las consultas con un Objeto como argumento del método query.
2-Hacer las consultas con texto parametrizado
3-Capturar los posibles errores en todas las consultas e imprimirlos por consola.
4-Obtener el registro de los estudiantes registrados en formato de arreglos.

1-Registrar un nuevo estudiante:

Instalar npm i pg

node server.js registrar 12345678-6 "Ignacio Dubo" G70 7  

Traerá como resultado por ejemplo un alumno que sea registrado:

***** Academy Always Music *****
Alumno Ignacio Dubo rut: 12345678-6 fue registrado con éxito!
Alumno Registrado:  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 7 }
PS C:\Users\nacho\Desktop\bootchan clases\modulo 07\desafio_always_music_v2> 

2-Obtener el registro de un estudiante por rut:
node server.js rut 12345678-6

***** Academy Always Music *****
Alumno consultado:  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 7 }

3-Consultar el registro de todos los estudiantes registrados de la base de datos: en formao de ARREGLOS

node server.js consulta

traerá como resultado alumnos registrados:

***** Academy Always Music *****
Alumnos registrados: [
  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 7 }]


4-Actualizar el registro de un estudiante de la base de datos:

node server.js actualizar 12345678-6 "Ignacio Dubo" G70 6

el resultado será el siguiente:

***** Academy Always Music *****
Alumno con rut 12345678-6 actualizado con éxito
Alumno Actualizado:  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 6 }

5-Eliminar el registro de un estudiante de la base de datos por rut:

node server.js eliminar 12345678-6 

***** Academy Always Music *****
Alumno con rut 12345678-6 eliminado con éxito
Alumno Eliminado:  { rut: '12345678-6', nombre: 'Ignacio Dubo', curso: 'G70', nivel: 6 }