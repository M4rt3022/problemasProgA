# PROBLEMA 109

Cree una agenda telefónica, en la cual se debe ingresar los siguientes datos por teclado: 
 Número de orden (Entero) 
 Nombre del abonado(String de 30 caracteres) (con formato: Apellido,Nombre) 
 Número de teléfono (String de 14 caracteres)
La lectura de los datos por teclado (sobre un arreglo de estructuras), finaliza cuando se ingrese 
un nombre de abonado “ultimo” o cuando se llegue al máximo previsto por la dimensión del 
arreglo. Luego, estos datos se deben guardar en archivo de texto cuyo nombre es “agenda” con 
extensión “txt”. Cada miembro de la estructura debe estar separado por un espacio en blanco. 
# NOTAS

revisar topdown subido a la carpeta

La lectura de los datos por teclado (sobre un arreglo de estructuras), finaliza cuando se ingrese 
un nombre de abonado “ultimo” o cuando se llegue al máximo previsto por la dimensión del 
arreglo. Luego, estos datos se deben guardar en archivo de texto cuyo nombre es “agenda” con 
extensión “txt”. Cada miembro de la estructura debe estar separado por un espacio en blanco. 
Para comenzar a resolver este problema, primero se aplica el método de análisis Top Down 
antes de editar el código en lenguaje C, usando las funciones necesarias. El problema se 
subdivide básicamente en tres partes que consiste en: Leer los datos por teclado, mostrar los 
datos leídos y guardar los mismos en el archivo, tal como se muestra a continuación. 
Si bien, cada bloque del diagrama de árbol representa un nodo del mismo, estos establecen 
una función dentro del main() del programa en C. Sin embargo, se observa que se debería 
desarrollar cada uno de ellos para poder comprender mejor la solución del problema.

Nodo 1:  
En este nodo se desarrolla la lectura de los datos, el cual se puede observar a continuación:
//revisar archivos adjuntos
En el enunciado no se estableció que se debían almacenar los datos en un arreglo dinámico, 
por lo tanto, se usa un arreglo estático.  
Por lo tanto, la función de lectura tiene como argumento de entrada un arreglo de estructuras, 
cuyos datos se pueden actualizar en la función y como única salida la cantidad de abonados 
válidos almacenados dentro de dicho arreglo, tal como se muestra a continuación. A la función 
de lectura se le puede llamar carga_abo.
La función tiene como: 
Entrada: AGENDA *age
Salida:   int i
La misma se desarrolla a continuación, respetando la secuencia establecida en el diagrama de 
árbol.
Como se puede observar, desde la función main se puede invocar a esta función de carga 
utilizando como argumento de entrada un arreglo estático, el cual es recibido por esta misma 
función de lectura como una dirección de memoria. Esto siempre ocurre cada vez que se 
ingresan arreglos como entrada de cualquier función, es por ello que dichos arreglos siempre se 
pueden actualizar sus datos.  
El algoritmo de lectura es típico, en el cual se utiliza una función de repetición while que evalúa 
las condiciones de entrada pedidas en el enunciado. 
Se devuelve el valor de índice i, que corresponde a la cantidad natural de abonados. 
 
Nodo 2: En este nodo se desarrolla la muestra de los datos leídos por teclado. De antemano 
debe ser un algoritmo sencillo, el cual se puede observar a continuación: 
//revisar archivos adjuntos
Este nodo simplemente se puede resolver mediante una única y clásica función de muestra de 
datos, la cual se puede denominar “mostrar”. La misma necesita de una instrucción de 
repetición para que los datos se vean en la pantalla. A diferencia de la función de lectura, esta 
debe tener como argumentos de entrada el arreglo de estructuras que contiene los datos y la 
cantidad de datos válidos que contiene el arreglo. No necesita que devuelva ningún valor de 
salida. 
El código en C de esta función se muestra a continuación.
// adjuntar código
Esta misma función de muestra simplemente incorpora la instrucción for para hacer la 
repetición.
Nodo 3: En este nodo se guarda la información del arreglo en un archivo texto. De antemano 
debe ser un algoritmo sencillo, el cual se puede observar a continuación:
// revisar archivos adjuntos
Este nodo se puede resolver mediante una única función que guarde los datos en el archivo 
agenda.txt, la cual se puede denominar “grabar”. 
Esta función tiene como misión abrir el archivo, verificar inmediatamente si existe un error de 
apertura del mismo y en caso de que no haya ningún error, se pueden almacenar los datos del 
arreglo de estructura. En caso contrario, se deberá informar por pantalla acerca del error 
producido. Por último se deberá cerrar el archivo en esta función grabar. 
Al igual que la función mostrar, la función grabar tiene los mismos argumentos de entrada y no 
devuelve ningún valor de salida.
A continuación se muestra el código en lenguaje C de esta función, que respeta el análisis 
hecho mediante la descomposición Top Down. El almacenamiento de los datos al disco duro 
deberá hacerse bajo la condición que no haya ningún error en la apertura del archivo 
agenda.txt
// adjuntar código
Se puede observar en el código en C que se necesitó de una bandera indicativa, como es la 
variable “band”, para verificar si hubo error de lectura del archivo.  
Por último, la función main simplemente consiste en invocar a las funciones desarrolladas 
previamente. Estas funciones están relacionadas con los nodos 1, 2 y 3 del esquema del 
diagrama de árbol.
//adjuntar código