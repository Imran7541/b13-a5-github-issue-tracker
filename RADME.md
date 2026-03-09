<-----------(1) What is the difference between var, let, and const?--------------------->

In JavaScript, var, let, and const are used to declare variables.

var:-------
var is the old way of declaring variables.It has function scope.
The same variable can be declared again.
Example: 
  var name ="Imran";
  var name = "Rahim";

Let:-------
let is used in modern JavaScript .It has block scope(work inside { }).
The value can be changed ,but the variable cannot be declared again in the same scope.

Example: let age = 24;
age = 21;

Const:--------
const also has block scope.The value cannot be changed after it is declared.
A Value must be assigned when declaring it.
Example:------
const country = "Bangladesh";

<--------------(2)What is the spread operator (...)?-------------->
The spread operator (...) is used to expand elements of an array or properties of an object.
It is often used to copy or combine arrays and objects.
Example with array:----------
const numbers = [1,2,3];
const nesNumbers = [...numbers,4, 5];
console.log(newNumbers);
output: [1,2,3,4,5]

<##############(3)What is the difference between map(), filter(), and forEach()?############>
These are array methods, but they work in different ways.
map()
map()goes through each element of an array.
it creates a new array after modifying each element.
Example: const numbers = [1,2.3];
     const result = numbers.map(n => n * 2);
     Result:[2,4,6]  
     
filter()------
filter() selects elements based on a condition.
It returns a new array with the elements that match the condition.

Example:
const numbers = [1, 2, 3, 4];
const result = numbers.filter(n => n > 2);
Result:[3,4]

forEach()------
forEach() loops through each element of an array.
It does not return a new array.

Example:
const numbers = [1, 2, 3];
numbers.forEach(n => {
  console.log(n);
});


<----*******************(4) What is an arrow function?*************---->
An arrow function is a shorter way to write functions in JavaScript.
It was introduced in ES6 and makes the code cleaner and easier to write.

Normal function: 
function add(a, b) {
  return a + b;
}

Arrow function:
const add = (a, b) => {
  return a + b;
};

##################(5)What are template literals?############################
Template literals are used to create strings with embedded variables.
They use backticks ( ) instead of single or double quotes.

Example:
const name = "Imran";
const age = 20;

const text = `My name is ${name} and I am ${age} years old.`;
console.log(text);
output:My name is Imran and I am 20 years old.
