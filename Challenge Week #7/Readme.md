# CHALLENGES FROM WEEK # 7


## CHALLENGES (Monday)

### 1. String: substr()
- Exercise

Write a function firstWord, taking a string and returning the first word in that string. The first word are all characters up to the first space.

Example: firstWord('see and stop') should return 'see'.

- Solution
```javascript
function firstWord(input){

let space = input.indexOf(' ');
return input.substr(0,space);

}
```

- Result
```javascript
Reading your code successfully.

firstWord is a function.

firstWord has 1 parameter(s).

firstWord('see and stop') returns 'see'.

firstWord('speak again') returns 'speak'.

All tests passed!

```
#

### 2. String: replace()
- Exercise
Write a function normalize, that replaces '-' with '/' in a date string.

Example: normalize('20-05-2017') should return '20/05/2017'.

- Solution
```javascript
function normalize(dateString) {
  return dateString.replace(/-/g, '/');
}
```

- Result
```javascript
Reading your code successfully.

normalize is a function.

normalize has 1 parameter(s).

normalize('20-05-2017') returns '20/05/2017'.

normalize('8-11-1922') returns '8/11/1922'.

All tests passed!
```

#

### 3. Increment

Which value does x have after execution of the following code?
```javascript
let x = 3;
x++;
x = x * 2;
x--;
```

- Solution
```javascript
x= 3
x + 1 = 4
x = x*2 // X=4
x = 4 *2 = // X = 8
x -- // x - 1
x = 8-1 // x = 7

// The value of x is 7
```
#

### 4. Fahrenheit

-Exercise

Write a function toFahrenheit that converts a temperature from Celsius to Fahrenheit.

Example: toFahrenheit(0) should return 32.
- Solution
```javascript
function toFahrenheit(Celsius) {
return 1.8*(Celsius) + 32
}
```
- Result
```javascript
Reading your code successfully.

toFahrenheit is a function.

toFahrenheit has 1 parameter(s).

toFahrenheit(0) returns 32.

toFahrenheit(10) returns 50.

toFahrenheit(40) returns 104.

toFahrenheit(100) returns 212.

All tests passed!
```
#

### 5. Boolean 
- Exercise

Write a function nand that takes two Boolean values. If both values are true, the result should be false. In the other cases the return should be true.

I.e.: The call nand(true, true) should return false. The calls nand(true, false), nand(false, true) and nand(false, false) should return true.

- Solution
```javascript
function nand(one, two) {
let or = one && two;
return !or
}
```
- Result
```javascript
Reading your code successfully.

nand is a function.

nand has 2 parameter(s).

nand(true, true) returns false.

nand(true, false) returns true.

nand(false, true) returns true.

nand(false, false) returns true.

All tests passed!
```

#
## CHALLENGES (Tuesday)

### 1. Variables
- Solution
```javascript
```

## CHALLENGES (Wednesday)

### 1. Variables
- Solution
```javascript
```

## CHALLENGES (Thursday)

### 1. Variables
- Solution
```javascript
```