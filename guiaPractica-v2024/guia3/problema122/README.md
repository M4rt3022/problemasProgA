# PROBLEMA 122

En el control de tránsito aéreo se almacenan los datos de las solicitudes de distintos aviones en 
vuelo y los que están con posibilidad de decolaje utilizando estructuras de datos que poseen los 
siguientes datos: 
- Fecha (string “dd:mm:aaaa”)
- Hora (string “hh:mm:ss”) 
- Altitud (entero sin signo, es un código de nivel) 
- Mensaje (string long. Máxima de 250 caracteres útiles) 
- Respuesta  (string long. Máxima de 80 caracteres útiles) 
- Código del avión (entero sin signo) 
- Código de la empresa (entero sin signo) 
Se necesita realizar un programa en  C que permita realizar las siguientes tareas: 
a) Leer todas las estructuras almacenadas en el archivo binario (“C:\vuelo\datos.bin”), 
realizando reserva dinámica de memoria, y previendo una cantidad adicional de 100 
estructuras, a los fines de permitir eventuales incorporaciones de nuevas estructuras. 
b) Agregar por teclado nuevas estructuras, solicitando al operador cada uno de los campos. 
c) Generar un archivo de texto que contenga los códigos de avión y empresa de aquellos 
aviones que se hubieren comunicado entre dos momentos determinados, ordenado por 
empresa y luego por  avión 
d) Muestre por pantalla un listado de todos aquellos aviones cuya altitud sea mayor que una 
ingresada por teclado, ordenado por fecha y hora. 
e) Actualizar el archivo binario. 
f) Eliminar una estructura cuyo código de empresa y avión se ingrese. 
g) Implementar  un menú  para realizar las operaciones de b) a f) en forma reiterada.