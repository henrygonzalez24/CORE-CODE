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
