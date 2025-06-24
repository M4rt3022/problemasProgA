# PROBLEMA 16

Se desea procesar la información del tipo de mercadería proveniente de los camiones de una 
empresa que realiza entregas a domicilio. Para ello se cuenta con la siguiente información cada 
paquete:  
- Código de identificación del paquete (entero corto) 
- forma de entrega del paquete (carácter: ‘i’ inmediata, ‘m’ moderada, ‘c’ corriente),  
- peso del paquete (en gramos), 
- distancia que recorrió (en Km).  
Se pide que se ingrese información hasta que se tenga un peso negativo o la distancia sea mayor a 
3000 Km. Se pide calcular: 
a) El promedio de peso de paquetes a entregar con peso mayor a 4000 gramos y que no necesiten 
entregarse en forma inmediata.
b) Indicar por pantalla aquellos paquetes que no recorrieron larga distancia (menor a 12Km), y con 
código de identificación entre 150 y 215. 
c) ¿Qué forma de entrega de paquetes se realiza con mayor frecuencia. Indique el porcentaje sobre 
el total de paquetes entregados. 
d) Cuanto se recaudó en total, sabiendo que el precio base es de $2, agregándose $0,10 por cada 
3Km y $0,05 por cada 100grs de exceso al peso límite sin cargo de unos 200grs.
e) Hacer un análisis del funcionamiento del algoritmo mediante un conjunto de datos de prueba , 
completando en una tabla los valores de las variables más significantes del algoritmo, tal como el 
ejemplo modelo.
# RESOLUCION PROBLEMA 16
    #include <stdio.h>
        int main( ) {
        int codigo,conttotal=0,contpeso=0,contI=0,contM=0,contC=0;
        float peso, prom, porc, dist, sumapeso=0,recaud=0,agregoKm,agregoKg;
        char formae;
        printf("Ingrese peso:\n");
        scanf("%f%*c", &peso);
        printf("Ingrese distancia:\n");
        scanf("%f%*c", &dist);
        printf("Ingrese forma de entrega:\n");
        scanf("%c%*c", &formae);
        while( peso > 0 && dist < 3000) {
        printf("Ingrese codigo de identificacion:\n");
        scanf("%d%*c", &codigo);
        conttotal++;
        if( peso > 4000 && formae != 'i' ) {
            sumapeso += peso;
            contpeso++;
        }
        if( dist <= 12 && codigo >= 150 && codigo <= 215 ) {
            printf("El paquete codigo %d no es larga distancia.\n", codigo);
        }
        if( formae == 'i' ) contI++;
        if( formae == 'm' ) contM++;
        if( formae == 'c' ) contC++;
        agregoKm = 0.10 * (((int)dist)/3);
        if( peso <= 200 )
            agregoKg=0;
        else
            agregoKg= (int)((peso-200) / 100) * 0.05;
            recaud += 2; // Precio fijo por paquete
            recaud += agregoKm; // Adicional por distancia
            recaud += agregoKg; // Adicional por peso
            printf("Ingrese peso:\n");
            scanf("%f%*c", &peso);
            printf("Ingrese distancia:\n");
            scanf("%f%*c", &dist);
            printf("Ingrese forma de entrega:\n");
            scanf("%c%*c", &formae);
        }
        if( contpeso > 0 ) {
            printf("Promedio de peso de paquetes a entregar: %f%*c",
            sumapeso/contpeso);
        } else {
            printf("No se entregaron paquetes con la condición de peso promedio.");
        }
        if( contI >= contM && contI >= contC )
            printf("El destino inmediato se hace con un porcentaje de: %f",(float)contI/conttotal*100);
        if( contM > contI && contM >= contC )
            printf("El destino inmediato se hace con mas frecuencia en: %f",(float)contM/conttotal*100);
        if( contC > contM && contC >= contI )
            printf("El destino inmediato se hace con mas frecuencia en un porcentaje de: %f", (float)contC/conttotal*100);
        printf("Se recaudo en total: %f\n", recaud);
        return 0;
    }
