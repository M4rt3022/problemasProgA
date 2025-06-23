# PROBLEMA 114

Una empresa que produce aceites, almacena los datos de la producción diaria de cada una de 
sus 2 filiales en estructuras del tipo: 
- Nombre del aceite (char) 
- Precio de Venta (float) 
- Cantidad Vendida (entero) 
- día (char) 
Se cuenta con un archivo binario que posee la información de la producción por día de un cierto 
periodo de la primer filial, ordenado de menor a mayor por Cantidad Vendida. Así mismo, existe 
un archivo binario correspondiente al mismo periodo de la segunda filial desordenado. 
Se solicita: 
a) Intercalar los datos de ambos archivos en un único arreglo de estructuras ordenado por el 
campo Cantidad Vendida y almacenarlo en un nuevo archivo texto. 
b) Calcular el promedio de las ventas de cada filial y el de la producción conjunta (pesos) por 
día. 
c) Contar cuantas ventas de la primer filial superaron el promedio conjunto de ventas calculado 
en el punto anterior.