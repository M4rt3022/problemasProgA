# PROBLEMA 136

Una empresa dedicada al riego por goteo dispone de un archivo binario denominado 
“clientes.bdd” con los cuales desea relevar cierta información estadística. Por cada propiedad de 
los clientes dispone de la siguiente información en el archivo: 
- Nombre del Cliente (string de 30 caracteres) 
- Cantidad de Hectáreas de propiedad (entero) 
- Numero de experimentos a realizar (entero por defecto 0) 
- Gotas por Hora por Experimento (arreglo de 100 enteros) 
- Rendimiento de las plantas (arreglo de 100 floats) 
La información en el archivo esta disponible parcialmente. 
Se desea: 
a) Leer el archivo binario utilizando asignación dinámica de memoria. Completar los datos de 
acuerdo al resultado de cada experimento. Los datos a completar son Numero de 
experimentos, Gotas por hora por experimento y rendimiento. Para poder llevar a cabo esta 
tarea se deberá requerir al operador (por teclado) el nombre de un Cliente y completar la 
información necesaria. Debe tener en cuenta que un mismo Cliente puede poseer mas de una 
estructura, este proceso finaliza cuando el nombre del cliente comience con la las letras 
“RPN”. 
b) Listar todos los datos de las clientes a los que se les haya completado la información ordenado 
por Nombre de cliente y cantidad de hectáreas. 
c) Generar un archivo de texto con la información del Cliente que más experimentos haya 
realizado. En caso de igualdad se deberá considerar el de mayor cantidad de hectáreas. El 
nombre del archivo debe ser, el nombre del cliente (8 primeros caracteres) y extensión “.txt”. 
La información a grabar en el archivo debe ser: Cantidad Total de hectáreas, Número total de 
experimentos, Promedio de rendimiento, Máximo y Mínimo rendimiento obtenido.