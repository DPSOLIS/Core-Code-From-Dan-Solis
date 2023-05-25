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

```
#
## Week challenges (Wednesday)

### 1. Distance to zero
- Solution 
```javascript

```
#
### 2. Toss coin
- solution
```javascript

```

#
#
## Week challenges (Thursday)
 ### 1. Structure of a function

#
 ### 2. Total price

 ### 3. Reverse direction and size

#