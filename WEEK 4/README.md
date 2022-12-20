# AVERAGE SALES AND COMISSIONS

## DECEMBER 12TH 

Make a program that asks how many sales the seller had, Once the number of sales is entered, ask for the value of each sale until all are entered, then return as a result the average value of sales, and the commission that the seller will take, If the seller had more than 5 sales, his commission will be 15% of the total value of the sales, if he sold 5 or less, his commission will be only 10%.

```
Algoritmo averageSalesAndCommission
	Escribir "Write the total number of sales to enter:"
	leer amountofsales
	totalrevenue = 0
	
	Para sale = 1 Hasta amountofsales Con Paso 1 Hacer
		Escribir "Write the value of the sale number: ",sale
		leer amount
		totalrevenue = totalrevenue + amount
	FinPara
	
	average = totalrevenue / amountofsales 
	Imprimir 'The average sales is: ', average
	
	SI amountofsales < 5 Entonces
		Imprimir 'The commission received by the seller is: ', totalrevenue * 0.10
	SiNo
		Imprimir 'The commission received by the seller is: ', totalrevenue * 0.15
	FinSi
	
FinAlgoritmo
```

![AVERAGE](https://user-images.githubusercontent.com/119624165/208527831-32cbf52d-4f42-48c5-bf85-0776381c4cfd.PNG)

---------------------------------

# Even or odd

Request a number from 1 to 50, if the number is not between those values, report the error and request it again until you get a valid number, then it shows on the screen all the numbers from 1 to that number, if the number is even it only shows the even numbers, if it is odd it only shows the odd ones.

```
Algoritmo evenOrOdd
	repetir
		imprimir 'write a number between 1 and 50: '
		leer number
		si number < 1 | number > 50 Entonces
			imprimir 'invalid number'
		FinSi
	
	Mientras Que number < 1  | number > 50
	
	par = number % 2 = 0
	para co = 1 Hasta number Con Paso 1 hacer 
		si co % 2 = 0 & par Entonces
			imprimir co
		SiNo
			si co % 2 = 1 & ~(par) Entonces
				imprimir co
			FinSi
	FinSi
	
FinPara

FinAlgoritmo
```

![EVEN AND OD](https://user-images.githubusercontent.com/119624165/208528108-9557e739-07cc-4cb9-a4ac-18b860cdcbb5.PNG)

-------------------------------

# FULL NAME

## DECEMBER 13TH

Make a program that takes a first name and a last name, then returns a string with both values ​​with the first letter uppercase and the rest lowercase.

```
Algoritmo MAYUS
	Imprimir 'Write your first name : '
	Leer name
	Imprimir 'Write your last name : '
	leer last
	correctname = Mayusculas(SubCadena(name,0,0)) + Minusculas(SubCadena(name,1,Longitud(name)-1))
	correctlast= Mayusculas(SubCadena(last,0,0)) + Minusculas(SubCadena(last,1,Longitud(last)-1))
	imprimir correctname , ' ', correctlast
FinAlgoritmo
```


![NAME](https://user-images.githubusercontent.com/119624165/208530407-a77b71ed-6763-4759-bf7d-7e4c563cdf3b.PNG)

-------------------------------------

# Throw dice

make a program that simulates the roll of 2 dice 10 times, and display for each roll the values ​​of the two dice separated by a space, in case the 2 dice throw the same value in addition to the result, add a string to the ending that says "the dice are the same".

```
Algoritmo AZARGAME
	imprimir 'THROW DICE'
	definir dice1, dice2 Como entero
	para count = 1 hasta 10 con paso 1 Hacer
		dice1 = aleatorio (1,6)
		dice2 = aleatorio (1,6)
		si dice1 = dice2 entonces
			Imprimir dice1, ' ' , dice2, 'are the same'
		SiNo
			imprimir dice1, ' ', dice2
		FinSi
	FinPara
FinAlgoritmo
```

![DICE](https://user-images.githubusercontent.com/119624165/208532133-927f6224-1dd9-4666-b459-a4ca8d8660c9.PNG)

-------------------------

# DISTANCE TO 0

### DECEMBER 14TH

Make a program that asks for 5 values ​​and also allows us to know which one is furthest from zero, once obtained it returns that number (the numbers can be negative), showing only the integer part of the number.

Expected output

```
Algoritmo ZeroNumber
	Escribir 'Write a number'
	leer distanceM
	Para count = 1 hasta 4 Con Paso 1 Hacer
		escribir 'Write a number'
		leer number
		si abs(number) > abs(distanceM) Entonces
			distanceM = number
		FinSi
	FinPara
	imprimir trunc(distanceM)
FinAlgoritmo
```

![MAX DISTANCE](https://user-images.githubusercontent.com/119624165/208537675-5c3d51d5-c33a-4c45-93d2-4a2088ac5ab2.PNG)

-------------------------------

# TOSS COIN

From the data we receive first a name and a value, then another name and another value, using the built-in function aleatorio() we simulate the flip of a coin, We must return the name of the winner in capital letters and the value I win, to avoid cheating, if a player puts a value of zero or negative, the opponent automatically wins, in case both cheat, "game canceled" is returned.

```
Algoritmo tosscoin
	escribir 'Enter the name of the first player :'
	leer name1
	Escribir 'Enter the amount to play: '
	leer amount1
	escribir 'Enter the name of the first player :'
	leer name2
	Escribir 'Enter the amount to play: '
	leer amount2
	
	si amount1 <= 0 | amount2 <= 0 Entonces
		si amount1 <= 0 | amount2 <= 0 Entonces
			imprimir 'Game canceled'
		SiNo
			si amount1 <= 0 Entonces
				imprimir 'Player wins: ', ' ', Mayusculas(name1), 'amount won: 0'
			SiNo
				imprimir 'Player wins: ', ' ', Mayusculas(name2), 'amount won: 0'
			FinSi
		FinSi
	SiNo
		si aleatorio(1,2) = 1 Entonces
			imprimir 'Player wins: ', ' ', Mayusculas(name1), 'amount won:' , amount1
		SiNo
			imprimir 'Player wins: ', ' ', Mayusculas(name2), ' ', 'amount won:' , amount2
		FinSi
	FinSi
FinAlgoritmo
```
![TOSS COIN](https://user-images.githubusercontent.com/119624165/208539444-84c8ada7-bd83-471a-b710-8aacd59ca5c9.PNG)

------------------------------------

# TOTAL PRICE

# DECEMBER 15TH

Create a function called TotalPrice that takes 2 parameters, price and VAT, and returns the price including VAT. if the price exceeds 3000 a 10 percent discount is made on the total price.

```
Funcion value <- TotalPrice (price, iva)
	Definir value Como Real;
	SI price > 3000 Entonces
		value = ( price + (price/100*iva) ) / 100*90
	SiNo
		value = ( price + (price/100*iva) )
	FinSi
Fin Funcion

Algoritmo tottalpriceExercise
	Imprimir TotalPrice(6000,12)
FinAlgoritmo
```

![TOTALPRICE](https://user-images.githubusercontent.com/119624165/208565643-5446b67a-6c87-4a08-b27f-0dd2158faaca.PNG)

--------------------------------------

#REVERSE DIRECTION AND SIZE

Create a function called ReverseDirectionAndSize that takes some text as a parameter and reverses it, eg: "Hello" -> "olleH" and also reverses the letters if they are uppercase to lowercase and if they are lowercase to uppercase

```
Funcion result <- ReverseDirectionAndSize (string)
	Definir result Como Caracter;
	result = "";
	Para count = Longitud(string) Hasta 0 Con Paso -1 Hacer
		letter = Subcadena(string,count,count);
		SI letter = Mayusculas(letter) Entonces
			letter = Minusculas(letter)
		SiNo
			letter = Mayusculas(letter)
		FinSi
		result = Concatenar(result, letter)
	FinPara
Fin Funcion

Algoritmo example_ReverseDirectionAndSize
	leer text
	Imprimir ReverseDirectionAndSize(text)
FinAlgoritmo
```

![REVERSE](https://user-images.githubusercontent.com/119624165/208567929-27bcfe5d-51b1-4cb5-883c-6331df0db1e6.PNG)

---------------------------------------
