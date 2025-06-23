# PROBLEMA 129

En una empresa maderera se desea llevar el registro de los productos que comercializa, para lo 
cual se dispone de un archivo ASCII denominado “madera.txt” con la información: 
- Especie de árbol (string 20) 
- Tipo de madera (carácter M = Machimbre, L = Listón, C = Cabio) 
- Ancho en pulgadas 
- Alto en pulgadas 
- Largo en pulgadas 
- Precio de la pulgada cúbica 
- Cantidad en stock 
Se pide se desarrolle un programa en “C” que ejecute la siguiente tarea: 
a) Leer el archivo entregado por la empresa y almacenarlo en memoria usando asignación 
dinámica de memoria. 
b) Permitir que el usuario ingrese una cierta cantidad de madera necesitada, la especie de árbol 
y el tipo de madera. Se deberá verificar su existencia en stock y en caso afirmativo se deberá 
descargar del mismo la cantidad solicitada. Este proceso debe continuar hasta que el 
operador manifieste que no necesita ingresar nuevos datos. 
c) Generar un archivo binario con la información anterior pero agregándole el precio de cada 
unidad de madera. En este caso deberá agregar más información que la que posee la 
estructura dada, la cual consiste  en el precio de cada madera. 
d) Generar un listado ordenado por Especie de árbol y por cantidad en stock de aquellas 
maderas que en stock se superen las 100.