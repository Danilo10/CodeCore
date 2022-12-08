************ CHALLENGES WEEK 03 *************

LUNES 5/12/2022
SIMPLE CALCULATOR

****** Algoritmo SimpleCalculator ********
	
	Mostrar "Ingrese el primer número"
	Leer primerNumero
	Mostrar "Ingrese el segundo número"
	Leer segundoNumero
	Mostrar "Ingrese la operación que desea realizar: +, -, *, /"
	Leer operacion
	
	Si operacion == "+" | operacion == "-" | operacion == "*" | operacion == "/" Entonces
		imprimir "Procesando: " + " " + ConvertirATexto(primerNumero) +" " + operacion + " " + ConvertirATexto(segundoNumero)
		Si (operacion == "+") Entonces
			//Mostrar "El resultado de la suma es:" primerNumero + segundoNumero
			//Imprimir "Resultado: " + ConvertirATexto(primerNumero + segundoNumero)
			Imprimir "Resultado: " primerNumero + segundoNumero
		SiNo
			Si (operacion == "-") Entonces
				Imprimir "Resultado: " primerNumero + segundoNumero
			SiNo
				si (operacion == "*") Entonces
					Imprimir "Resultado: " primerNumero * segundoNumero
					SiNo
						si (operacion == "/") Entonces
							Imprimir "Resultado: " primerNumero / segundoNumero
						FinSi
					FinSi
				FinSi
			FinSi
		SiNo
			Imprimir "La operación no es válida"
	FinSi
FinAlgoritmo

********* SPECIAL NUMBER **********
Algoritmo specialNumber
		Leer n
		Si n == 100 Entonces
			Imprimir 'This is a special number'
		SiNo
			Si (n < 1000) & (n % 10 == 0) & (n<>100) Entonces
				Imprimir '¡Este es casi un número especial!'
			SiNo
				Imprimir 'Just a regular number'
			FinSi
		FinSi
FinAlgoritmo
---------------------------------------------------------------------------------------
MARTES 6/12/2022

****** SIMPLE CALCULATOR WITH SWITCH ********
Algoritmo SimpleCalculatorWithSwitch
	
	Imprimir "Ingrese el primer Número"
	Leer primerNumero
	Imprimir "Ingrese el segundo Número"
	Leer segundoNumero
	Imprimir "Ingrese la operación que desea realizar: +,-,*,/"
	Imprimir "Opción 1 - Suma"
	Imprimir "Opción 2 - Resta"
	Imprimir "Opción 3 - Multiplicacion"
	Imprimir "Opción 4 - Division"
	Leer opc
	
	Si opc == "1" | opc == "2" | opc == "3" | opc == "4" Entonces
	
		Segun opc Hacer
			1:
				Imprimir "Resultado: " primerNumero + segundoNumero
			2:
				Imprimir "Resultado: " primerNumero - segundoNumero
			3:
				Imprimir "Resultado: " primerNumero * segundoNumero
			4:
				Imprimir "Resultado: " primerNumero / segundoNumero
		Fin Segun 
	SiNo
		Imprimir "La operación no es válida"
	FinSi	
FinAlgoritmo

******** MULTI OPTION PROGRAM ********

Algoritmo SimpleCalculatorWithSwitch
	
	Imprimir "Ingrese el primer Número"
	Leer primerNumero
	Imprimir "Ingrese el segundo Número"
	Leer segundoNumero
	Imprimir "Ingrese la operación que desea realizar: +,-,*,/"
	Imprimir "Opción 1 - Suma"
	Imprimir "Opción 2 - Resta"
	Imprimir "Opción 3 - Multiplicacion"
	Imprimir "Opción 4 - Division"
	Leer opc
	
	Si opc == "1" | opc == "2" | opc == "3" | opc == "4" Entonces
	
		Segun opc Hacer
			1:
				Imprimir "Resultado: " primerNumero + segundoNumero
			2:
				Imprimir "Resultado: " primerNumero - segundoNumero
			3:
				Imprimir "Resultado: " primerNumero * segundoNumero
			4:
				Imprimir "Resultado: " primerNumero / segundoNumero
		Fin Segun 
	SiNo
		Imprimir "La operación no es válida"
	FinSi	
FinAlgoritmo
--------------------------------------------------------------------------------------
MIÉRCOLES 07/12/2022

******** MULTIPLICATION TABLES ********

Algoritmo MultiplicationTables
	
	Imprimir "Ingrese el número de la tabla de multiplicar que desea obtener"
	Leer num
	x=1
	
	Mientras x<=10 Hacer
		Imprimir num "*" x "=" num * x
		x= x+1
	FinMientras	
FinAlgoritmo

******** SIMPLE CALCULATOR WITH DO WHILE ********

Algoritmo DoWhileCalculator
	
	Repetir 
	Imprimir "Ingrese el primer número"
	Leer primerNumero
	Imprimir "Ingrese el segundo número"
	Leer segundoNumero
	Imprimir "Ingrese la operacion que desea realizar: +,-,*,/"
	Leer opcion

	Si opcion == "+" | opcion == "-" | opcion == "*" | opcion == "/" Entonces
		Imprimir "Procesando: " ConvertirATexto(primerNumero) + opcion + ConvertirATexto(segundoNumero)
		Si (opcion == "+") Entonces
			Imprimir "El resultado es: " primerNumero + segundoNumero
		SiNo
			Si (opcion == "-") Entonces
				Imprimir "El resultado es: " primerNumero - segundoNumero
			SiNo 
				Si (opcion == "*") Entonces
					Imprimir "El resultado es: " primerNumero * segundoNumero
				SiNo
					si (opcion =="/") Entonces
						Imprimir "El resultado es: " primerNumero / segundoNumero
					FinSi
				FinSi
			FinSi
		FinSi
		SiNo
		Imprimir "Operación no válida"
	FinSi
	Imprimir "¿Desea realizar otra operacion? si/no"
	Leer respuesta
Hasta Que !(respuesta == "si" | respuesta == "Si" )
FinAlgoritmo
-------------------------------------------------------------------------------------------------
JUEVES 08/12/2022

***** MULTIPLICATION TABLE WITH FOR *****

Algoritmo MultiplicationTableWithFor
	
	Imprimir "Ingrese el número del que desea conocer su tabla de multiplicar"
	Leer num
	Para iterador <- 0 Hasta 10 Con Paso 1 Hacer
		Imprimir num "*" iterador " = " num*iterador
	Fin Para	
FinAlgoritmo

***** ASCENDING AND DESCENDING *****

Algoritmo AscendingAndDescending
	
	Imprimir "Ingrese un número"
	Leer num	
	Imprimir "Ingrese la operación que desea realizar"
	Imprimir "Opcion1 - Orden Ascendente"
	Imprimir "Opcion2 - Orden Descendente"	
	Leer opcion
	
	Segun opcion Hacer
		1:
			Imprimir "El orden ascendente es: "
			Para iterador <-0 Hasta num Con Paso 1 Hacer
				Imprimir iterador
			Fin Para
		2:
			Imprimir "El orden descendente es: "
			Para iterador <-num Hasta 0 Con Paso -1 Hacer
				Imprimir iterador
			Fin Para		
		De Otro Modo:
			Imprimir "Opción No Válida"
	Fin Segun	
FinAlgoritmo

***** GREETINGS *****

Algoritmo Greetings
	contador <-0
	Repetir
	Imprimir "*********** Greetings *************"
	Imprimir "Ingrese que hora del día es: " 
	Leer hora	
	
	Si (hora <= 12) Entonces
		Imprimir "Buenos días!"
	SiNo
		Si (hora <= 18) Entonces
			Imprimir "Buenas Tardes!"
		SiNo
			Si (hora <= 23) Entonces
				Imprimir "Buenas Noches!"
			FinSi
		FinSi
	FinSi
	Imprimir "Desea un nuevo saludo? Si/No"
	Leer respuesta
	Si (respuesta == "si" | respuesta == "Si") Entonces
		contador <- contador +1
	FinSi
Hasta Que !(respuesta == "si" | respuesta == "Si")
Imprimir "El programa se ejecutó : " contador " " "número de veces"
	
FinAlgoritmo

