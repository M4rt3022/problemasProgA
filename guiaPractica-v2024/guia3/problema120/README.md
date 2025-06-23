# PROBLEMA 120

Una empresa dedicada al tratamiento de agua desea realizar un algoritmo en lenguaje C para 
procesar la información relativa al proceso durante un año. La información producida por el equipo 
de purificación se almacena en un archivo binario de nombre “purific.bdd” con los siguientes 
datos: 
- fecha de lectura (caracter 9) en formato aaaammdd 
- hora de lectura (caracter 7) en formato hhmmss 
- porcentaje de cloro (real) 
- cantidad de metros cúbicos procesados (real) 
- tiempo de procesamiento (caracter 7) en formato hhmmss 
- estación del año (I, V, O, P) caracter. 
Además se dispone de otro archivo binario con 4 estructuras cuyo nombre es ¨epoca.bdd¨, con 
la siguiente información: 
- estación del año (I, V, O, P) 
- porcentaje de cloro ideal 
- tolerancia del porcentaje de cloro 
- tiempo de procesamiento ideal. 
Realizar un programa en C que realice lo siguiente 
a) Leer la base de datos y almacenarla en un arreglo dinámico de memoria. 
b) Listar ordenado por fecha y hora los datos correspondientes a Primavera y Verano. 
c) Generar un archivo de texto “Audit.txt” que contenga la información de todos aquellos 
registros que cumplan con la especificación , que se encuentra en el segundo archivo, para 
invierno. 
d) Ingresar dos fechas por teclado, buscar y listar todos los registros comprendidos entre ellas.