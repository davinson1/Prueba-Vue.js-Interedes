#Prueba de ingreso a Interedes SAS

EXAMEN
Prueba practica de vue.js
Usted a sido contratado por la empresa abc para diseñar una aplicación web que permita realizar conversion de divisas, la cual tendra como datos de entrada (Monto, Moneda Origen y Modeda Destino), para ello debera consumir un api que le brindara los datos de tipos de cambio (Divisas) :
1.	Debera crear una cuenta en https://openexchangerates.org/
2.	Una vez verificada su cuenta se dirige a la opcion de “App IDS” y obtendra un App_ID que le permitira consultar el listado de divisas.
 
3.	Este enpoint le permitira obtener la lista de divisas con precio base en dolares en formato JSON

https://openexchangerates.org/api/latest.json?app_id=YOUR_APP_ID

4.	Este enpoint le permitira obtener la lista de los nombres de las divisas a trabajar en formato JSON
https://openexchangerates.org/api/currencies.json?app_id=YOUR_APP_ID

Criterios a evaluar:
1.	El monto no debe aceptar valores negativos, ceros o letras
2.	El monto debe ser un campo numerico
3.	El monto es un campo requerido.
4.	El campo moneda origen es un valor requerido
5.	El campo moneda objetivo es un valor requerido
6.	La lista desplegable de divisas (moneda origen y moneda objetivo) debe concatenar el nombre y sigla por ej: Bitcoin (BTC)
7.	El resultado de la conversion debe indicar la moneda origen y la moneda destino seleccionada por medio de la abreviatura obtenida desde el API por ej:
1 BTC  = 113,226,550,30 COP
8.	El resultado de la conversion debe estar en formato moneda como se aprecia en el mockup abajo.
9.	El aplicativo de debe adaptarse correctamente a cualquier tamaño de dispositivo, usted podra elegir a libertad la biclioteca de css que mejor le parezca para cumplir con este requisito
Resultado esperado:
 
Formula de conversión:
mountConverted = amount / sourceRate * targetRate

Mostrar datos de histórico de precios de  divisas

1.	Para el siguiente ejercicio debera obtener la fecha actual del navegador en formato YYYY-MM-DD y pasarlo como parametro al enpoint:
https://openexchangerates.org/api/historical/ YYYY-MM-DD.json?app_id=YOUR_APP_ID&base=USD

2.	El resultado de la consulta debera plasmarlo en una tabla cumpliendo los siguientes requisitos
Criterios a evaluar:
1.	El historial debe mostrar en pantalla la fecha actual del navegador
2.	Los datos deben estar ordenados en orden alfabetico por nombre de la divisa
3.	La tabla de resultado debe mostrar Nombre, Abreviatura y Precio 
4.	El aplicativo de debe adaptarse correctamente a cualquier tamaño de dispositivo, usted podra elegir a libertad la biclioteca de css que mejor le parezca para cumplir con este requisito

Resultado esperado:
 
