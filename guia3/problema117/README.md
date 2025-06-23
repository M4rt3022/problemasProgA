# PROBLEMA 117

Un hospital dispone de un sistema automático de evaluación de fallas de sus equipos. Este 
sistema, por cada máquina graba en un archivo binario (falla.bin) una estructura con la 
siguiente información: 
- Nombre de la máquina (17 caracteres) 
- Nro. de serie (entero ocho dígitos numéricos) 
- Ubicación (15 caracteres) 
- modelo (5 caracteres) 
- tiempo entre fallas (arreglo de 200 muestras, cada muestra expresada en minutos) 
- MTBF (real) 
El tiempo entre fallas es un arreglo de enteros que almacena los intervalos entre fallas, por 
ejemplo: 60, 30, 45, 15,..., 0, 0, 0, 0.... 
a) Calcular el tiempo medio entre fallas (MTBF) para cada máquina y almacenarlo en el 
campo MTBF de la estructura de datos. Este se calcula como el promedio de los tiempos 
entre fallas para cada maquina. 
b) Almacenar la información en otro archivo (de texto ) falla2.txt, ordenado por MTBF y 
modelo de mayor a menor. 
c) Calcular el MTBF promedio de las máquinas que con número de serie entre 100.000 y 
200.000, y mostrarlo por pantalla.
d) Calcular el porcentaje de máquinas del total cuyo MTBF sea inferior al promedio 
calculado en el punto anterior.