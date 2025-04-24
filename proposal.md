# Propuesta TP DSW

## Grupo
### Integrantes
* 52634 - Gregoret, Facundo
* 52417 - Repupilli, Irina
* 53256 - Schiffo, Bruno
* 53133 - Frassine, Lautaro

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema
### Descripción
Es un sistema para una inmobiliaria el cual se encargaria de facilitar la consulta de clientes sobre distintos tipos de inmuebles para alquilar o comprar. Considerando dos tipos de usuarios, el cliente que hara lo previamente dicho y podrá realizar reseñas de estos, y el administrador que gestionara las altas, bajas y consultas de los inmuebles.

### Modelo
https://drive.google.com/drive/folders/1Knr2XjKzyxp0qlXE8TDpo4KdaIdVoK8Z


## Alcance Funcional 

### Alcance Mínimo


Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario <br>2. CRUD Inmueble<br>3. CRUD TipoServicio<br/> 4.CRUD Propietario|
|CRUD dependiente|1. CRUD Precio {depende de} CRUD Inmueble<br>2. CRUD Consulta {depende de} CRUD Inmueble|
|Listado<br>+<br>detalle| 1. Listado de habitaciones filtrado por tipo de habitación, muestra nro y tipo de habitación => detalle CRUD Habitacion<br> 2. Listado de reservas filtrado por rango de fecha, muestra nro de habitación, fecha inicio y fin estadía, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Habitacion<br>2. CRUD Servicio<br>3. CRUD Localidad<br>4. CRUD Provincia<br>5. CRUD Habitación<br>6. CRUD Empleado<br>7. CRUD Cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía y servicios|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

