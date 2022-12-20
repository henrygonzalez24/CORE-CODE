# TIME CONVERTER

## DECEMBER 19TH

```
Funcion result <- timeConverter (number)
	Definir result Como Caracter;
	Definir days, hours, minutes, seconds Como Entero;
	seconds = number % 60;
	minutes = Trunc(number/60) % 60;
	hours = Trunc(number/3600) % 24;
	days = Trunc(number/86400);
	result = Concatenar('days: ', ConvertirATexto(days));
	result = Concatenar(result, ', hours: ');
	result = Concatenar(result, ConvertirATexto(hours));
	result = Concatenar(result, ', minutes: ');
	result = Concatenar(result, ConvertirATexto(minutes));
	result = Concatenar(result, ', and seconds: ');
	result = Concatenar(result, ConvertirATexto(seconds));
Fin Funcion

Algoritmo Timeconverterexercise
	Imprimir timeConverter(150000)
FinAlgoritmo
```

![TIME](https://user-images.githubusercontent.com/119624165/208787110-192dcd66-fe68-4351-b447-a1eacac81a4d.PNG)

----------------------------------------------

# COMPARE DISTANCES

Create a function called compareDistances that asks for 5 numbers, these can be positive or negative, add the positives with positives and negatives with negatives, the function should return true if there is more distance to 0 with positives or false if the distance is greater with negatives .

```
Funcion result <- compareDistances ()
	Definir result Como Logico;
	Definir negativeNumber, positiveNumber Como Real;
	negativeNumber = 0;
	positiveNumber = 0;
	Para count=1 Hasta 5 Con Paso 1 Hacer
		Escribir "write a number"
		leer num
		SI num > 0 Entonces
			positiveNumber = positiveNumber + num;
		SiNo
			negativeNumber = negativeNumber + num;
		FinSi
	FinPara
	result = positiveNumber > Abs(negativeNumber)
Fin Funcion

Algoritmo CompareDistancesExercise
	Imprimir compareDistances()
FinAlgoritmo
```


