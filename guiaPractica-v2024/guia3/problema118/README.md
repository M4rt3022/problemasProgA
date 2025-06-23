# PROBLEMA 118

Dada la siguiente estructura de datos: 
struct Integrado{ 
int Codigo; 
int Cantidad; 
float PrecioUnitario; 
char Descripcion[40]; 
char Proveedor[40]; 
}; 
Realizar un programa en lenguaje C que permita: 
a) Leer todas las estructuras del tipo mencionado, que existan en el archivo A:\circ.dat", el 
cual es de tipo binario. 
b) Ingresar nuevas estructuras tomando los datos desde teclado. 
c) Ordenar las estructuras por el campo Código en forma creciente y guardarlas ordenadas en 
el archivo de tipo ascii "c:\almacen\lista.txt" 
d) Actualizar el archivo binario "c:\almacen\circ.dat" 
El programa, al iniciarse, debe reservar memoria, levantar todas las estructuras existentes y 
presentar un menú de opciones al usuario, a fin de que realice cualquiera de las operaciones 
descriptas o pueda abandonar el programa. Cuando se realiza la reserva de memoria prever 
que se deben agregar nuevas estructuras y cuando se agregan de no superar la memoria 
solicitada.