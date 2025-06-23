# PROBLEMA 133

Una fábrica dispone de una archivo con información de sus productos denominado prod.bdd 
con la siguiente información: 
- Código del producto (entero sin signo) 
- Nombre del Producto (string de 25 caracteres) 
- Tipo de producto (carácter) 
- Cantidad de productos en stock (entero) 
- Precio Unitario del producto (real) 
- Fecha última reposición de productos (string aaaammdd). 
Se pide realizar un programa en C que ejecute lo siguiente: 
a) Volcar la información del archivo a la memoria utilizando asignación dinámica. 
b) Realizar un listado ordenado por tipo de producto y nombre de producto de aquellos productos 
con fecha de última reposición en el rango dado a continuación. Se debe permitir el ingreso 
de una fecha por teclado, se calcula el rango como la fecha ingresada y la fecha de un año 
antes de esta. 
c) Generar un nuevo arreglo de estructuras que contenga código y cantidad de productos cuyo 
stock esté por debajo de 10. 
d) Generar un archivo de texto con la información contenida en el arreglo generado en el punto 
anterior. 
e) Calcular el capital disponible de la empresa ( total de cantidad de productos por precio 
unitario). Este valor también deberá guardarse en el archivo generado en el punto anterior.