# CHALLENGES FROM WEEK # 6

## Index
- ### Week challenges (Monday)
    No challenges for this week, only watch the HTML VIDEOS
- ### Week challenges (Tuesday)
1.  Developtmen environment (the tools for html and javascripts have been set up)

    [2. Variables](#2-variables)

    [3. What is X](#3-what-is-x)
    
    [4. Several Variables](#4-several-variables)
    
    [5. Reassignment](#5-reassignment)
    
    [6. Assign Variables](#6-assign-variables)


- ### Week challenges (Wednesday)
    [1. MDN Repositary](https://developer.mozilla.org/en-US/docs/Web/javascript)
    
    [2. Functions](#2-functions)
    
    [3. Multiple Functions](#3-multiple-functions)
    
    [4. Function Calls](#4-functions-calls)
    
    [5. What is X](#5-what-is-x-function-version)
    
    [6. Parameters](#6-parameters)
- ### Week challenges (Thursday)
    [1. Strings](#1-strings)
    
    [2. Strings: length](#2-strings-lenght)

    [3. Strings: toUpperCase()](#3-strings-touppercase)

    [4. Strings: charAT()](#4-strings-charat)

    [5. Strings: IndexOf()](#5-strings-indexof)

#
#

## CHALLENGES (Tuesday)

### 2. Variables
- Solution
```javascript
let firstname = 'Lata';
```

### 3. What is X

Which value does x have after execution of the following code?
```javascript
let x = 'Geeta';
```

- Solution
```javascript
'Geeta'
```
### 4. Several variables 


- Exercise

Declare a variable flower and assign it the value 'rose'. Declare a second variable tree and assign it the value 'maple'.

- Solution
```javascript
let flower = 'rose';
let tree = 'maple';
```
### 5. Reassignment
- Exercise

Which value does x have after execution of the following code?
```javascript
let x = 'Tic';
x = 'Tac';
x = 'Toe';
```
- Solution
```javascript
'Toe'
```
### 6. Assign Variables
- Exercise

Which value does x have after execution of the following code?
```javascript
let x = 'Laurel';
let y = 'Hardy';
let z = y;
y = x;
x = z;
```
- Solution
```javascript
'Hardy'
```
#
#

## CHALLENGES (Wednesday)

### 2. Functions
- Exercise

Define a function hello that returns 
```
'Hello world!'.
```
- Solution
```javascript
function hello() {

return 'Hello world!';

}
```
### 3. Multiple Functions
- Exercise

Define two functions. The first function a should return 'Hello a!' and the second function b should return 'Hello b!'.

- Solution
```javascript
function a() {
 return 'Hello a!';
}

function b() {
 return 'Hello b!';
}
```

### 4. Functions Calls

- Exercise

1. Define a function greet returning the value 'Haydo!'.

2. Declare a variable salutation. Call the function greet and assign the result of the call to the variable salutation.

- Solution

```javascript
function greet() {
  return 'Haydo!';
}

let salutation = greet();
```

### 5. What is X? (Function version)

- Exercise

Which value does x have after execution of the following code?
```javascript
function reply(phrase) {
  return phrase;
}

let x = reply('How do you do?');

```
- Solution
```javascript
'How do you do?'
```

### 6. Parameters
- Exercise

Write a function echo that also returns the passed parameter. echo('Greta') should return 'Greta' and echo('CO2') should return 'CO2'

- Solution
```javascript
function echo(input) {
  return input;
}

let result = echo('Greta');
```

#
#

## CHALLENGES (Thursday)

### 1. Strings
- Solution
```javascript
```

### 2. Strings: Lenght
- Solution
```javascript
```

### 3. Strings: toUpperCase()
- Solution
```javascript
```

### 4. Strings: charAt()
- Solution
```javascript
```

### 5. Strings: indexOf()
- Solution
```javascript
```