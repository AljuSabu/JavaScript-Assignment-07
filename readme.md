# JavaScript Assignment 07

### 1. Write a JavaScript function to check whether an `input` is an array.
(Array.isArray([1,2,3]))
 
**Ans.** 

```js
function arr(input){
    return Array.isArray(input)
}
if (arr([1,2,3])===true) {
    console.log("The input is an Array");
} else {
    console.log("The input is not an Array");
}
```

### 2. Write a JavaScript function that takes an array as an argument and returns the first element of the array.

**Ans.** 

```js
function firstElement(arr){
    return arr[0]
}
console.log(firstElement([1,2,3,4]));
```

### 3. Write a JavaScript function that takes an array as an argument and returns the last element of the array.

**Ans.** 

```js
function lastElement(arr){
    return arr[arr.length-1]
}
console.log(firstElement([1,2,3,4,5,6,7,8]));
```

### 4. Write a simple JavaScript function to join all elements of the following array into a string. 
Sample array : myColor = ["Red", "Green", "White", "Black"];

**Ans.**

```js
function arr(myColor){
    return myColor.join(" ")
}
let myColor = ["Red", "Green", "White", "Black"];
console.log(arr(myColor));
```

### 5. Write a JavaScript program that accepts a number as input and inserts dashes (-) between each. For example, if you accept 925468 the output should be 9-2-5-4-6-8
(toString().split().join())

**Ans.** 

```js
function arr(input){
    return input.toString().split("").join("-")
}
console.log(arr(987654));
```

### 6. Write a JavaScript function that checks if the given number is even or odd then returns a Boolean value.
(use: arrow function, return keyword, ternary operator)

**Ans.** 

```js
let input = (num)=>{
    return num%2===0
}
console.log(input(10));
```

### 7. Create an array of guestList. Write a javascript function that takes the user’s name as an argument and checks whether it is in the guestlist. If yes, return the string “Welcome” else, return “Sorry, good luck next time”.

**Ans.** 

```js
function check(name){
    let guestList = ["Alju","Remith","Abhinav","Alan","Athul"]
    if (guestList.includes(name)) {
        return "Welcome"
    } else {
        return "Sorry, good luck next time"
    }
}
console.log(check("Alju"));
```

### 8. Write a javascript function that reverses a given number.
example: 123456789 => 987654321 (toString(), split(), reverse (), join())

**Ans.** 

```js
function reverseNum(input){
    return input.toString().split("").reverse().join("")
}
console.log(reverseNum(54321));
```

### 9. Write a JavaScript function that accepts a string as a parameter and converts the first letter into upper case.
Example: “javascript” => “Javascript”

**Ans.** 

```js
function finalString(input){
    return input.charAt(0).toUpperCase()+input.slice(1)
}
console.log(finalString("javascript"));
```

### 10. You will create a function that tells us how many days, weeks, and months we have left if we live until 90 years old. It will take your current age as the input and console.logs a message with our time left in this format:
You have x days, y weeks, and z months left. where x, y, and z are replaced with the actual calculated numbers. For this challenge, assume there are 365 days in a year, 52 weeks in a year, and 12 months in a year. 

**Ans.**

```js
function timeLeft(age){
    let yearsLeft = 90-age
    let days = yearsLeft*365
    let weeks = yearsLeft*52
    let months = yearsLeft*12
    console.log(`You have ${days} days, ${weeks} weeks, and ${months} months left`);
}
timeLeft(16)
```

### 11. The Body Mass Index (BMI) is a way of estimating the amount of body fat. It's used in medicine to calculate risk of heart disease.
You can calculate it using the formula, where weight divided by height squared.Your challenge is to create a function that takes weight and height as inputs and gives the calculated BMI value as an output. The output should be rounded to the nearest whole number.The first parameter should be the weight and the second should be the height.

**Ans.** 

```js
function calculator(weight,height){
    let bmi = weight/(height*height)
    return Math.round(bmi)
}
console.log(calculator(70,1.72));
```
