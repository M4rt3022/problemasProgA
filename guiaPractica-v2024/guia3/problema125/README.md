# PROBLEMA 125

Dos Empresas dedicadas a la fabricación de DVD transfieren información relevante de la 
producción a través de un archivo binario que se llama “datosdvd.bin”. La Empresa número 1 
se dedica a la fabricación del DVD virgen con la caja, la segunda empresa se encarga de 
grabar, etiquetar y distribuir cada uno de los DVD que le llegan de acuerdo a la demanda del 
publico. El archivo binario a través del cual se transfiere la información entre las empresas, 
posee los siguientes datos: 
- Numero de serie (entero largo positivo) 
- Color (string) 
- Control de Calidad (string: Ver más abajo el formato de este campo) 
- Capacidad (entero largo). 
- Tipo (string: M=Musica, V=Video, S=Software Operativo, A= Software de Aplicación, 
I=Multimedia, ver más abajo) 
- Distribuidora (string) 
La empresa 1 llena solamente los campos numero de serie, color y control de calidad, siendo 
este último un string de la forma E1nn donde nn es 00 si esta defectuoso, 01 si posee una cara 
útil, 10 si posee la otra cara útil y 11 si las dos caras son útiles. 
La Empresa 2 al recibir el archivo completa la estructura con todos los datos faltantes, agregando 
al campo control de calidad un string de la forma E2xx, donde xx significa: 00 si no se pudo 
grabar la información, 11 si la grabación fue un éxito y está listo para ser comercializado. 
Importante: El campo tipo por su lado puede ser una combinación de caracteres de acuerdo a 
lo explicitado en la definición (P.ej: M o MV o MSA, etc..., es decir, cualquier combinación válida 
de los caracteres se permite). 
Se pide:
a) Hacer un programa en C que lea el archivo binario enviado por la Empresa 1 y permita la 
carga de la información faltante por la empresa 2 según el proceso explicado (usar 
asignación dinámica de memoria). 
b) Regenerar el archivo binario original, de forma tal que en él solo aparezcan todos los datos 
de aquellos DVD que tienen al menos una cara útil y cuya grabación fue exitosa y que son 
de color “VERDE”, ordenados por número de serie. 
c) Calcular la cantidad de DVD defectuosos entregados por la empresa 1 y la cantidad de DVD 
que no han sido grabados por la Empresa 2. Calcular también el porcentaje que estas dos 
cantidades representan del total de DVD fabricados.