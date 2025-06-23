# PROBLEMA 123

Una empresa que fabrica telas almacena los datos de su producción utilizando estructuras que 
contienen los siguientes datos para cada lote: 
- Fecha (string “aaaa:mm:dd”) 
- Hora (string “hh:mm:ss”) 
- Longitud en metros (real) 
- Ancho en metros (real) 
- Color (string de 10 caracteres útiles) 
- Código del lote (entero sin signo) 
Se necesita realizar un programa en  C que permita realizar las siguientes tareas: 
a) Leer todas las estructuras almacenadas en el archivo binario (“C:\stock\datos.bin”), 
realizando reserva dinámica de memoria, y previendo una cantidad adicional de 50 
estructuras más, a los fines de permitir eventuales incorporaciones de nuevas estructuras. 
b) Agregar por teclado nuevas estructuras, solicitando al operador cada uno de los campos. 
c) Generar un archivo de texto que contenga las longitudes y anchos de los lotes de un color 
determinado, ordenados por fecha y hora de fabricación en orden ascendente (los más 
viejos arriba). 
d) Muestre por pantalla un listado de todos aquellos lotes que hayan sido fabricados en un 
determinado día y cuyo ancho esté comprendido entre dos límites determinados, ordenado 
por color. 
e) Actualizar el archivo binario.