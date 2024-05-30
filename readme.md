Pasos a realizar para ejecutar la base de datos:

Instalar:
npm i pg

***Pasos de registro en la base de datos:***

1-Registrar un nuevo estudiante:
<!-- node server.js registrar 12345678-9 "Juan Perez" G70 7  (ya se encuentra agregado, intentar con el siguiente.) -->
node server.js registrar 12345678-4 "Bianca Salcedo" G70 7
node server.js registrar 12345678-5 "Eduardo Ramos" G70 7
node server.js registrar 12345678-6 "Ignacio Dubo" G70 7
node server.js registrar 12345678-7 "Diego Cabre" G70 7

Traerá como resultado por ejemplo un alumno que sea registrado:

***** Academy Always Music *****
Alumno Juan Perez: 12345678-9 fué registrado con éxito!
Alumno Registrado:  { rut: '12345678-9', nombre: 'Juan Perez', curso: 'G70', nivel: 7 }

y asì mostrara todos los agregados..

![image](https://github.com/garekss/desafio_alwaysmusic/assets/159491346/4800b558-9046-40c8-94aa-f86de3c597a2)


2-Obtener el registro de un estudiante:

node server.js rut 12345678-4
Traerá  como resultado: --Alumno consultado: { rut: '12345678-9', nombre: 'Juan Perez', curso: 'G70', nivel: 7 }

3-Consultar el registro de todos los estudiantes registrados de la base de datos:

node server.js consulta
Traerá  como resultado: Alumnos registrados: [ { rut: '12345678-9', nombre: 'Juan Perez', curso: 'G70', nivel: 7 } ]
![image](https://github.com/garekss/desafio_alwaysmusic/assets/159491346/13ce7066-30c3-46b0-a17e-cd04fe194510)

4-Actualizar el registro de un estudiante de la base de datos:

node server.js actualizar 12345678-9 "Juan Perez" g70 8
Traerá  como resultado: --Alumno Actualizado: { rut: '12345678-9', nombre: 'Juan Perez', curso: 'g70', nivel: 8 }s

![image](https://github.com/garekss/desafio_alwaysmusic/assets/159491346/3ff86fd6-67f3-4eed-8a0e-558ceb60101b)


5-Eliminar el registro de un estudiante de la base de datos:

node server.js eliminar 12345678-9
Traerá  como resultado por ejemplo:

***** Academy Always Music *****
Alumno con rut 25675678-9 eliminado con éxito
Alumno Eliminado:  {
  rut: '12345678-9',
  nombre: 'Juan Perez',
  curso: 'g70',
  nivel: 18
}

![image](https://github.com/garekss/desafio_alwaysmusic/assets/159491346/f5e53af9-d097-45e1-bb47-62524c87093a)
