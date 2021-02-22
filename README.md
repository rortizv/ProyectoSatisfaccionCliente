# ProyectoSatisfaccionCliente

El Proyecto de Sistema de Medición de la Satisfacción al Cliente está pensado para brindar información sobre las calificaciones que reciben los empleados de atención al cliente
o de servicio de cualquier compañía.

Se trata de un sistema que almacena en una base de datos las calificaciones recibidas en cada servicio por cada agente, el sistema guarda el número del cajero y la respectiva
calificación y la base de datos asigna la fecha en que se crea el registro al igual que un id auto incrementable para identificar el registro.

La calificación es recibida a través de una board de Arduino que se compró por Amazon y se armó con 5 botones, cada uno indica un nivel de satisfacción del servicio:
- Excelente
- Bueno
- Normal
- Regular
- Malo

La board de Arduino es programada en lenguaje C a través de un IDE que se descarga desde la página de Arduino para que envíe el pulso del botón presionado a Java
y lo envíe a la base datos.

Se envía el dato a través del puerto programado a través del método arduinoRXTX que recibe el puerto como parámetro ("COM4" por ejemplo).

Java almacena los datos en una base de datos que está en la nube, motor MySQL.

Aquí pueden visualizar los resultados de las pruebas:
https://www.prototiposatisfaccion.unicartagena.co


