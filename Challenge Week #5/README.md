# CHALLENGES FROM WEEK # 4 

## Index
- ### Week challenges (Monday)
    - [1. Time Converter](#1-time-converter)
    - [2. Compare distances](#2-compare-distances)
- ### Week challenges (Tuesday)
    - [1. Sum of pairs](#1-sum-of-pairs)
    - [2. Mid point](#2-mid-point)
- ### Week challenges (Wednesday)
    - [1. Cashier](#1-cashier)
    - [2. Weather average](#2-weather-average)
- ### Week challenges (Thursday)
    - [1. if]()
    - [2. While]()
    - [2. For]()

#
#

## CHALLENGES (MONDAY)

### 1. Time Converter
- Solution
```javascript
Funcion resultado <- timeConverter(segundos)
	Definir dias, horas, minutos, segundosRestantes Como Entero;
	Definir resultado Como caracter;
	
	dias = trunc(segundos/(24 * 60 * 60))
	horas = trunc(segundos/(60 * 60))%24
	minutos = trunc(segundos/60)%60
	segundosRestantes = trunc(segundos % 60)
	
	resultado = Concatenar('dias: ', ConvertirATexto(dias));
	resultado = Concatenar(resultado, ', horas: ');
	resultado = Concatenar(resultado, ConvertirATexto(horas));
	resultado = Concatenar(resultado, ', minutos: ');
	resultado = Concatenar(resultado, ConvertirATexto(minutos));
	resultado = Concatenar(resultado, ', y segundos: ');
	resultado = Concatenar(resultado, ConvertirATexto(segundosRestantes));
FinFuncion

Algoritmo exampleTimeConverter
	Imprimir timeConverter(4000)
	Imprimir timeConverter(8000)
	Imprimir timeConverter(5000)
FinAlgoritmo
```
- Run Program

![Image](/Challenge%20Week%20%235/Images/4070-PSeInt_-_Ejecutando_proceso_EXAMPLETIMECONVERTER.png)

### 2. Compare Distances
- Solution
```javascript
Funcion result <- compareDistances()
	Definir result Como Logico;
	Definir NegativeNumber, PositiveNumber Como Real;
	NegativeNumber = 0;
	PositiveNumber = 0; 
	
	Para count = 1 hasta 5 Con Paso 1 hacer 
		Escribir "write a number";
		leer number;
		
		Si number > 0 Entonces
			PositiveNumber = PositiveNumber + number;
		SiNo
			NegativeNumber = NegativeNumber + number; 
			
		FinSi
		
		result = PositiveNumber > abs(NegativeNumber) 
		
	FinPara
FinFuncion

Algoritmo exampleCompareDistances
    Imprimir CompareDistances()
FinAlgoritmo
```
- Run Program
    - True 

![Image](/Challenge%20Week%20%235/Images/4071-PSeInt_-_Ejecutando_proceso_EXAMPLECOMPAREDISTANCE.png)

   - False

![Image](/Challenge%20Week%20%235/Images/4073-PSeInt_-_Ejecutando_proceso_EXAMPLECOMPAREDISTANCE.png)

#
#

## CHALLENGES (TUESDAY)

### 1. Sum of Pairs

- Solution
```javascript
Funcion result <- sumOfPair()
	Definir result, suma Como real;
	
	suma = 0;
	Repetir 
		Escribir "Enter a number between 1 and 100";
		leer number;
		si number < 1 | number >100 Entonces
			Imprimir "Number is out range"
		SiNo
			si number % 2 = 0 Entonces
				suma = suma + number;
			FinSi
		FinSi
		
		result = suma 
		
	Mientras Que number>=1 & number <= 100 
	
	
FinFuncion

Algoritmo ExampleSumofPairs
	Imprimir sumOfPair()
FinAlgoritmo
```
- Run Program

![Image](/Challenge%20Week%20%235/Images/4074-PSeInt_-_Ejecutando_proceso_EXAMPLESUMOFPAIRS.png)

#

### 2. Mid point

- Solution
```javascript
Funcion result <- midPoint (num1,num2)
	si num1 > 0 Entonces
		si num2>0 Entonces
			si num1>num2 Entonces
				result = num2 + ((num1 - num2) /2);
			SiNo
				result = num1 + ((num2 - num1) /2);
			FinSi
		SiNo
			result = num1 - ((num1 + abs(num2))/2)
			
		FinSi
	SiNo
		si num2>0 Entonces
			result = num1 + ((num2 + abs(num1))/2)
		SiNo
			si abs(num1) > abs(num2) Entonces
				result = num1 + ((abs(num1) - abs(num2)) /2);
			SiNo
				result = num2 + ((abs(num2) - abs(num1)) /2);
			FinSi
		FinSi
		
	FinSi
FinFuncion

Algoritmo exampleMidpPoint
	Imprimir midPoint(40,80)
	Imprimir midPoint(40,-80)
	Imprimir midPoint(50,50)
	Imprimir midPoint(-50,50)
FinAlgoritmo
```
- Run Program

![Image](/Challenge%20Week%20%235/Images/4075-PSeInt_-_Ejecutando_proceso_EXAMPLEMIDPPOINT.png)

#
#

## CHALLENGES (WEDENESDAY)

### 1. Cashier

- Solution

```javascript
Funcion balance <- cashier()
	Definir balance como Real
	balance = 1000 
	Repetir 
		Imprimir "Choose an option ";
		Imprimir "A. make a deposit ";
		Imprimir "B. Make a withdraw.";
		Imprimir "C. Exit the program";
		leer option;
		si option = "a" Entonces
			balance = balance + deposit()
		
			
		FinSi
		
		si option = "b" Entonces
			balance = balance - Withdraw()
		FinSi
		
	Mientras Que option = 'a' | option = 'b'
	
FinFuncion

Funcion value <- deposit ()
	Imprimir " How much do you want to deposit: " 
	Leer value 
	
FinFuncion

Funcion value <- Withdraw ()
	Imprimir " How much do you want to withdraw: " 
	Leer value 
FinFuncion

Algoritmo ExampleCahier
		Imprimir cashier()
FinAlgoritmo

```
- Run Program

![Image](/Challenge%20Week%20%235/Images/4247-PSeInt_-_Ejecutando_proceso_EXAMPLECAHIER.png)

#

### 2. Weather average

- Solution

```javascript
Funcion celsius <- FarenheittoCelsius(Farenheit)
	Definir celsius Como Real
	celsius = (Farenheit - 32)/ 1.8;
FinFuncion

Algoritmo ExampleWeatherAverage
	Count = 0
	total = 0
	
	Repetir
		Imprimir " Choose an option with the letter related: ";
		Imprimir "a. Enter a degrees celsius";
		Imprimir "b. Enter a degrees Farenheit";
		Imprimir "c. exit the program";
		Leer option ;
		si option = "a" | option = "b" Entonces
			count = count + 1;
			leer degree;			
		FinSi
		
		si option = "a" Entonces
			total = total + degree;
			
		FinSi
		
		si option = "b" Entonces
			total = total + FarenheittoCelsius(degree);
			
		FinSi
	Mientras Que option = 'a' | option = 'b'	
	
	Imprimir total/count;
FinAlgoritmo
```
- Run Program

![Image](/Challenge%20Week%20%235/Images/4248-PSeInt_-_Ejecutando_proceso_EXAMPLEWEATHERAVERAGE.png)

#
#

## CHALLENGES (Thursday)

### 1. if 

    - solution
``` javascript
let x = 10;

if (x > 5) {
  console.log("x is greater than 5");
} else if (x === 5) {
  console.log("x is equal to 5");
} else {
  console.log("x is less than 5");
}
```

#
### 2. While

- solution
``` javascript
let count = 1;

while (count <= 5) {
  console.log("Count: " + count);
  count++;
}
```

#
### 3. For
- solution
``` javascript
for (let i = 1; i <= 5; i++) {
  console.log("Count: " + i);
}
```


#
#