## Javascript Programming Tasks

Try to use best programming practices when writing solutions.
Focus more on code readability and coding conventions, not trying to 
create the most efficient and compact solution (which are often 
really hard to read/understand).

### Problem 1

Your job is to create a simple password validation function, as seen on many websites.
The rules for a valid password are as follows:

- There needs to be at least 1 uppercase letter.
- There needs to be at least 1 lowercase letter.
- There needs to be at least 1 number.
- The password needs to be at least 8 characters long.
- You are permitted to use any methods to validate the password.

For example:

```javascript
password("Abcd1234") // -> true
password("Abcd123") // -> false
password("abcd1234") // -> false
password("AbcdefGhijKlmnopQRsTuvwxyZ1234567890") // -> true
password("ABCD1234") // -> false
password("Ab1!@#$%^&*()-_+={}[]|\:;?/>.<,") // -> true
password("!@#$%^&*()-_+={}[]|\:;?/>.<,") // -> false
```

You will only be passed strings and the string can contain any standard keyboard character.
Accepted strings can be any length, as long as they are 8 characters or more.



### Problem 2

Create a piece of code named Car which takes model, register number and color as parameters and
 saves them to model, registerNumber and color properties. 
 Once created, model and registerNumber are **immutable** properties and cannot be 
 changed. Color property is mutable and can be changed directly or through .paint() method,
 which takes new color value as an argument.

```javascript
var car = new Car('Audi', 'ASD-123', 'green')
  
// then
car.model // -> 'Audi'
car.registerNumber // -> 'ASD-123'
car.color // -> 'green'
  
// and if you try
car.model = 'Ford'
car['registerNumber'] = 'QWE-987'
car.color = 'pink'
  
// then
car.model // -> 'Audi'
car.registerNumber // -> 'ASD-123'
  
// but
car.color // -> 'pink'
  
// also
car.paint('purple')
  
car.color // -> 'purple'

```

### Problem 3

The JavaScript standard includes functional additions to array like map, filter and 
reduce, but sadly is missing the convenience functions range and sum. Implement your 
version of range and sum methods.

Array.range(start, count) should return an array containing 'count' numbers from 'start' to 'start + count'
Array.sum() returns the sum of all numbers in the array.

For example:

```javascript
Array.range(0, 3) // -> [0, 1, 2]
Array.range(5, 5) // -> [5, 6, 7, 8, 9]
[0, 1, 2].sum() // -> 3
Array.range(-1, 4).sum() // 2
 
```
