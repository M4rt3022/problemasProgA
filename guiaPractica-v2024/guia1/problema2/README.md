# PROBLEMA 2

Leer datos enteros hasta que se llegue a 1000 elementos o que el dato ingresado sea igual a –50. 
Calcular e imprimir: 
a) La cantidad de elementos ingresados 
b) El porcentaje de elementos pares. 
c) El promedio de todos los datos ingresados, excluyendo si se ingresa el –50. 

# NOTAS
Recordar que el operador %(módulo) se usa para obtener al resto de la división entera.
# RESOLUCION PROBLEMA 2
    #include <stdio.h>
        int main( ) {
        int dato=0, cont_total=0, cont_par=0, sum=0;
        float porc=0, prom=0;
        printf("\n Ingrese el dato: ");
        scanf("%d%*c", &dato);
        while( (dato!=-50) && (cont_total!=1000) ) {
            cont_total++;
            if(dato % 2 == 0){
                cont_par++;
            }
            sum+=dato;
            printf ("\n Ingrese el dato: ");
            scanf("%d%*c", &dato);
        }
        printf ("\n La cantidad de elementos es: %d", cont_total);
        if( cont_total!=0 ) {
            porc =(float)(cont_par*100)/cont_total;
            prom =(float)sum/cont_total;
            }
        printf( "El porcentaje de los pares es: %8.2f\%\n", porc );
        printf( "El promedio de los datos ingresados es: %8.2f\n", prom);
        return 0;
    }
