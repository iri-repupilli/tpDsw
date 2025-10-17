# Propuesta TP DSW

## Grupo
### Integrantes
* 52634 - Gregoret, Facundo
* 52417 - Repupilli, Irina
* 53256 - Schiffo, Bruno
* 53133 - Frassine, Lautaro

### Repositorios
* [frontend app](https://github.com/facugreg/inmobiliariaFrontEnd)
* [backend app](https://github.com/iri-repupilli/inmobiliariaBackend)

## Tema
### Descripción
Este sistema inmobiliario permite la gestión y publicación de distintos tipos de inmuebles como casas, departamentos, cocheras y terrenos. Los usuarios pueden ser clientes o administradores, mientras que los propietarios registran sus inmuebles. Cada inmueble incluye información detallada, historial de precios y puede recibir consultas y reseñas. Está clasificado por tipo y servicio (venta o alquiler). Las propiedades están vinculadas a localidades y direcciones específicas. El sistema busca facilitar la interacción entre usuarios y la administración eficiente de propiedades.

### Modelo
![Modelo de datos](inmobiliaria3.jpg)

## Alcance Funcional 

### Alcance Mínimo


Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario <br>2. CRUD Propietario<br>3. CRUD TipoServicio<br/> 4.CRUD Localidad|
|CRUD dependiente|1. CRUD Inmueble {depende de} CRUD Propietario, TipoServicio, Localidad<br>2. CRUD Visita {depende de} CRUD Inmueble y Usuario|
|Listado<br>+<br>detalle| 1. Listado de inmuebles filtrado por tipo de inmueble, muestra los atributos de cada tipo de inmueble => detalle CRUD Inmueble<br> 2. Listado de inmuebles filtrado por localidad, muestra los inmuebles de la localidad elegida => detalle muestra datos de cada inmueble|
|CUU/Epic|1.Solicitar una visita<br>2. Hacer una consulta (dejar una opinion)|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Imagenes <br>2. CRUD Consulta<br>|
|CUU/Epic|1. Agregar la ubicacion de los inmuebles desde un Mapa<br>2. Moderar reseña (con API de IA o libreria)|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Inmueble filtrado por mts2, antiguedad, fecha de publicacion<br>|
|Otros|1. Envío de email cuando un usuario se registra y cuando un administrador responde la consulta de un cliente<br/>2. Manejo de archivos como agregar imagenes del inmueble<br/> 3. Envio de email a los clientes en base a sus gustos|

