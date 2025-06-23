# PROBLEMA 138

El Gremio que nuclea los docentes de San Juan necesita procesar la información de sus afiliados. 
La información de los  mismos se encuentran guardados en un archivo de texto denominado 
“Afil.txt” que se encuentra ubicado dentro del directorio Recursos del disco C:, teniendo en 
cuenta la siguiente estructura: 
- Apellido y Nombre del Docente (String de 30 caracteres, separados por espacio en blanco) 
- Numero de afiliado (entero largo) 
- Título profesional del docente(String de 15 caracteres) 
- Edad (entero sin signo) 
- Cantidad de cargos que ocupa (Entero sin signo) 
- Cantidad de horas cátedra que dicta todas las escuela (entero sin signo) 
- Antigüedad docente (entero sin signo) 
- Sueldo (Real)  
a) Leer el archivo de texto y asignarlo a un arreglo de estructuras en forma dinámica en la 
memoria, teniendo en cuenta que se pueden agregar nuevos docentes. Se debe dejar a 
criterio del operario si se integran nuevos docentes en la lista. En ese caso es necesario 
actualizar el archivo original inmediatamente. 
b) Completar el sueldo que cobra cada docente, teniendo en cuenta si el docente cobra por cargo 
o por horas cátedras. En caso de que cobre por cargo se debe partir que el sueldo básico es 
1250$, a ello se le debe agregar 1300$ en adicionales por suma fija más  un 15% respecto 
del básico, por cada 5 años de antigüedad que tenga. Un docente con 2 o más cargos solo 
se le agrega una vez la antigüedad y las sumas fijas. En caso de que tenga horas cátedras 
se le debe computar un básico de 120$, más 40$ por cada hora que dicta,  incluyendo un 15% 
más por antigüedad con respecto al total de horas. Pueden existir docentes con cargos y horas 
cátedras. 
c) Generar los respectivos archivos binarios que agrupan los docentes por cada  título 
profesional que posee, donde cada archivo debe tener como nombre las primeras 8 letras del 
título, más la extensión “. bnn”. En dicho archivo se deberá colocar: Apellido y Nombre, número 
de afiliado, antigüedad,  y sueldo. Se recomienda ordenar por título antes de realizar este 
proceso. 
d) Generar un archivo binario  de aquellos docentes que estén a punto de jubilarse. Se debe 
tener en cuenta que la antigüedad llegue o supere los 30 años y sea mayor de 60 años. Se 
exige el  Apellido y Nombre, el número  de Afiliado, la cantidad  de Cargos, la cantidad total 
de horas cátedra. Al final del archivo guardar la cantidad total de docentes en esa condición.  
e) Se dispone de un archivo de texto denominado “Listado.txt”, que contiene los números de 
afiliado y (separado por un tabulador: \t) el monto total en sueldos atrasados que el estado le 
adeuda a cada afiliado. Leer el archivo binario y generar un único string con los  apellidos
separados por un guión (-) y un espacio en blanco de  todos los docentes afiliados en esa 
lista. Mostrar el nuevo string en el main().
# NOTAS

El campo de sueldo se encuentra inicialmente vacío.