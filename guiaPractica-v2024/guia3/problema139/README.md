# PROBLEMA 139

Los datos relevantes de un grupo de alumnos de la Facultad de Ingeniería son: 
- Nombre (Cadena de caracteres) 
- Registro (Entero) 
- Código de especialidad (Carácter) 
- Cantidad de exámenes rendidos (Entero) 
- Notas de los exámenes (un conjunto de hasta 60 notas posibles). 
- Promedio de los exámenes (Real, sin incluir los aplazos. Este miembro no debe ser 
ingresado, debe ser calculado por el programa). 
Se pide escribir un programa en C que sea capaz de leer estos datos de todos los alumnos desde 
un archivo de texto cuyo nombre se debe ingresar por teclado. El archivo tiene extensión “.txt” y 
está ubicado en la unidad E:\ del disco duro.  
Se pide: 
a) Listar todos los alumnos que no tienen ningún examen reprobado, ordenados por código de 
especialidad y registro. 
b) Se debe ingresar por teclado el código de una especialidad. Con estos valores crear un 
nuevo arreglo de estructuras de otro tipo con los datos correspondientes a Nombre, 
Número de Registro y Promedio formado por todos los datos de todos los alumnos que 
pertenezcan a la especialidad ingresada. Usar asignación dinámica de memoria.  
c) Listar todos los datos correspondientes a los alumnos del arreglo creado, cuyo promedio sea 
superior a 6 (seis). 
d) Calcular y mostrar el promedio de notas correspondiente a cada especialidad. Indicar cuál 
es la especialidad que posee mayor promedio y mostrar su valor. 
e) Generar un archivo binario de nombre “Mejores.bin” que contenga el Nombre, registro, 
especialidad y promedio de notas de los mejores alumnos de cada especialidad.