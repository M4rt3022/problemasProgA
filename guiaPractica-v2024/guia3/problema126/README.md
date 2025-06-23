# PROBLEMA 126

La Policía de San Juan está realizando un relevamiento de los conductores de automóviles para 
obtener información del pago o no del incentivo docente. Con tal motivo la información recabada 
para cada conductor es: 
- Nombre y Apellido (string de 40 caracteres) 
- Tipo de vehículo (A=auto, M=moto, C=camioneta) 
- Modelo (string de 15 caracteres) 
- Marca (string de 15 caracteres)
- Monto pagado (real) 
- Fecha actual(string de la forma aaaa-mm-dd) 
- Fecha de Pago (string de la forma aaaa-mm-dd) 
- Condición (carácter) (P = pagado, M= moroso) 
Con esta información se genera un archivo binario de nombre incentiv.bdd que luego es 
enviado a la Sec. de Hacienda para calcular datos estadísticos de importancia. 
Se solicita implementar un programa en lenguaje C que permita realizar las siguientes tareas: 
a) Leer el archivo binario utilizando asignación dinámica de memoria. 
b) Generar un archivo texto denominado Regla.txt con los datos de la base ordenados por tipo 
de vehículo y por nombre de los conductores que han pagado el incentivo docente. 
c) Generar un nuevo archivo binario (ATiempo.bdd) con los datos de los conductores que 
hayan pagado antes del primero de agosto del año 1999 ordenados por fecha de Pago. 
d) Calcular el porcentaje de morosos. 
e) Calcular, por separado, los porcentajes de Autos, motos y camionetas que han pagado el 
incentivo.