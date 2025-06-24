# PROBLEMA 1

Escribir un algoritmo que permita leer un valor entero y un real, que calcule y muestre la potencia del valor 
real elevado al valor entero, utilizando la técnica de productos sucesivos para la potenciación. 

Por teclado se debe ingresar el conjunto de datos de entrada: base y exponente, mediante las 
dos variables declaradas en el ambiente: base y exp. Si bien el resultado final se muestra a 
partir de la variable de salida prod, esta variable sufre ciertos cambios de valores a medida que 
se ejecuta el programa editado en C. Por pantalla se muestra toda la evolución. Por lo que se 
podría utilizar para observar el valor de cda variable a medida que corre el programa. Se 
propone el siguiente conjunto de datos de prueba para verificar el funcionamiento: 
Si se toma como base 2 (variable base=2 ingresada por teclado) y exponente 6 (variable exp=6 
ingresada por teclado). El resultado final será de 26=64 (variable prod=64 que se muestra por 
teclado).
De esta manera se puede verificar que los datos obtenidos en el programa diseñado coinciden 
con los datos calculados antes de hacer correr el programa en C.
# RESOLUCION PROBLEMA 1
    #include <stdio.h>
        int main( ) {
        int base, nro_repeticiones;
        float exp, prod=1;
        printf("\n Ingrese el valor de la base: ");
        scanf("%f%*c", &base);
        printf("\n Ingrese el valor del exponente: ");
        scanf("%d%*c", &exp);
        for( nro_repeticiones=1; nro_repeticiones <= exp; nro_repeticiones++ ) {
            prod *= base; /* Equivale a colocar prod = prod * base */
            printf( "En la repeticion:%d\n", nro_repeticiones);
            printf( "En esta vuelta el valor de producto corresponde:%f\n\n", prod );
        }
        printf("\n\n El valor de la base elevado al exponente es:%f\n", prod );
        return 0;
    }
