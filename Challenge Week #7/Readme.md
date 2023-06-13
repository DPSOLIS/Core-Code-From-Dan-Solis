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

### 1. Register in Codewars
I already register in codewars with github account.

### 2. Objects
- Solution
```javascript
function animal(obj){
  // Access the properties of the object using dot notation or bracket notation

  var name = obj.name;
  var color = obj.color;
  var legs = obj.legs;
  
    // Create the desired string using string concatenation or template literals
var result = "This " + color + " " + name + " has " + legs + " legs."

return result
}
```

- result
```javascript
Time: 695ms Passed: 3Failed: 0
Test Results:
Tests
test
Test Passed: Value == '\'This white dog has 4 legs.\''
Test Passed: Value == '\'This red cock has 2 legs.\''
Test Passed: Value == '\'This gray rabbit has 4 legs.\''
Completed in 1ms
Completed in 5ms
You have passed all of the tests! :)
```

### 3. Return to sanity
- Solution
```javascript
function mystery() {
  var results =
    {sanity: 'Hello'};
  
  
  return results;
}
```

### 4. Object syntax debug
- Solution
```javascript
var rooms = {
  first: {
    description: 'This is the first room',
    items: {
      chair: 'The old chair looks comfortable',
      lamp: 'This lamp looks ancient'
      }
  },
  second: {
    description: 'This is the second room',
    items: {
      couch: 'This couch looks like it would hurt your back',
      table: 'On the table there is an unopened bottle of water'
    }
  }
}
```


## CHALLENGES (Wednesday)

### 1. Count a String in objects
- Explanation
```javascript

/*Create a function strCount (takes an object as argument) that will count all string values inside an object. For example:*/

strCount({
  first: "1",
  second: "2",
  third: false,
  fourth: ["anytime",2,3,4],
  fifth:  null
  })
  //returns 3
```

- Solution
```javascript
function strCount(obj) {
  let count = 0;

  for (let key in obj) {
    if (typeof obj[key] === 'string') {
      count++;
    } else if (typeof obj[key] === 'object' && obj[key] !== null) {
      count += strCount(obj[key]); // Recursively call strCount for nested objects
    }
  }

  return count;
}
```

### 2. VariablesExtending JavaScript Objects: Get First & Last Array Element
- explanation
```javascript
/*Your task is to extend JavaScript Array object, with methods .first() and .last(), so you can get respectively first or last element of the array.*/

var a = [2, 5, 7, 3 ,4];

a.first();  // 2
a.last();   // 4

/*Note: in case of empty array, methods should return undefined.*/
```

- solution
```javascript
Array.prototype.first = function() {
  if (this.length === 0) {
    return undefined;
  } else {
    return this[0];
  }
};

Array.prototype.last = function() {
  if (this.length === 0) {
    return undefined;
  } else {
    return this[this.length - 1];
  }
};
```
### 3. Object Oriented Piracy
- instructions
```javascript
/*
You have access to the ship "draft" and "crew". "Draft" is the total ship weight and "crew" is the number of humans on the ship.

Each crew member adds 1.5 units to the ship draft. If after removing the weight of the crew, the draft is still more than 20, then the ship is worth looting. Any ship weighing that much must have a lot of booty!

Add the method

isWorthIt
to decide if the ship is worthy to loot. For example:*/

titanic.isWorthIt() // return false
Good luck and may you find GOOOLD!
```

- Solution
```javascript
function Ship(draft, crew) {
  this.draft = draft;
  this.crew = crew;
  
}

Ship.prototype.isWorthIt = function() {
  var totalWeight = this.draft - (this.crew * 1.5);
  return totalWeight > 20;
};

var titanic = new Ship(15, 10);
console.log(titanic.isWorthIt()); // Output: false
```
## CHALLENGES (Thursday)

### 1. Variables
- Solution
```javascript
```