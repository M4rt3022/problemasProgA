# PROBLEMA 140

Un instituto de capacitación recibe inscripciones para sus cursos de verano. Para cada inscripto 
se disponen de los siguientes datos.  
- Apellido y nombre 
- Edad 
- Cantidad de cursos que va a tomar 
- Código de cada uno de los cursos en los que se inscribió (arreglo de enteros máximo 5 
elementos) 
- Turno elegido para todos los cursos. (M  Mañana ó T  Tarde).  
- Monto a pagar  (este campo no está en el archivo, pero debe ser incluido en la estructura) 
Los cursos están codificados con enteros de la siguiente manera: 
0->Matemática 
1->Física 
2->Química 
3->Computación 
4->Redes 
5->Sistemas Contables.  
Implementar un programa en lenguaje C que realice las siguientes tareas:
Los datos de los inscriptos se encuentran almacenados en un archivo de texto "Inscrip.txt", estos 
datos deberán transferirse a memoria utilizando asignación dinámica y previendo que se pueden 
agregar unos cincuenta alumnos más a los ya inscriptos. 
Mediante un menú de opciones se deben realizar los siguientes ítems: 
a) Permitir la inscripción de un alumno en un curso. Puede pasar que el alumno sea nuevo, o 
bien que el alumno ya esté inscripto en algún curso y quiera hacerlo en otro, para esto se le 
debe requerir al operador la información que sea necesaria según el caso. Se debe tener en 
cuenta de que un alumno no podrá inscribirse dos veces en el mismo curso, y que para los 
cursos de Matemática  y Física no admiten más de 30 alumnos por turno y que la cantidad 
total de alumnos no supere lo previsto en la reserva de memoria.  
b) (*) Permitir eliminar la inscripción de un alumno a un curso. En el caso que el alumno no esté 
inscripto en ningún curso, se lo debe borrar del arreglo de estructuras. 
c) Calcular y almacenar el monto a pagar de cada uno de los alumnos teniendo en cuenta que 
los cursos de Química y Matemática cuestan $190 c/u, y el resto $240 c/u. 
d) Ingresar por teclado un turno y generar un archivo binario que contenga los datos de los 
inscriptos en ese turno ordenado alfabéticamente por Apellido y nombre, escribiendo: Apellido 
y nombre, cantidad de cursos y el nombre completo de cada uno de los cursos en los que 
se inscribieron. El nombre del archivo  estará formado por una primera letra que corresponde 
al turno ingresado, seguido del año que deberá ser leído también por teclado y con la 
extensión ".dat" 
e) Calcular cual es el curso que tiene más inscriptos indicando el nombre del curso 
correspondiente.