------------------------------------ WEEK04 ---------------------------------------------------

LUNES 12/12/2022

AVERAGE AND SALES
Algoritmo AverageSales
	
	Imprimir "Ingrese el número de ventas que realizó el vendedor"
	Leer num
	contador <-0
	
	Mientras contador <> num Hacer
		Imprimir "Ingrese el monto de la venta"
		Leer cantidadVenta
		totalVenta= totalVenta+cantidadVenta
		contador = contador +1		
	Fin Mientras
	promedio = totalVenta/num
	Imprimir "El Promedio de la venta es: " promedio
	
	Si (num >5) Entonces
		comision = (promedio * 15)/100
		Imprimir "El total de la comisión es : " comision
	SiNo
		si (num <=5) Entonces
			comision = (promedio *10)/100
			Imprimir "El total de la comisión es : " comision
		FinSi
	FinSi	
FinAlgoritmo

EVEN OR ODD

Algoritmo EvenOrOdd
	
	Imprimir "Ingrese un número del 1 al 50"
	Leer num	
	Si (num <1 | num>50) Entonces
		Imprimir "Error el número no está entre el 1 y el 50"
		Imprimir "Vuelva a Ingresar otro número"
		Leer num
	SiNo
		Si (num>1 ) & (num <=50 ) Entonces
			Si (num % 2 = 0) Entonces	
			
			Para contador <- 0 Hasta num Con Paso 2 Hacer				
				Imprimir "La Secuencia de números es: " contador
				contador = contador 
				 
			Fin Para
		FinSi
		Si (num % 2 = 1) Entonces			
			
			Para contador <- 1 Hasta num Con Paso 2 Hacer
				Imprimir "La Secuencia de números es: " contador
				
			Fin Para
		FinSi
	FinSi
FinSi			
FinAlgoritmo
-------------------------------------------------------------------------------------------------------------------

MARTES 13/12/2022
FULL NAME

Algoritmo FullName
	
	Imprimir "Ingrese el Nombre: "
	Leer Nombre
	Imprimir "Ingrese el Apellido: "
	Leer Apellido
	
	NombreCorrecto = Mayusculas(Subcadena(Nombre,1,1)) + Minusculas(Subcadena(Nombre,2,Longitud(Nombre)))
	ApellidoCorrecto = Mayusculas(SubCadena(Apellido,1,1)) + Minusculas(Subcadena(Apellido,2,Longitud(Apellido)))
	Imprimir "El nombre completo es : " NombreCorrecto + " " + ApellidoCorrecto	
FinAlgoritmo

THROW DICE
Algoritmo THROWDICE
	
	Para cont <-1 Hasta 10 Con Paso 1 Hacer
		azar1 = azar(6)
		azar2 = azar(6)
		//Imprimir azar1,  "   " , azar2
		si (azar1 = azar2) Entonces 
			Imprimir azar1,  "   " , azar2 "  Los Dados Son Iguales"
			//Imprimir "Los dados son iguales"
		SiNo
			Imprimir azar1,  "   " , azar2
		FinSi		
	Fin Para	
FinAlgoritmo
--------------------------------------------------------------------------------------------------------------------

MIERCOLES 14/12/2022
DISTANCE TO ZERO

Algoritmo DistanceToZero	
	Imprimir "Ingrese un número: "
	Leer distanciaMax
	
	Para i=1 Hasta 4 Con Paso 1 Hacer
		Imprimir "Ingrese un Número: "
		Leer num
		
		Si (abs(num) > abs(distanciaMax)) Entonces
			distanciaMax = num				
		FinSi
	Fin Para
	Imprimir trunc(distanciaMax)		
FinAlgoritmo

TOSS COIN

Algoritmo TossCoin	
	Imprimir "Ingrese el nombre del primer jugador: "
	Leer jugador1
	Imprimir "Ingrese el Monto a jugar: "
	Leer monto1
	Imprimir "Ingrese el nombre del segundo jugador: "
	Leer jugador2
	Imprimir "Ingrese el Monto a jugar: "
	Leer monto2	
	
	moneda = aleatorio(1,2)
	Si (monto1 <=0) & (monto2 <=0) Entonces		
		Imprimir "Juego Cancelado"	
	SiNo		
		Si (monto1 <=0) Entonces
		Imprimir Mayusculas(jugador2) "   Ganó"
	SiNo
		Si (monto2 <=0) Entonces
			Imprimir Mayusculas(jugador1) "  Ganó"		
	SiNo		
		Si (moneda = 1) Entonces
			Imprimir Mayusculas(jugador1) "   Ganó"
	SiNo
		Si (moneda = 2) Entonces
			Imprimir Mayusculas(jugador2) "  Ganó"
					FinSi
				FinSi
			FinSi
		FinSi
	FinSi	
FinAlgoritmo
-----------------------------------------------------------------------------------------------------------

JUEVES 15/12/2022
TOTAL PRICE

Funcion value <- precioTotal (precio, iva)
	
	SI precio > 3000 Entonces
		
		precioiva = (precio + ((precio*iva)/100)) 
		descuento = (precioiva *10)/100
		value = precioiva - descuento
	SiNo
		value = (precio + ((precio*iva)/100))
	FinSi
Fin Funcion

Algoritmo ejemploPrecioTotal
	Imprimir precioTotal(5000,21)
FinAlgoritmo

REVERSE DIRECTION AND SIZE
Funcion value2 <- ReverseDirectionAndSize ( texto )
	Imprimir "Ingrese un texto: "
	Leer texto
	//Para i<-1 Hasta Longitud(texto) Con Paso 1 Hacer
		//nuevoTexto = SubCadena(texto,i,i)
	//Fin Para
	//value2 = Concatenar(value2,value)
	Para i= Longitud(texto) Hasta 1 Con Paso -1 Hacer
		caracter = SubCadena(texto,i,i)
		Si (caracter >= "a" & caracter < "z") Entonces
			value = Mayusculas(caracter)
		SiNo
			value = Minusculas(caracter)
		FinSi
		
		value2 = value2 + value
	Fin Para
Fin Funcion

Algoritmo EjemploReverseDirectionAndSize
	Imprimir ReverseDirectionAndSize(texto)
	
FinAlgoritmo
