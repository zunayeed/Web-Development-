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
 he
 ---

