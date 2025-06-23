# PROBLEMA 121

Una empresa dedicada a la fabricación de diskettes desea relevar información de la producción. 
A cada disquete se le asocian los siguientes datos: 
- Número de Serie (long) 
- Tipo (String: FD1.44, FD1.2,FD720, FD360) 
- Calidad (entero: 10-8: Buena, 7-5: Regular, 5-0: Mala) 
- Color caja (String) 
- Test( Carácter: 'A': Aprobado, 'R': Rechazado) 
Se dispone de un archivo binario denominado diskette.bin con la información de la producción 
de los disquetes. Se pide: 
a) Leer el contenido del archivo (con asignación dinámica de memoria). 
b) Analizar cada disquete y llenar el campo test de acuerdo a la calidad de cada uno, siendo 
'A'= Calidad buena, 'R'= calidad regular o mala. 
c) Generar un archivo de texto (ASCII) denominado buenos.txt, en el directorio c:\diskettes 
con la información de los disquetes aceptados ordenados por tipo. 
d) Hacer un listado ordenado por test y tipo indicando el porcentaje de disquetes aprobados y 
rechazados para cada tipo.