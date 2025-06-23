# PROBLEMA 135

Un laboratorio de análisis clínicos necesita de un programa en C que le permita obtener 
información acerca de los estudios que realizan. Para este motivo por cada estudio realizado se 
llena la siguiente información: 
- Código del Estudio (string 5 caracteres válidos) 
- Numero de afiliado (entero largo) 
- Obra Social del paciente (string 15 caracteres válidos) 
- Cantidad de Glóbulos Rojos (máximo valor = 15.000.000) 
- Cantidad de Glóbulos Blancos (máximo valor = 50.000) 
- Cantidad de Plaquetas (máximo valor = 1.000.000) 
- Eritrosedimentación (entero) 
- Diagnóstico (string 20 caracteres vacío) 
Esta información se guarda en un archivo binario, cuyo nombre es ingresado por el operador. 
Se pide realizar mediante un programa en C las siguientes tareas: 
a) Leer el archivo binario y asignarlo a un arreglo de estructuras en forma dinámica en la 
memoria. 
b) Para cada uno de los pacientes se debe rellenar el campo diagnostico con la información consignada en 
la tabla siguiente.
condicion							diagnostico
Cantidad de Glóbulos Rojos inferior a 2.000.000. 		anemia
Cantidad de Glóbulos Blancos superior a 15.000 y 
Eritrosedimentación en el rango 10 a 19mm. 			Infección leve 
Cantidad de Glóbulos Blancos superior a 20.000 y 
Eritrosedimentación en el rango 20 a 30mm. 			Infección media
Cantidad de Glóbulos Blancos superior a 35.000 y 
Eritrosedimentación superior a 31 mm 				Infección severa 
Cantidad de plaquetas en el rango 230.000 a 270.000  		Reservado 
En otro caso se deberá indicar por pantalla la información 
concerniente a Cantidad de Glóbulos rojos, blancos y 
plaquetas y requerir al operador que ingrese el diagnostico. 	Ingresado por el operador
Realizar un listado ordenado por Obra Social y Diagnostico de todos los pacientes con  
eritrosedimentación entre 21mm y 35mm. 
d) Generar un archivo de texto cuyo nombre sea COddmmaa.txt. Donde ddmmaa es la fecha 
que debe ser ingresada por el operador. El archivo debe contener la siguiente información y 
según el siguiente formato,  
Obra Social 
Numero de Afiliado Código de Estudio 
... 
Numero de Afiliado  Código de Estudio 
Obra Social 
Numero de Afiliado  Código de Estudio 
...
Numero de Afiliado  Código de Estudio