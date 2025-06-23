# PROBLEMA 134

La Facultad de Ingeniería necesita de un programa en C para evaluar el rendimiento de los 
alumnos durante el cursado, para cada una de las 12 Carreras de Grado. Sección alumno 
entrega la información de cada alumno en un archivo binario con la siguiente información: 
- Numero de registro del alumno; 
- Nombre de la Carrera a la que pertenece 
- Semestre de cursado 
- Cantidad de materias que cursa 
A su vez se dispone de un archivo de texto con la siguiente información: 
- Numero de registro del alumno 
- Cantidad de materias que cursa 
- Nota de cada una de las materias que cursa. 
En cada uno de estos archivos existe solo un registro por cada alumno de la Facultad. Se pide: 
a) Realizar la carga de los datos de cada alumno que se encuentra en los archivos. Esto se 
debe hacer en forma dinámica respetando la siguiente estructura de datos 
- Numero de registro del alumno (entero largo sin signo) 
- Nombre de la Carrera a la que pertenece (string de 40 caracteres válidos) 
- Semestre de cursado (entero sin signo) 
- Cantidad de materias que cursa (entero sin signo) 
- Arreglo de 10 enteros con las notas obtenidas por los alumnos en cada una de las 
asignaturas que cursa. 
- Promedio de notas. 
b) Calcular la nota promedio por alumno y almacenarla en la estructura (llenar el campo vacío). 
c) Calcular las notas promedio por Carrera.
d) Realizar un listado ordenado por Carrera y Semestre de la nota promedio de los exámenes, 
indicando en cada caso la cantidad de alumnos que han rendido. 
e) Generar un archivo binario con el nombre de la Carrera, Semestre y nota promedio, solo de 
aquellas Carreras en las cuales la nota promedio ha superado los 6 puntos.