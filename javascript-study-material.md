## Topics at JavaScript
- Primitives(5)
- variables(var)
- methods
  -  console.log(), 
  -  prompt(),
  -  alert() 
 ### Primitives
 1. Numbers
 2. Strings: 
  - Single or double quotes ok, 
  - escape chartacter starts with backslash "\"
  - Strings have length property `"helloworld".length `
  - Access individual characters `"Hello"[0] // h`
  - `"zunayeed"[0]  // z`
  
 3. Booleans
 4. null: explicitly nothing `var name = zunayeed; name = null;// no name`
 5. undefined: declared but uninitialized 
 ### Variables 
- `var name = "zunayeed";`
- Convention of variable: 
  -  camelCase(java scripts supports camelCase)
  -  snake_case(underscore between words)
  -  kebab-case(dash between words)
- Comments in js: //(double forwardslash)
###  Built-in methods: 
- clear() // to clear console
- alert("hello there"); // popup window will appaer at chrome saying hello world
  - can do maths also : `alert(2*3) // popup window saying 6 will appear `
- console.log("Hello"); // it will make the result appear in console
- use to prompt the user with:   `prompt("what is your name?")// value displayed in console`
  - can save the prompt valuein var: `var userName = prompt("What is your name? ");`
### JavaScripts 
```javascript
//alert("Hello from JS file");
var userName = prompt("What is your name");
alert("Nice to meet you, "+ userName);
console.log("Also great to meet you "+ userName);
```
### Adding Javascripts in html file
```html
<head>
	<title>Including JS Files</title>
	<script src = "script.js" type="text/javascript"></script>
</head>
```
### Example of javascript get user name and age, then  show it to console
```javascript
var firstName = prompt("What is your first name? ");
var lastName = prompt("What is your last name? "); 
var age = prompt("what is your age?");
var fullName = firstName + " " + lastName;
console.log("Your full name is "+ fullName );
console.log("you are "+ age +" years old" );
```
### Age Calculator: ageCalculator.js file
```javascript 
var age = prompt("Enter your age"); 
var totalDays= age*365 ; 
alert("you are "+ totalDays+ " alive");
```
## Javascript Basics: Control Flow(conditional statements and loops)
---
* Objective 1: Evaluate complex logical statements: 
  - Boolean operator
  - Logical operators 
  - Comparator operators 
* Objective 2: write 3 part JS Conditional statement(if-elseif-esle)
* Objective 3: Write js loops 
  - while loops
  - for loops 
* Objective 4: Translate between for and while loops
 ---
 * "==" performs type coercions, while "===" does not
 * Identity / strict equality (===):The identity operator returns true if the operands are strictly equal  with no type conversion.
   - main difference between "==" and "===" operator is that formerly compares variable by making type correction e.g. if you compare a number with a string with numeric literal, == allows that, but === doesn't allow that, because it not only checks the value but also type of two variable, if two variables are not of the same type "===" return false, while "==" return true. 
   - 3 === 3   // true
   - 3 === '3' // false
   - 
   ```java script
   var x = 99;
   x == "99"  //true
   x === "99" //false
   var y = null; 
   y == undefined //true
   y === undefined //false
   true == "1"          //true
   0 == false           //true
   null == undefined    //true
   NaN == NaN           //false
   ```
   - [Logical operator slides Link](http://webdev.slides.com/coltsteele/deck-4-47#/5)
   - Truthy and Falsy in boolean context: Values that aren't actually true or false, are still inherently "truthy" or "falsey" when evaluated in a boolean context. in console, it can be checked with negate operator !"hello"
   - Falsy Values:false,0,"",null,undefined,NaN, 
   - Everything Else Is Truthy
   -
   ```javascript
   // Get age and convert it to a Number (prompt always returns a String)
   var age = Number(prompt("What is your age?"));
	// If age is negative
	if(age < 0) {
	 console.log("Come back once you're out of the womb");
	}
	// If age is 21  
	if(age === 21) {
	 console.log("Happy 21st Birthday!");
	}
	// If age is odd
	//(not evenly divisible by two)
	if(age % 2 !== 0) {
	 console.log("Your age is odd!");
	}
	// If age is a perfect square
	if(age % Math.sqrt(age) === 0) {
	  console.log("Your age is a perfect square!");
	}
   ```
     ### Loop: [Link of Introduction to loops](http://webdev.slides.com/coltsteele/loops-58#/1)
 * DRY: Don't Repeat Yourself We want to keep our code as DRY as possible.  It saves us a lot of time and makes our code cleaner.
   
   ### Functions 
   ```javascript
   //to declare
   function sayHi(){
   console.log("Hello world"); 
   } 
   // to call 
   sayHi(); 
   ```
 
   ### Array 
   - reverse function
   ```javascript
   
   ```
  
