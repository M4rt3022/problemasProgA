# PROBLEMA 141

Una entidad financiera que administra y gerencia una tarjeta de crédito, al final del día, guarda en 
un archivo de texto toda la información de las compras realizadas por sus clientes durante el día 
que transcurrió. Los datos por cada compra realizada son los siguientes: 
- DNI del usuario (entero largo) 
- Apellido y Nombre del  Usuario (alfanumérico) 
- Código del comercio donde realizó la compra (entero) 
- Hora de la compra (entero largo en la forma hhmmss) 
- Cantidad de tipos de productos comprados (entero de 1 a 10) 
- Cantidades de cada uno de los productos comprados (conjunto de enteros) 
- Precio unitario de cada tipo de los productos comprados (conjunto de reales). 
El archivo se  denomina “CreditMMDD.txt”, donde MMDD corresponde al mes y día del corriente 
año, los cuales deberán en forma separada ingresarse por teclado y validarse sus valores 
antes de usarlos. Se pide diseñar un programa en lenguaje C que realice las siguientes tareas. 
a) Leer el contenido del archivo de texto y almacenarlo en un arreglo dinámico de estructuras. 
Tenga en cuenta que deberá agregar a la estructura arriba descripta un campo destinado a 
almacenar el monto total de la compra para cada usuario. 
b) Calcular el importe total de cada compra, completando el campo correspondiente en la 
estructura de datos. 
c) Se debe calcular y mostrar el monto total que deberá abonar la empresa a cada uno de los 
comercios en los que se realizaron las operaciones de compra (tener en cuenta que en un 
mismo comercio pueden haber comprado más de un usuario). Además, esta misma 
información debe ser almacenada en un archivo de texto de nombre “pagos.txt”, donde se
especifique el código de cada comercio y el monto a pagar, de manera que cada línea en este 
archivo de texto tenga la forma: 
[codigo de comercio] [monto a pagar] 
d) Listar por pantalla los códigos de los comercios en los que se realizó por lo menos una compra 
en un intervalo de tiempo de media hora en más o en menos respecto de una hora y minutos 
ingresados por teclado. 
e) Se dispone de un archivo binario llamado “limite.dtt”, el cual contiene los DNI de todos los 
usuarios y su importe límite de crédito disponible hasta el momento. Este archivo debe ser 
actualizado con aquellos usuarios que hicieron uso de la tarjeta durante el día, descontando 
de dicho límite el monto gastado. En caso de haber un exceso de compra sobre el importe 
límite, este tomará un valor negativo,  en ese caso se deberá mostrar por pantalla el nombre 
y DNI de los usuarios que tienen excedido el límite de compra.