# LOGIC PROBLEM
## NOVEMBER 28TH 

The teacher asks his 5 students if they studied mathematics yesterday.

Alice: "Nobody studied math yesterday".
Bob: "1 person studied math yesterday".
Charlie: "2 people studied math yesterday".
Dan: "3 people studied mathematics yesterday".
Eva: "4 people studied mathematics yesterday".

The teacher knows that only those who studied would be telling the truth and those who didn't would be lying. Who is telling the truth?

### SOLUTION

```
Bob is telling the truth, because he can say that he study math yesterday without know if the rest of the people study or not.
``` 
------------------

# CEREAL OR MILK

Create an algorithm to prepare a bowl of cereal with milk. Represent the result in pseudocode and in a flowchart.

1. Grab a bowl
2. Add cereal
3. Ask if wants something more:
  3.1 add fruit (banana/strawberries) 
  3.2 Add granola
4. Add milk
5. Enjoy

![CEREAL](https://user-images.githubusercontent.com/119624165/205734739-a29fc2a1-9462-46f1-86f8-56eb13c9a5a8.PNG)

---------------------
# PRINT MY NAME

## NOVEMBER 29TH

The pseudocode of the algorithm is the following:

```
-Algorithm: myname
   - Imprimir 'Henry González'
-Algorithm end
```

![MY NAME](https://user-images.githubusercontent.com/119624165/205738671-59876b4a-7b42-4096-9197-7057d59836e5.PNG)
-----------------------
# PRINT MY NAME & AGE

The pseudocode of the algorithm is the following:

```
-Algorithm: myname
    -Imprimir 'Henry González'
   - Imprimir '24'
-Algorithm end
```

![my name and age](https://user-images.githubusercontent.com/119624165/205738701-85799afd-8ff1-45a1-aed3-f97d875a186f.PNG)
-------------------------
# SQUIRREL GAME

## NOVEMBER 30

![SQUIRREL](https://user-images.githubusercontent.com/119624165/205783518-d858ea55-d128-4bc8-8aca-629a6b9b36f8.PNG)

--------------------------

# MOD

The challenge for you now is to create a PSeInt program that will receive a number from the user and add the mod operator using the even/odd case ( X % 2 ) where X is the user input

```
    Algoritmo odd/even
        Leer X
        Imprimir X % 2
     Fin Algoritmo
 ```    
     
![PAR](https://user-images.githubusercontent.com/119624165/205784989-dbfc72dc-1dfb-4130-a191-4e7e278136b1.PNG)

![IMPAR](https://user-images.githubusercontent.com/119624165/205785005-a4494214-9828-495f-aa98-e6bb7379a68b.PNG)

----------------------------------

# REGISTER FORM

```
Algoritmo REGISTER 
	Imprimir '====== USER FORM ======'
	Imprimir 'First Name' 
	Leer firstName
	imprimir 'Last Name'
	Leer lastName
	Imprimir 'age'
	Leer age
	Imprimir 'email'
	Leer email
	Imprimir 'address'
	Leer address
	Imprimir '====== USER DATA =======' 
	Imprimir 'Full name: ' + FirstName +'' + LastName
	imprimir 'Age: ' + age
	imprimir 'Email: ' + Email
	Imprimir 'adress: ' + address
	Imprimir '==========================='
FinAlgoritmo
```

![REGISTER](https://user-images.githubusercontent.com/119624165/205786513-e9834ff3-ff20-4739-b0b5-af024da4f343.PNG)

----------------------------------

# TRUTH TABLES 

## DECEMBER 1ST

You are going to learn about three main logical operations used in programming, these operations are called AND, OR, and NOT. Each of the operations uses booleans as operands, and when applying the operations a result is generated, which is also a boolean, this is easier to check using the Truth Tables for each of the operations, now your task is for you to learn, and add the Truth Tables for each of the operations add them to your README and check if the following operations are correct by answering ✅ or ❌ at the end of each operation

|Operation | Answer|
|----------|-------|
| T `&` T = T | ✅ |
| T `&` F = F | ✅ |
| F `&` T = T | ❌ |
| F `&` F = F | ✅ |
| T `OR` T = T | ✅ |
| T `OR` F = F | ❌ |
| F `OR` T = T | ✅ |
| F `OR` F = F | ✅ |
| `~`T = T | ❌ |
| `~`F = T | ✅ |
| (T `&` F) `OR` (`~`F) = T | ✅ |
| (T `OR` F ) `&` (F `OR` F) = T | ❌ |
| `~`((T `OR` F ) `&` (F `OR` F)) `&` F = T | ❌ |
| `~`((T `OR` F ) `&` (F `OR` F)) `&` T = F | ❌ |

----------------------------------------------

# BOOLEAN RESULTS

You have been assigned to verify and explain a code created by one of your colleagues, the idea is that you can describe the value that each variable has within the code as well as what was done for each line. What is expected of you is that you add comments below each line showing the value that the variable would have and a short explanation of how that value is reached.

```
Algoritmo Boolean
	a <- 5 == 3
	// FALSE, Because 5 is not the same with 3
	b <- 4 <> 3
	// True, Because 4 and 3 are different
	c <- 7 > 7
	// False, Because we are comparing the same number, no one can be mayor
	d <- 4 < 4
	// False, Because we are comparing the same number, no one can be mayor
	e <- 100 <= 90
	// FALSE, Because 90 is minor than 100, also it's not the same
	f <- 40 >= 40 
	// TRUE, Because we are comparing the same number
FinAlgoritmo
 
 ```

-----------------------------------

# Identify odd and even numbers

Remember the last challenge about the Mod operator? well, today your task will be to create a program that will be able to detect based on the user input if the number is odd or even. The process should be the following:

The user enters a number
Your algorithm detects if the number is odd or even (remember to use conditional statements Si...Entonces)
Print ‘Número: x es par’ if the number is even (x is the number the user enters)
Print ‘Número: x es impar’ if the number is odd (x is the number the user enters)

```
Algoritmo DetectEvenOdd
	imprimir 'Enter number to verify'
    Leer X
	Si x % 2 == 0 Entonces
		Imprimir 'Number: ' + ConvertirATexto(X) + ' is even'
	SiNo
		Imprimir 'Number: ' + ConvertirATexto(X) + ' is odd'
	FinSi
FinAlgoritmo

```
![EVEN](https://user-images.githubusercontent.com/119624165/205800738-9d1878c6-0b54-4874-94e0-5ccc7cb74449.PNG)

--![ODD](https://user-images.githubusercontent.com/119624165/205800754-727cd521-d8b6-4ad3-aba4-cf2353bf992d.PNG)

----------------------------------------

