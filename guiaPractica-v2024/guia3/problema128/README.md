# PROBLEMA 128

Una editora de libros desea contar con información relativa a la fabricación de sus productos. 
Para ello nos envía un archivo en formato texto denominado “libros.txt” con información de su 
producción. Para cada conjuntos de libros producidos el archivo contiene la siguiente 
información de cada uno de los libros: 
- Titulo del libro (máximo 50 caracteres). 
- Autor(máximo 30 caracteres) 
- Cantidad de paginas
- Precio 
- Presentación (caracter D: Tapas duras, B:Tapas blandas) 
- Cantidad de libros. 
Se pide realizar un programa en lenguaje C que permita procesar esta información: 
a) Leer los datos de cada libro a un arreglo dinámico en memoria. 
b) Calcule el precio de cada libro y se llene el campo de la estructura correspondiente teniendo 
en cuenta que cada página cuesta $0.001 y la encuadernación de tapas blandas $5 y de 
tapas duras $8.  
c) Generar un archivo binario denominado “libros2.bdd” ordenado por Autor y simultáneamente 
por cantidad de paginas con la siguiente información: Título del Libro, Autor. numero de 
paginas y precio. 
d) Permitir que el usuario introduzca una cierta cantidad de lestras del nombre del Autor vía 
teclado y muestre la información para cada Autor  que sus primeras letras coincidan con las 
letras ingresadas toda la información de cada uno de sus libros.