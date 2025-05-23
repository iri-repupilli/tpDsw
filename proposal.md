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
Este sistema inmobiliario permite la gestión y publicación de distintos tipos de inmuebles como casas, departamentos, cocheras y terrenos. Los usuarios pueden ser clientes o administradores, mientras que los propietarios registran sus inmuebles. Cada inmueble incluye información detallada, historial de precios y puede recibir consultas y reseñas. Está clasificado por tipo y servicio (venta o alquiler). Las propiedades están vinculadas a localidades y direcciones específicas. El sistema busca facilitar la interacción entre usuarios y la administración eficiente de propiedades.

### Modelo
![Modelo de datos](Inmobiliaria.png)

## Alcance Funcional 

### Alcance Mínimo


Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario <br>2. CRUD Inmueble<br>3. CRUD TipoServicio<br/> 4.CRUD Localidad|
|CRUD dependiente|1. CRUD Precio {depende de} CRUD Inmueble<br>2. CRUD Consulta {depende de} CRUD Inmueble|
|Listado<br>+<br>detalle| 1. Listado de inmuebles filtrado por tipo de inmueble, muestra los atributos de cada tipo de inmueble => detalle CRUD Inmueble<br> 2. Listado de inmuebles filtrado por localidad, muestra los inmuebles de la localidad elegida => detalle muestra datos de cada inmueble|
|CUU/Epic|1.Realizar una consulta<br>2. Registrar propietarios|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Usuario <br>2. CRUD Inmueble<br>3. CRUD TipoServicio<br/> 4.CRUD Localidad <br/> 5. CRUD Precio <br>6. CRUD Consulta|
|CUU/Epic|1. Registrar reseña<br>2. Moderar reseña (con API de IA o libreria)|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Inmueble filtrado por mts2, antiguedad, fecha de publicacion<br>|
|Otros|1. Envío de email cuando un usuario se registra y cuando un administrador responde la consulta de un cliente<br/>2. Manejo de archivos comoagregar imagenes del inmueble<br/> 3. Envio de email a los clientes en base a sus gustos|

