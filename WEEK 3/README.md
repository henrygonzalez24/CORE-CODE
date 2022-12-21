# Simple calculator

## December 5th

For this challenge you will be performing a simple calculator, this calculator can perform the following operations:

Sum (+)
Subtract (-)
Multiplication (*)
Division (/)

```python
Algoritmo simpleCal
	Imprimir ' =========SIMPLE CALCULATOR========'
	Imprimir 'Ingrese primer numero'
	leer n1
	Imprimir 'Ingrese segundo numero'
	leer n2
	Imprimir 'Ingrese operación +,-,*,/'
	leer op
	Si op == '+' | op == '-' | op == '*' | op == '/' Entonces
		Imprimir ' Procesando ' + ConvertirATexto(n1) + ' ' + op + ' ' + ConvertirATexto(n2)
		Si op == '+' Entonces
			imprimir ' Resultado :' + ConvertirATexto( n1 + n2 )
		sino 
			Si op == '-' Entonces
				imprimir 'Resultado :' + ConvertirATexto( n1 - n2 )
			SiNo
				si op == '*' Entonces
					Imprimir 'Resultado :' + ConvertirATexto( n1 * n2)
				SiNo
					Imprimir 'Resultado :' + ConvertirATexto( n1 / n2)
				FinSi
			FinSi
		FinSi
	Sino 
		Imprimir 'Operación no valida'
	FinSi
FinAlgoritmo


```
SIMPLE CALCULATOR

![SIMPLE](https://user-images.githubusercontent.com/119624165/206333241-58d99612-1795-4744-a0f4-e633772c0cab.PNG)

-----------------------

# SPECIAL NUMBER

You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number". Another developer was trying to program the logic, but apparently couldn't, you need to fix the code to work properly

This was the code from the developer
```python
Algoritmo specialNumber
	Leer n
	Si n == 100 Entonces
		Imprimir 'This is a special number'
	FinSi
	Si n < 1000 Entonces
		Imprimir ''
	SiNo
		Imprimir 'Just a regular number'
	FinSi
	Si n % 10 == 0 Entonces
		Imprimir 'This number is multiple of 10'
	FinSi
FinAlgoritmo
```

#### SOLUTION

```python
Algoritmo specialnumber
	Leer n
	Si n == 100 Entonces
		Imprimir ' This is a special number'
	SiNo
		Si ( n < 1000) & ( n % 10 == 0) Entonces
			imprimir 'this number is almost special'
		SiNo
			Imprimir 'Just a regular number'
		FinSi
	FinSi
FinAlgoritmo
```
##### SPECIAL NUMBER
![SPECIAL](https://user-images.githubusercontent.com/119624165/206324194-f9f778b3-3666-4ce2-a077-e7b24f5be237.PNG)

##### ALMOST SPECIAL
![ALMOST](https://user-images.githubusercontent.com/119624165/206324251-baff0c0e-1a8c-4f64-80c7-2c3adaed4e30.PNG)

##### REGULAR NUMBER
![REGULAR NUMBER](https://user-images.githubusercontent.com/119624165/206324295-8d04a9fe-f284-46a5-830b-34684b1633e4.PNG)

-------------------------------------------
# SIMPLE CALCULATOR WITH SWITCH

## December 6th

For this challenge you will be performing a simple calculator using Switch (Segun), this calculator can perform the following operations:

Sum (+)
Subtract (-)
Multiplication (*)
Division (/)

Sum (+)
Subtract (-)
Multiplication (*)
Division (/)

```python
Algoritmo simplecalc
	Imprimir '=======Simple Calculator======='
	Imprimir 'Ingrese primer numero'
	Leer n1
	Imprimir 'Ingrese segundo numero'
	Leer n2
	Imprimir 'Ingrese operación: +,-,*,/'
	Leer op
	Imprimir 'Procesando: ' + ConvertirATexto(n1) + ' ' + op + ConvertirATexto(n2)
	Segun op Hacer
		"+" :
			Imprimir "SUMAR" 
			imprimir 'resultado ' + ConvertirATexto(n1 + n2)
		"-" :
			Imprimir "RESTAR" 
			imprimir 'resultado ' + ConvertirATexto(n1 - n2)
		"*" :
			Imprimir "MULTIPLICAR" 
			imprimir 'resultado ' + ConvertirATexto(n1 * n2)
		"/" :
			Imprimir "DIVISION"
			si n2 == 0 Entonces
				imprimir 'No definido'
			SiNo
				imprimir 'resultado ' + ConvertirATexto(n1 / n2)
			FinSi
		De Otro Modo:
			imprimir 'Operación no definida'
	FinSegun
FinAlgoritmo

```
SIMPLE CALCULATOR

![SIMPLE CALCULATOR](https://user-images.githubusercontent.com/119624165/206322168-d5115f47-0c52-4c34-93e2-c8adf4914f20.PNG)

FAIL OPERATION

![OPERACION NO VALIDA](https://user-images.githubusercontent.com/119624165/206322435-b2dbaa25-8464-4a4c-a4a3-ab5ea703c58b.PNG)

---------------------------

# Multi Option Program

```python
Algoritmo Multipleopcion
	Imprimir '1.Sumar dos numeros'
	Imprimir '2.mostrar dia de la semana'
	Imprimir '3.calcular longitud de texto'
	Imprimir 'Ingrese la opción seleccionada: '
	Leer R
	Segun R Hacer 
		"1" : 
			Imprimir '1. Suma de dos numeros'
			Imprimir 'Ingrese primer numero'
			Leer n1
			Imprimir 'Ingrese segundo numero'
			Leer n2
			Imprimir 'Resultado :' + ConvertirATexto(n1 + n2)
		"2" :
			imprimir '2. Mostrar día de la semana'
			Imprimir 'Ingrese dia de la semana (1-7)'
			Leer n3
			Segun n3 Hacer
				"1" : 
					Imprimir 'lunes'
				"2" : 
					Imprimir 'Martes'
				"3" :
					Imprimir 'miercoles '
				"4" :
					Imprimir 'Jueves'
				"5" :
					Imprimir 'Viernes'
				"6" :
					Imprimir 'Sabado'
				"7" :
					Imprimir 'Domingo'
				De Otro Modo:
					Imprimir 'dia incorrecto'
			FinSegun
		"3" :
			Imprimir '3. Calcular Longitud de texto ' 
			Imprimir 'Ingrese texto'
			Leer cadena
			Imprimir 'Resultado :' + ConvertirATexto(Longitud(cadena))
		De Otro Modo: 
			Imprimir'Opción incorrecta'
	FinSegun
FinAlgoritmo
```

OPTION 1
![OPTION 1](https://user-images.githubusercontent.com/119624165/206336138-fa8f8003-6629-4bf9-8169-9a0c8b09a375.PNG)

OPTION 2
![OPTION 2](https://user-images.githubusercontent.com/119624165/206336177-407e9e8b-e0de-4515-a44a-7989f104cb9e.PNG)

OPTION 3
![OPTION 3](https://user-images.githubusercontent.com/119624165/206336232-43f42996-01de-4e85-8b24-69715bf003b4.PNG)

INCORRECT OPTION
![INCORRECT OPTION](https://user-images.githubusercontent.com/119624165/206336429-05151c0e-a1cc-43c2-8435-eddc2571ccde.PNG)

-----------------------------------

# Multiplicacion tables

 ## December 7th
 
For this challenge you will create a program to calculate the multiplication tables for a given number using While (Mientras). The user must enter a number and then the multiplication table for the number must be printed.

```python
Algoritmo sin_titulo
	Imprimir '========= TABLA DE MULTIPLICAR ============'
	Imprimir 'Ingrese la tabla para calcular'
	Leer tabla 
	Imprimir '@ Tabla de ' + ConvertirATexto(tabla) + ' @ '
	iterador <- 1
	mientras iterador <= 10 Hacer
		imprimir ConvertirATexto(tabla) + ' * ' + ConvertirATexto(iterador) + ' = ' + ConvertirATexto(tabla * iterador)
		iterador <- iterador + 1
	FinMientras
FinAlgoritmo

```

![MULTIPL](https://user-images.githubusercontent.com/119624165/207413325-e8146d66-c754-4a74-9be9-76b197b0dd31.PNG)

---------------------------------------
 # Simple calculator with Do While
 
 ```python
 Algoritmo simpleCalswitch
	Imprimir ' =========SIMPLE CALCULATOR========'
	Repetir
		Imprimir 'Ingrese primer numero'
		leer n1
		Imprimir 'Ingrese segundo numero'
		leer n2
		Imprimir 'Ingrese operación +,-,*,/'
		leer op
		Si op == '+' | op == '-' | op == '*' | op == '/' Entonces
			Imprimir ' Procesando ' + ConvertirATexto(n1) + ' ' + op + ' ' + ConvertirATexto(n2)
			Si op == '+' Entonces
				imprimir ' Resultado :' + ConvertirATexto( n1 + n2 )
			sino 
				Si op == '-' Entonces
					imprimir 'Resultado :' + ConvertirATexto( n1 - n2 )
				SiNo
					si op == '*' Entonces
						Imprimir 'Resultado :' + ConvertirATexto( n1 * n2)
					SiNo
						Imprimir 'Resultado :' + ConvertirATexto( n1 / n2)
					FinSi
				FinSi
			FinSi
		Sino 
			Imprimir 'Operación no valida'
		FinSi
	
		Imprimir 'Desea continuar? Si / No'
		Leer continuar 
	Hasta Que continuar == 'no' | continuar == 'No'
FinAlgoritmo
```
![DO WHILE](https://user-images.githubusercontent.com/119624165/206342303-fe993c41-68c4-49e5-abde-0d76053c87d7.PNG)

---------------------------
# Multiplication Tables with For

## DECEMBER 8TH

For this challenge you will create a program to calculate the multiplication tables for a given number using the For(Para) loop.

```python
Algoritmo MultiplicarPara
	Imprimir '========= TABLA DE MULTIPLICAR ============'
	Imprimir 'Ingrese la tabla para calcular'
	Leer tabla 
	Imprimir '@ Tabla de ' + ConvertirATexto(tabla) + ' @ '
	Para iterador <- 1 Hasta 10 Con Paso 1 Hacer
		Imprimir ConvertirATexto(tabla) + ' * ' + ConvertirATexto(iterador) + ' = ' + ConvertirATexto(tabla * iterador)
	FinPara
FinAlgoritmo
```


![calcu 2](https://user-images.githubusercontent.com/119624165/207485715-5f521914-3923-47c1-af6e-34c317e3c3bb.PNG)

--------------------------

# Ascending and Descending Numbers

For this challenge we are going to print numbers in ascending or descending order. The user must enter a number, then he must enter if he wants to print the numbers in ascending or descending order. If the user chooses ascending, the numbers will be printed from the number 0 to the number entered, otherwise the numbers will be printed descending from the number entered to the number 0.To solve this challenge remember to use the For(Para) loop.

```python
Algoritmo AscendAndDescen
	Imprimir '===Ascending and Descending numbers==='
	Imprimir 'Ingrese numero'
	Leer num
	Imprimir 'Opciones disponibles'
	imprimir 'Imprimir en orden ascendente'
	Imprimir 'Imprimir en orden descendente'
	Imprimir 'Ingrese opción elegida'
	leer op
	Segun op Hacer
		1:
			Para i <- 1 Hasta num con paso 1 hacer
				imprimir i
			Fin Para
		2:
			Para i <- num Hasta 0 con paso -1 hacer
				imprimir i
			Fin Para
		De Otro Modo:
			imprimir 'Opción no valida'
	Fin Segun
FinAlgoritmo
```



![ASCENDIENTES](https://user-images.githubusercontent.com/119624165/207670055-654000fe-63c7-4189-a61e-998141247d87.PNG)



--------------------------
# GREETINGS

For this challenge, you need to create a program that prints a greeting based on an hour entered. The program should do the following:

Print Buenos dias! if the hour is from 0 to 12
Print Buenas tardes! if the hour is from 13 to 18
Print Buenas noches! if the hour is from 19 to 23
Ask the user if he wants to perform another greeting. If the answer is Si, the program must start again.
At the end of the program, print out the number of times the program has greeted.



```python
Algoritmo Greetings
	Imprimir '======= Greetings ======='
	Definir continuar Como Cadena
	Definir contador Como Entero
	contador <- 0
	continuar <- 'Si'
	Mientras continuar == 'Si' Hacer
		Imprimir 'Ingrese la hora actual (0-23):'
		Leer hora
		Si hora <= 12 Entonces
			Imprimir 'Buenas dias!'
		SiNo 
			Si hora <= 18 Entonces
				Imprimir 'Buenas tardes!'
			SiNo
				Imprimir 'Buenas noches!'
			Fin Si
		Fin Si
		
		contador <- contador + 1
		
		Imprimir 'Desea continuar ? Si/No'
		Leer continuar
	Fin Mientras
	
	Imprimir 'Cantidad de Saludos realizados: ' + ConvertirATexto(contador)
FinAlgoritmo
```

![GREETINGS](https://user-images.githubusercontent.com/119624165/207448289-fd02229d-110d-45fc-915b-d63fb5dabed8.PNG)

----------------------------------------

