# PROBLEMA 137

Una empresa de turismo promociona viajes para estudiantes a distintos destinos dentro de la 
República Argentina. Para esto carga la siguiente información de cada estudiante como 
preinscripción del viaje. 
 Nombre Completo 
 Documento 
 Teléfono 
 Dirección 
 Destino 
Esta información se guarda en un archivo binario cuyo nombre es: viajes.bdd. 
Suponiendo que se dispone de este archivo se pide realizar un programa en C que permita: 
a) Cargar la información del archivo en un arreglo dinámico de memoria. 
b) Permitir que se pueda confirmar el viaje agregando a la información disponible de cada 
estudiante la fecha del viaje, el costo del viaje y un campo carácter de confirmación 
(´C´confirma, otra cosa no confirma). También se debe permitir agregar estudiantes que a 
último momento decidieron realizar el viaje. 
c) Realizar un listado ordenado por Destino y Nombre de estudiante de acuerdo al siguiente 
detalle:
destino
nombre		documento	teléfoto	$costo
...
Total Destino:					$(costo total)
Averiguar cual es el destino mas elegido por los estudiantes y que porcentaje de estudiantes 
representa. (Esta información debe ser mostrada en el main). 
Generar un archivo de texto con la siguiente información: Nombre del estudiante, documento, 
teléfono, destino.