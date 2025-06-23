# PROBLEMA 124

Una empresa de telefonía lleva un registro detallado de cada uno de los teléfonos que produce. 
La información relevante para cada uno de ellos es la siguiente: 
- Número de serie del teléfono (string de 10 caracteres alfanuméricos con el siguiente 
formato: LnnSxxTyyy, donde nn son dos dígitos que indican el número de lote, ss son dos
dígitos que indican el número de  semana del año cuando se fabricó el teléfono e yyy son 
tres letras minúsculas que indican el tipo de teléfono: ang si es analógico o dig si es digital). 
- Cantidad de memorias para discado rápido (entero positivo). 
- Color del teléfono (string que puede tomar los valores “BLANCO”, “GRIS” o “NEGRO”) 
- Calidad de fabricación (entero positivo que puede tomar los siguientes valores: 0 si es de 
primera calidad, 1 si es de segunda calidad o –1 si es para descarte). 
Los datos de la fabricación del último año se encuentran grabados en un archivo binario con el 
nombre “telefono.bin”, pero se desconoce la cantidad de registros grabados en el mismo (hay 
que contarlos). 
Se necesita un programa en lenguaje C que permita las siguientes operaciones sobre estos datos: 
a) Cargar desde disco a memoria todos los datos del archivo telefono.bin (es obligatorio usar 
asignación dinámica de memoria). 
b) Listar por pantalla el número de serie y la calidad de fabricación de todos los teléfonos 
negros que tienen más de cuatro (4) memorias de discado rápido, ordenados por numero 
de serie. 
c) Generar un archivo de tipo texto (ASCII), llamado descarte.txt, con todos los datos de los 
teléfonos cuya calidad es de descarte, que pertenezcan al lote número 13 y que hayan sido 
fabricados antes de la semana 24. 
d) Calcular y mostrar la cantidad de teléfonos y el porcentaje que ella representa sobre el total, 
de todos aquellos teléfonos GRISES cuya calidad es de segunda.