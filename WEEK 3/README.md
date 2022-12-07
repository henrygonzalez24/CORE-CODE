# Simple calculator

## December 5th

For this challenge you will be performing a simple calculator, this calculator can perform the following operations:

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

-----------------------
