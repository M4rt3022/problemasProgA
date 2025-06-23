# PROBLEMA 119

Una compañía fabricante de tornillos recibe diariamente por correo electrónico un archivo 
binario conteniendo las especificaciones de los tornillos que fabricará ese día. El archivo 
consiste en un conjunto de bloques de datos que contienen las siguientes especificaciones: 
- Código  o tipo del tornillo (alfanumérico de 12 caracteres válidos). 
- Sistema de medida del tornillo (un único carácter: M -> métrico, P -> pulgadas) 
- Largo del tornillo en mm (Real) 
- Diámetro del tornillo en mm (Real) 
- Número de filetes por unidad de medida (entero) 
- Cantidad de tornillos a fabricar con esas especificaciones (entero) 
La empresa dispone de un torno de mando numérico que fabrica automáticamente los tornillos,  
el cual requiere que la información de cada tipo de tornillo a construir le sea entregada en un 
archivo de texto. Es necesario entonces construir a partir del archivo binario recibido un conjunto 
de archivos de texto (uno para cada tipo de tornillo) cuyo nombre sea igual a los ocho primeros 
caracteres del código y con la extensión .tor. La información contenida en cada archivo así 
generado es la misma que existe en el bloque de datos correspondiente con la excepción del 
código del tornillo.  La generación de los archivos debe hacerse ordenada por código.  
Se deberá listar por pantalla aquellos tipos de tornillo fabricados en el sistema métrico cuyo 
volumen total de material utilizado no supere 150000 mm3. 
Se deberá ingresar por teclado un tipo de tornillo  especificado, e indicar el número  total de 
filetes que este posee, ordenados por cantidad a fabricar.