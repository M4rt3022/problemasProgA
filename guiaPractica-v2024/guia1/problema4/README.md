# PROBLEMA 4

Realizar un algoritmo que permita leer un valor R y un conjunto de N de números reales (máximo 
100), y que calcule y escriba: 
a) La cantidad de valores mayores que el primero ingresado. 
b) El promedio de los valores positivos menores que R. 
c) El porcentaje de valores positivos pares.
# RESOLUCION PROBLEMA 4
    #include <stdio.h>
        int main( ) {
        int cont=0, cont_rechaz=1, cont_acept = 0;
        float prom, espesor, suma=0, max_espesor=-1;
        printf("\nIngrese el espesor: ");
        scanf("%f%*c", &espesor);
        while( (espesor >= 0.) && (cont<1000) ) {
            cont++;
            if(espesor <= 1.5 && espesor >= 1.1){/*Caso en que el espesor es aceptado*/
                suma += espesor;
                cont_acept++;
            }
            else{
                cont_rechaz++;
            }
            if( espesor > max_espesor ) {
                max_espesor = espesor;
            }
            printf( "\nIngrese el espesor:" );
            scanf( "%f%*c", &espesor );
        }
        if( cont > 0 ) {
            printf("Botellas que no cumplen especificacion es: %d\n", cont_rechaz);
            if( cont_acept > 0 ) {
                prom=(float)suma / cont_acept;
            } else {
                prom=0;
            }
            printf("El promedio de las botellas aceptadas es: %f\n ", prom);
            printf("El mayor espesor de botellas ingresado es: %f\n", max_espesor);
        }
        else {
            printf("No se ingresaron valores para poder procesar\n");
        }
        return 0;
    }
