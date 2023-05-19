# CHALLENGES FROM WEEK # 4 

## Index
- ### Week challenges (Monday)
    - [1. Average sales and commission](#1-average-sales-and-commission)
    - [2. Even or Odd](#2-even-or-odd)
- ### Week challenges (Tuesday)
    - [1. Predefined functions](#1-predefined-functions)
    - [2. Full name](#2-full-name)
    - [3. Throw dice](#3-throw-dice)
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
### 2. Even or Odd

#

## Week challenges (Tuesday)
### 1. Predefined functions
#
### 2. Full name
#
### 3. Throw dice
#
## Week challenges (Wednesday)

### 1. Distance to zero
#
### 2. Toss coin

#
#
## Week challenges (Thursday)
 ### 1. Structure of a function

#
 ### 2. Total price

 ### 3. Reverse direction and size

#