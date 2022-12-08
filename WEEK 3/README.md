# Simple calculator

## December 5th

For this challenge you will be performing a simple calculator, this calculator can perform the following operations:

Sum (+)
Subtract (-)
Multiplication (*)
Division (/)

```
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
```
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

```
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
# SIMPLE CALCULATOR WITH SWITH

For this challenge you will be performing a simple calculator using Switch (Segun), this calculator can perform the following operations:

Sum (+)
Subtract (-)
Multiplication (*)
Division (/)

Sum (+)
Subtract (-)
Multiplication (*)
Division (/)

```
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
