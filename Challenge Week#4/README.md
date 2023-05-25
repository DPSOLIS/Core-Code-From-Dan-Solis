# CHALLENGES FROM WEEK # 4 

## Index
- ### Week challenges (Monday)
    - [1. Average sales and commission](#1-average-sales-and-commission)
    - [2. Even or Odd](#2-even-or-odd)
- ### Week challenges (Tuesday)
    - [1. Full name](#1-full-name)
    - [2. Throw dice](#2-throw-dice)
- ### Week challenges (Wednesday)
    - [1. Distance to zero](#1-distance-to-zero)
    - [2. Toss coin](#2-toss-coin)
    
- ### Week challenges (Thursday)
    - [1. Structure of a function](#1-structure-of-a-function)
    - [2. Total price](#2-total-price)
    - [3. Reverse direction and size](#3-reverse-direction-and-size)

#

## Week challenges (Monday)

### 1. Average sales and commission
- Solution
```javascript


Algoritmo SalesCommission
	
    Definir numVentas Como Entero
    Definir totalVentas, venta, comision Como Real
    Definir promedioVentas Como Real
	
    // Leer el número de ventas del vendedor
    Escribir "Ingrese el número de ventas realizadas:"
    Leer numVentas
	
    totalVentas = 0
	
    // Leer el valor de cada venta y calcular el total de ventas
    Para i<-1 Hasta numVentas Con Paso 1 Hacer
        Escribir "Ingrese el valor de la venta ", i, ":"
        Leer venta
        totalVentas = totalVentas + venta
    FinPara
	
    // Calcular el promedio de ventas
    promedioVentas = totalVentas / numVentas
	
    // Determinar la comisión del vendedor
    Si numVentas > 5 Entonces
        comision = totalVentas * 0.15
    Sino
        comision = totalVentas * 0.10
    FinSi
	
    // Mostrar los resultados
    Escribir "El promedio de ventas es: ", promedioVentas
    Escribir "La comisión del vendedor es: ", comision
	
FinAlgoritmo
```

- Run program

![image](/Challenge%20Week%234/Images/3869-PSeInt_-_Ejecutando_proceso_SALESCOMMISSION.png)

#

### 2. Even or Odd
- Solution:
```java
Algoritmo NumberDisplay
	
    Definir numero Como Entero
	
    // Leer el número del usuario y validar
    Repetir
        Escribir "Ingrese un número entre 1 y 50:"
        Leer numero
		
        Si numero < 1 & numero > 50 Entonces
            Escribir "Error: El número debe estar entre 1 y 50. Inténtelo nuevamente."
        FinSi
		
    Hasta Que numero >= 1 & numero <= 50
	
    Escribir "Los números son:"
	
    // Mostrar los números según si son pares o impares
    Si numero % 2 = 0 Entonces
        Para i <- 2 Hasta numero Con Paso 2 Hacer
            Escribir i
        FinPara
    Sino
        Para i <- 1 Hasta numero Con Paso 2 Hacer
            Escribir i
        FinPara
    FinSi
	
FinAlgoritmo
```
- Run program
![image](/Challenge%20Week%234/Images/3878-PSeInt_-_Ejecutando_proceso_NUMBERDISPLAY.png)

#

## Week challenges (Tuesday)

### 1. Full name
- Solution 
```Javascript
Algoritmo CapitalizeName
	
    Definir nombre, apellido, nombreCompleto, primerLetraNombre, primerLetraApellido Como Cadena
    Definir restoNombre, restoApellido Como Cadena
    Definir longitudNombre, longitudApellido Como Entero
	
    // Leer el nombre y el apellido
    Escribir "Ingrese su nombre:"
    Leer nombre
    Escribir "Ingrese su apellido:"
    Leer apellido
	
    // Obtener la primera letra y el resto del nombre
    primerLetraNombre = Mayusculas(subcadena(nombre, 0, 0))
    restoNombre = Minusculas(subcadena(nombre, 1, Longitud(nombre)-1))
	
    // Obtener la primera letra y el resto del apellido
    primerLetraApellido = Mayusculas(subcadena(apellido, 0, 0))
    restoApellido = Minusculas(subcadena(apellido, 1, Longitud(apellido)-1))
	
    // Construir el nombre completo capitalizado
    nombreCompleto = primerLetraNombre + restoNombre + " " + primerLetraApellido + restoApellido
	
    // Mostrar el nombre completo capitalizado
    Escribir "Nombre completo:", nombreCompleto
	
FinAlgoritmo
```
- Run Program

![image](/Challenge%20Week%234/Images/3879-PSeInt_-_Ejecutando_proceso_CAPITALIZENAME.png)

#
### 2. Throw dice
- solution 
```javascript
Algoritmo Dados
	Definir dado1, dado2 Como Entero
// Simular el lanzamiento de los dados 10 veces
Para i = 1 Hasta 10 Hacer
	// Lanzar los dados	
	dado1 = Aleatorio(1,6)
	dado2 = Aleatorio(1,6)
	
	
	
	// Comprobar si los valores de los dados son iguales y agregar el mensaje correspondiente
	Si dado1 = dado2 Entonces
		Imprimir dado1, " ",  dado2, " - Los dados son iguales"
	SiNo
		Imprimir  dado1, " ", dado2
	FinSi
	
	// Ir a la siguiente línea para el siguiente lanzamiento
	Escribir ""
	
FinPara
FinAlgoritmo
```
- Run Program

![image](/Challenge%20Week%234/Images/3880-PSeInt_-_Ejecutando_proceso_DADOS.png)

#
## Week challenges (Wednesday)

### 1. Distance to zero
- Solution 
```javascript
Algoritmo FurthestFromZero
	
    Definir valor1, valor2, valor3, valor4, valor5, maxValor, maxValorEntero Como Real
	
    // Leer los 5 valores
    Escribir "Ingrese el valor 1:"
    Leer valor1
    Escribir "Ingrese el valor 2:"
    Leer valor2
    Escribir "Ingrese el valor 3:"
    Leer valor3
    Escribir "Ingrese el valor 4:"
    Leer valor4
    Escribir "Ingrese el valor 5:"
    Leer valor5
	
    // Calcular el valor absoluto de cada número
    valor1 <- Abs(valor1)
    valor2 <- Abs(valor2)
    valor3 <- Abs(valor3)
    valor4 <- Abs(valor4)
    valor5 <- Abs(valor5)
	
    // Encontrar el valor máximo
    maxValor <- valor1
	
    Si valor2 > maxValor Entonces
        maxValor <- valor2
    FinSi
	
    Si valor3 > maxValor Entonces
        maxValor <- valor3
    FinSi
	
    Si valor4 > maxValor Entonces
        maxValor <- valor4
    FinSi
	
    Si valor5 > maxValor Entonces
        maxValor <- valor5
    FinSi
	
    // Obtener la parte entera del número máximo
    maxValorEntero <- abs(maxValor)
	
    // Mostrar el número entero más lejano a cero
    Escribir "El número entero más lejano a cero es:", maxValorEntero
	
FinAlgoritmo
```
- Run program

![image](/Challenge%20Week%234/Images/3881-PSeInt_-_Ejecutando_proceso_FURTHESTFROMZERO.png)


#

### 2. Toss coin
- solution

```javascript
Algoritmo CoinFlipGame
	
    Definir nombre1, nombre2 Como Cadena
    Definir valor1, valor2, resultadoAleatorio Como Real
	
    // Leer el nombre y valor del primer jugador
    Escribir "Ingrese el nombre del primer jugador:"
    Leer nombre1
    Escribir "Ingrese el valor del primer jugador:"
    Leer valor1
	
    // Leer el nombre y valor del segundo jugador
    Escribir "Ingrese el nombre del segundo jugador:"
    Leer nombre2
    Escribir "Ingrese el valor del segundo jugador:"
    Leer valor2
	
    // Verificar si alguno de los jugadores colocó un valor no válido
    Si valor1 <= 0 Entonces
        Escribir "El primer jugador ha colocado un valor no válido. ¡El segundo jugador gana!"
    Sino 
		Si valor2 <= 0 Entonces
			Escribir "El segundo jugador ha colocado un valor no válido. ¡El primer jugador gana!"
		Sino
			// Simular el lanzamiento de la moneda
			resultadoAleatorio = Aleatorio(valor1,valor2)
			
			// Verificar el resultado del lanzamiento de la moneda
			Si resultadoAleatorio >= 0.5 Entonces
				Escribir "¡", Mayusculas(nombre1), " gana con un valor de ", valor1, "!"
			Sino
				Escribir "¡", Mayusculas(nombre2), " gana con un valor de ", valor2, "!"
			FinSi
		FinSi
	FinSi
	
FinAlgoritmo
```
- run program Player 1 wins when the second player enter a negative number

![image](/Challenge%20Week%234/Images/3882-PSeInt_-_Ejecutando_proceso_COINFLIPGAME.png)

- run program Player 2 wins when the first player enter a negative number

![image](/Challenge%20Week%234/Images/3883-PSeInt_-_Ejecutando_proceso_COINFLIPGAME.png)

- run program when the program select the random winner

![image](/Challenge%20Week%234/Images/3884-PSeInt_-_Ejecutando_proceso_COINFLIPGAME.png)


#
#
## Week challenges (Thursday)
 ### 1. Structure of a function

#
 ### 2. Total price

 ### 3. Reverse direction and size

#