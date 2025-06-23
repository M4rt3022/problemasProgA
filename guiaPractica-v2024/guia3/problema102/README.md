# PROBLEMA 102

Un laboratorio de análisis clínicos lleva el control de calidad del resultado de su trabajo. Para eso 
cuenta con planillas que contienen la siguiente información: 
- Nombre del Paciente (alfanumérico) 
- Fecha del Análisis (alfanumérico; año, mes y día) 
- Colesterol HDL (numérico) 
- Colesterol LDL (numérico) 
- Triglicérido (numérico)
Luego de presentar las planillas a un organismo de control, se recibe un listado de 17 fechas en 
las cuales los resultados están fuera de los estándares proporcionados por tal organismo y se 
deben eliminar de la base. 
Hacer un programa en C que permita: 
a) Ingresar los datos de las planillas (Suponga que existe una cantidad N de datos)  
b) Mediante un algoritmo de búsqueda binaria permitir encontrar las fechas que han sido 
reportadas como dudosas (un total de 17 fechas) y eliminarlas del conjunto de registros de la 
base (para esto se deberán ingresar todas las fechas al mismo tiempo). 
El funcionamiento del programa debe ser automático en el sentido de que el usuario ingresa la 
totalidad de los datos y de las fechas. El programa deberá listar por pantalla la información que 
se considera correcta sin intervención del operador.