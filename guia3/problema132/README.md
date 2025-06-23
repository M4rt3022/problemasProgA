# PROBLEMA 132

Una fábrica de resmas de papel genera diariamente un archivo binario en el que se encuentra 
la información de la producción de ese día. Esta información consta de los datos de todas y 
cada una de las resmas fabricadas, según el siguiente detalle: 
- Número de serie de cada resma. (string de 15 caracteres útiles)  
- Peso del papel por metro cuadrado, en gramos. (entero) 
- Dimensiones del papel de la resma. (largo y ancho en centímetros; reales)  
- Cantidad de hojas de papel que forman la resma. (entero) 
- Hora de fabricación de la resma. (string en el formato hh:mm:ss ) 
Se pide realizar un programa en lenguaje C que permita: 
a) Generar un archivo ASCII (texto) con el número de serie y la hora de fabricación de        
todas las resmas cuyo tamaño sea de 21 cm por 29.7 cm y con un peso de papel superior a 
los 70 grs., ordenado por hora de fabricación. 
b) Generar un archivo binario con todos los datos de las resmas cuyo peso (peso de la resma, 
no del papel) supere los 2000 grs. 
c) Imprimir por pantalla el número de serie y hora de fabricación de todas las resmas que han 
sido fabricadas entre las 06:00:00 hs. y las 10:30:00 hs, ordenadas Por número de serie.