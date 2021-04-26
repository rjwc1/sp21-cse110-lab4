## Part 1a. A quick Introduction

### var declaration

Question 1. `values added: 20`

Question 2. `final result: 20`

### let declaration

Question 3. `values added: 20`

Question 4. The code returns an error because `result` was created inside of the if statement with `let` keyword. Using this variable outside this code block is out of scope.

### const declaration

Question 5. The code returns an error because line 7 tried to change the value of a `const` variable. This wil not allow for line 9 to print.

Question 6. The code returns an error because line 7 tried to change value of `const` variable. Also, if there was no code to change a `const` variable, this would also return an error because the variable is out of scope since it was created inside the if statement code block.

## Part 1b. A little more of a challenge

Question 1. At line 12, the number 3 is printed. This is because `i` is declared with the `var` keyword in the for loop, so it can be accessed anywhere inside the function it is defined in. The for loop will iterate until `i` becomes a 3 to fail the condition to continue as the array is indexed from 0 to 2. 

Question 2. At line 13, the number 150 is printed. This is because `discountedPrice` is declared with the `var` keyword in the for loop, so it can be accessed anywhere inside the function it is defined in. At the end of the for loop, the array of prices will get 50% off the last index that contains 300 and store 150 into `discountedPrice` as the last value.

Question 3. At line 14, the number 150 is printed. `finalPrice` is a `var` variable declared outside of the for loop and modified inside it, so this is fine. Also, `finalPrice` depends on `discountedPrice`, so `finalPrice` will just round `discountedPrice` and the last index of `prices` happens to be 300, so it gets 50% off and rounded into `finalPrice`.

Question 4. The function will return an array of discounted prices. We originally sent an array [100, 200, 300] and we would get discounted values for a new array of [50, 100, 150]. 

Question 5. At line 12, if this function is called, it would return an error because `i` is out of scope as it was declared using `let` keyword inside the for loop.

Question 6. At line 13, an error is returned because the variable `discountedPrice` was created inside the for loop using `let` so it is out of scope.

Question 7. At line 14, 150 gets printed. This is because `finalPrice` was created using `let` outside of the for loop so the variable is within scope of the entire function. The variable was used to create a rounded discount of each index of the array. At the end of the loop, it maintained the last rounded discount of 150 that came from 300.

Question 8. The function will return an array of discounted prices. We sent array values of [100, 200, 300] and we would get discounted values for a new array with [50, 100, 150].

Question 9. At line 11, it returns an error, because `i` was created with `let` in the for loop so it is out of scope.

Question 10. At line 12, 3 gets printed. While `length` is a `const`, there is no attempt to change the value from its assignment value of array size and the variable is within scope to output the value.

Question 11. The function will return an array of discounted prices of values [50, 100, 150].

Question 12. 

  A.  `student.name`
  
  B.  `student['Grad Year']`
  
  C.  `student.greeting()`
  
  D.  `student['Favorite Teacher'].name`
  
  E.  `student.courseLoad[0]`
  
Question 13. Arithmetic

  A. `'32'` - String Conversion: Adding an integer with string causes integer to map to their string represenation before concatenating
  
  B. `1` - Number Conversion: Subtracting a string with an integer causes string to convert to its number representation before applying arithmetic.
  
  C. `3` - Number Conversion: null is represented as a 0 with an integer so 0 + 3  is 3.
  
  D. `'3null'` - String Conversion: Adding null to a string will convert null to a string before concatentation since null is considered a 0 so we get a string as a result.
  
  E. `4` - Number Conversion: true maps to 1, so adding it to an integer creates number arithmetic.
  
  F. `0` - Number Conversion: false maps to 0 and null maps to 0, so adding these two creates number arithmetic.
  
  G. `'3undefined'` - String Conversion: undefined will map to its string representation before concatenating. 
  
  H. `NaN` - Arithmetic operation of undefined with subtracting a string results in a NaN.
  
Question 14. Comparison

  A. `true` - JavaScript converts the values to numbers when comparing different types, so the string becomes a number and 2 is greater than 1.
  
  B. `false` - String comparison: The first characters differ from each other and Unicode says '2' is NOT less than '1' so returns false.
  
  C. `true` - JavaScript converts the values to numbers when comparing different types, so string '2' becomes a number and it does equal 2.
  
  D. `false` - === is a strict equality operator that checks the equality without converting any types, so string '2' is not converted and is NOT equal to number 2.
  
  E. `false` - JavaScript converts the values to numbers when comparing different types, so true converts to 1. 1 is NOT equal to 2. 
  
  F. `true` - Boolean() converts other data types to a boolean, and Boolean(2) is true because non-zero numbers are considered true. The strict equality operator is comparing two true booleans, so return true.
  
Question 15. `==` is an equality operator that converts different data types before checking if two values are equal to return a boolean. Meanwhile, `===` is the strict equality operator that does NOT convert two different data types. Instead, it checks if the two operands are equal with their actual data type. If they're different data types, it will return false.

Question 16. (In part1b-question16.js)

Question 17. Array values of [2, 4, 6] get returned. Upon calling modifyArray, we send array values and a function. We inititiate a new array to store new values that we want to return. With the for loop, we iterate through the sent array values in `array`. In doing so, we send each index value to `doSomething(num)` that returns 2 times the value before pushing it to the `newArr` array. We do this until the end of the `array` values and return `newArr` with [2, 4, 6].

Questtion 18. (In part1b-question18.js)

Question 19. 
```
1
4
3
2
```
