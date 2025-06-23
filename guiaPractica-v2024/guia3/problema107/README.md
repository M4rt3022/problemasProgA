# PROBLEMA 107

El servicio meteorológico nacional posee varias estaciones meteorológicas en diferentes puntos 
de la república. Cada estación envía el central los datos recopilados durante un día de 
mediciones. La información entregada se ajusta a una estructura del tipo: 
- Número de estación (entero largo sin signo) 
- Ubicación ( alfanumérico de 25 caracteres) 
- Temperatura ( arreglo de 24 datos flotantes, medición por hora del día) 
- Temp_max (flotante) 
- Hora (entero) 
- Fecha ( string de 9 caracteres, con la fecha actual) 
Se pide un programa en C que realice lo siguiente: 
a) asumir que el servicio posee N estaciones, realizando la reserva dinámica de memoria para 
un mes de mediciones (30 días). 
b) Carga de las mediciones para el mes. 
c) Calcular la temperatura máxima de cada  estación para ada día y almacenarlo en el miembro 
de la estructura correspondiente, llenando también la hora a la cual se produjo.    
d) Un listado ordenado por fecha y número de estación, siempre y cuando la temperatura máxima 
registrada sea superior a los 35 grados. 
e) Permitir por teclado el ingreso de una fecha y buscar la estación que registró la temperatura 
máxima durante ese día, mostrar todos los elementos de la estructura.