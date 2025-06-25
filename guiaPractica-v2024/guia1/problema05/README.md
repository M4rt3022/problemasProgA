# PROBLEMA 5

Una fábrica de botellas requiere que el espesor del vidrio de sus productos esté comprendido en el 
rango de 1,1 y 1,5mm. Leer como máximo 1000 valores de espesor o terminar la lectura si el valor 
ingresado es negativo. Calcular e imprimir: 
a) La cantidad de botellas que no cumplen la especificación. 
b) El promedio de espesor de las botellas que cumplen la especificación.
c) Mostrar el mayor espesor de los productos ingresados.
d) Hacer un análisis del funcionamiento del algoritmo mediante un conjunto de datos de prueba, 
completando los valores de la tabla, tal como el ejemplo modelo.
|espesor|cont|max_espesor|suma|cont_rechaz|prom|
||1|||||
||2|||||
||3|||||
||4|||||
||5|||||
||6|||||
|-1||||||

# RESOLUCION PROBLEMA 5
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
