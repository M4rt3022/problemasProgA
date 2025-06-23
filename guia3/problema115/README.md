# PROBLEMA 115

Una fábrica de cables desea evaluar los resultados de su producción durante un mes para 
realizar el control de calidad de la misma. Los datos de los lotes de cables fabricados son: 
- Número de Lote (entero positivo de cuatro cifras) 
- Fecha de fabricación (cadena de 7 caracteres -> aammdd) 
- Peso del cobre utilizado (real) 
- Longitud del cable fabricado (real) 
- Color del aislante (cadena de caracteres) 
- Peso del aislante por metro de cable (real) 
Los datos de la producción de un mes se encuentran ya grabados en un archivo tipo ASCII. 
Se pide generar un programa en lenguaje C que lea los datos de este archivo y los procese 
para obtener: 
a) Un archivo binario que contenga los números de lote, longitud del cable y peso del cobre de 
todos los lotes cuyo color del aislante coincidan con uno ingresado por el usuario mediante 
teclado, ordenado por número creciente de lote. El nombre de este archivo será el nombre 
del color seleccionado con la extensión .CBL (debe ser un nombre DOS válido)
b) Un archivo ASCII que contenga los números de lote, longitud del cable y peso del cobre de 
todos los lotes cuya longitud de cable sea igual a un valor ingresado por el usuario por 
teclado con una tolerancia del 10% en más o menos, ordenados por fecha de producción. 
c) Un listado por pantalla de los datos de todos los lotes fabricados en el mes que tengan un 
peso de cobre superior al peso del lote correspondiente al que posee menor numero de lote.