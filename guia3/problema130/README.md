# PROBLEMA 130

Un supermercado atiende a los grandes clientes a través de un sistema de computo que genera 
un archivo binario de nombre clientes.bdd. La información contenida en este archivo es la 
siguiente: 
- Nombre del Cliente (string de 30 caracteres) 
- Razón Social (string de 20 caracteres) 
- Fecha del pedido (string, aaaa-mm-dd) 
- Código del producto mas vendido al cliente (entero) 
- Cantidad de productos comprados (entero)
 Monto total de la compra (real) 
Al final del día se extrae información del archivo. Se pide se haga un programa en C que permita 
realizar las siguientes tareas: 
a) Leer el archivo binario utilizando asignación dinámica de memoria  
b) Calcular y mostrar cual fue el código del producto mas vendido durante el día y a que Clientes 
se vendieron. 
c) Generar un archivo ASCII con la información de Nombre del cliente, Razón Social, Código del 
producto más vendido y monto total de la compra solo para aquellos clientes que satisfacen 
la condición dada en b). 
d) Realizar un listado total ordenado por Nombre del Cliente y Código del producto más vendido 
de aquellos clientes que compraron mas de $100 o que la cantidad de productos comprados 
superaron los 40.