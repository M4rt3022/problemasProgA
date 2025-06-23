# PROBLEMA 58

Genere una matriz cuadrada de dimensión n. Los elementos de la misma deben ser enteros y 
creados aleatoriamente mediante la función srand(), correspondiente a la biblioteca stdlib.h. 
Cada elemento debe estar acotado entre los valores 0 y 25. La función srand() se utiliza para 
generar valores aleatorios y se encuentra definido y explicado su modo de funcionamiento en la 
guía de trabajos prácticos de funciones y strings. Se pide invertir los elementos que están por 
encima de la diagonal principal por los que están por debajo de la diagonal, tal como se puede 
ver a continuación: 
    1 2 3       1 4 7            
De  4 5 6   a   2 5 8    
    7 8 9       3 6 9