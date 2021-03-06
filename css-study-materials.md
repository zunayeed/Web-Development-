*  Deﬁne CSS and the role that it plays in WebDev
 use it to describe how page look -The "adjectives"
*  The General Rule:
 selector {  property: value;  anotherProperty: value; } 
* Examples:  
*  /*Make All h1's purple and 56px font*/ 
  h1 {  color: purple;  font-size: 56px; } 
 * /*Give All img's a 3px red border*/ img {  border-color: red;  border-width: 3px; 
 
 ## where to write styles? 
  1.  **Inline**
       ```html
		<h3 style="color: pink;">blah blah blah </h3>
		<h3 style="color: pink;">knock knock </h3>
		<p style="color: yellow;">blah blah blah </p>
        ```

 2.  __`<style>`__ Tag: need to be placed inside `<head>` tag
  * we want our css to be self contained in its own file. Htlm is structure and css is `<style>`
		
```css
// selector basic structure inside style tag and link tag
selector{
property:value;
}
```
			
 
 
 ```html
	 <head>
		<title>About Zunayeed</title>
		<style type="text/css">
			h1{
				color: red;
			}
			li{
				color: orange;
			}
		</style>
	</head>
```
3. ** writing css on a separate `.css` file,  and connecting it with a `<link>` tag inside `<head>` tag **. For example for app.css file, 
Separate file using `<link>` is the most preferred way of writing. `<link>` tag inside `<head>` tag should be:
	
 ```css
 <link rel="stylesheet" type="text/css" href="app.css">
 
 inside app.css file : 
 
 h1{
	color:red;
}
li{
	color:darkOrchid;
}
h4 {
	color:purple;
}
```

# Color

Color in CSS
Hexadecimal
####  # + String of 6 hexadecimal numbers(from 0-F)
h1 {color: #000000;}
h2 {color: #4B0082;}
h3 {color: #FF1493;}
# + String of 6 hexadecimal numbers(from 0-F)
#### Color in CSS: RGBA
3 channels: Red, Green, and Blue.  Each ranges from 0 - 255
```css
h1 {color: rgb(0,255,0);}
h2 { color: rgb(100, 0, 100);}
h3 {color: rgb(11, 99, 150);}
```
#### Color in CSS RGBA
> Just like RGB, but with an alpha(transparency) channel.  Ranges from 0.0 - 1.0
```css
h1 {color: rgba(11, 99, 150, 1);}
h2 {color: rgba(11, 99, 150, .6);}
h3 {color: rgba(11, 99, 150, .2);}
```
## mix of color syntax combiration:
```css
h1{color:#FF001A;}
li{color:rgb(0,255,0);}
h4 {color:rgba(0,255,200,.5);}
```
####  Color and Background
## Use 'color' attribute to set text color and 'background' attribute for background color
```css
body {background: #95a5a6;}
div{background: #3498db;}
p {color: #ecf0f1;}
```
* Background Image
The background property can also set a background image
body {
background:url(<url of the image>);
background-repeat: no-repeat;// if you do not wanna repeat image
           // but it might not srteach out to cover the full image
background-size:cover// it will ensure taking up entire body
 
 }
*  border color in css has 3 different parts: 
     -  width, 
     -  style,
     -  color
     Example: 
 h1{
	color:#FF001A;
	border-color: purple;
	border-width: 5px ; 
	border-style: solid;
}
* shortcut syntax of border:  **border: width style color;**
   -  example:
   ```css
       border: 5px solid purple;
       border: 2px dashed purple;
  ```
   ...................---------------------------------------
   
   
### Aboutme.htlm: 

```html
   <!DOCTYPE html>
<html>
<head>
	<title>About Zunayeed</title>
	<link rel="stylesheet" type="text/css" href="app.css">
</head>
<body>
	<h1>Zunayeed Kamal</h1
	<h4>My Hobbies </h4>
	<ul>
		<li >Learning CSS</li>
		<li>Learning Java Core</li>
		<li >Learing Springboot</li>
		<li>Learing Advanced JDBC part 2</li>
	</ul>
</body>
</html>
```

*  Inside app.css :
```css

h1{
	color:#FF001A;
	/*border-color: purple;
	border-width: 5px ; 
	border-style: solid;*/
	/*border: 5px solid purple;*/ 
	border: 2px dashed purple;  
}
li{
	color:rgb(0,255,0);
}
h4 {
	color:rgba(0,255,200,.5);
	background: rgb(255,120,80);
}
body {
  background: pink; 
    /* background:url(https://thenypost.files.wordpress.com/2020/04/moana-the-rock-01.jpg?quality=90&strip=all&w=606);
    background-repeat: no-repeat;
    background-size: cover;
    */
}
```   
   
----------------------------------------------------------------------   

# 3 CSS Selectors: element, id, class 

 1. Element Selector: 
Select all instances of a given element. An HTML element usually consists of a start tag and an end tag, with the content inserted in between:
<tagname>Content goes here...</tagname>

The HTML element is everything from the start tag to the end tag:
Ex. <p>My first paragraph.</p>

Here we have 2 divs and both divs have 2 paragragp,we slelect both divs to be purple and we get 2 purple divs. 
<div>
  <p>You say yes</p>
  <p>I say no</p>
</div>

<div>
  <p>You say goodbye</p>
  <p>I say hello </p>
</div>

div{
  background: purple;
}
p {
  color: yellow;
}
 -------------------------------------
 #  ID Selector:
Selects an element with a given ID.  Only one per page!We can have multiple id in a page, as long as they appear only once.
<li id = special><input type="checkbox" name=""> Study CSS</li>
#special{color: yellow;}

#  Class Selector 
Select all elements with a given class. If we want to select half of the li in one way, and other half of the li in different ways, we go for class selector. It is just like an id and we can apply it to any number of times.

```html
<ul>
		<li class = "completed">
			<input type="checkbox" name=""> Buy Groceries
		</li>
		<li class = "completed">
			<input type="checkbox" name=""> Watch Movies
		</li>
		<li id = special>
			<input type="checkbox" name=""> Study CSS
		</li>
	</ul>
```

```css
.completed{
	text-decoration: line-through;
}
```
-  The text-decoration property specifies the decoration added to text.It can be: 
*  text-decoration: overline;
*  text-decoration: line-through;
*  text-decoration: underline;
*  text-decoration: underline overline;

----------------------------------------------------------
	you can add  "checked" to checkbox in order to make the box checked while loading the page.  
	<input type="checkbox" checked>
-----------------------------------------------------------------
#  Selectors in CSS 
*  /* elements*/  `li{}`
*  /* class*/    `.hello{}`
*  /* id */       `#name{}`
   `*` selector applies to whole page 
*  /* star*/    `*{border: 1px solid lightgrey;} `
* /*Descended  or nested  */    `li .hello {font-size: 25px;}`
*  /*Adjacent selector*/  ` h4+ul{ border: 4px solid red;}`


##  **Descendended selector(nested selector):** 
   -  It takes two or more elememt tag name and you select them together. 
   -  For instance, if we want to select all  `<a>`  tag inside ` <li> ` tag: 
```css  
li a{ 
color: red;
}  
```  

```html
<ul>
<li>One</li>
<li>Two!</li>
<li>Three</li>
</ul>
```

  Above  code will select all `<a>` inside `<li>`
    -  `li .hello {}` will select all hello inside `<li>`
	
## **Adjacent selector**: Adjacent selector will allow us to select element that come after another element, but not nested insie, it will allow us to select siblings.  
  The adjacent sibling combinator (+) separates two selectors and matches the second element only if it immediately follows the first element, and both are children of the same parent element.
  ```css
 /* Paragraphs that come immediately after any image */
img + p {
  font-weight: bold;
}
```
Syntax
former_element + target_element { style properties }
CSS Example
```css
li:first-of-type + li {
  color: red;
}
```
HTML
```html
<ul>
  <li>One</li>
  <li>Two!</li>   /*red*/ 
  <li>Three</li>
</ul>
```
## Attribute Selector 
The CSS attribute selector matches elements based on the presence or value of a given attribute
* **it can be used to select images of a particular source or all inputs of a particular type**
* `/* <a> elements with an href attribite matching "https://www.goole.com" */`

```css
a[href="https://www.google.com"] {
  color: green;
}
```
 * another example: 
```css
input[type="checkbox"]{
background:blue;
}
```

CSS :nth-of-type() Selector: 
1.	ul:nth-of-type(3){
	background: purple;
	}
2.   Specify a background color for every <p> element that is the second p element of its parent:
	p:nth-of-type(2) {
	  background: red;
	}
  for selection of even number: 
	p:nth-of-type(2) {
	  background: red;
	}

Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied. Specificity is based on the matching rules which are composed of different sorts of CSS selectors.

##  :checked selector
The :checked CSS pseudo-class selector represents any radio `(<input type="radio">)`, checkbox `(<input type="checkbox">)`, or option `(<option> in a <select>)` element that is checked or toggled to an on state.
```css
/* Matches any checked/selected radio, checkbox, or option */
input[type="checkbox"]:checked {
  margin-left: 25px;
  border: 1px solid blue;
}
```


```css
/* Give the <body> element a background of #bdc3c7*/
body{
	background: #bdc3c7 ;
}

/* Make the <h1> element #9b59b6*/
 h1{
 	color:#9b59b6;
 }

/* Make all <h2> elements orange */

h2{
	color:orange;
}
/* Make all <li> elements blue(pick your own hexadecimal blue)*/ 
li{
	color:#0000ff;
}

/*Change the background on every paragraph to be yellow*/

p{
	background: yellow;

}
/*Make all inputs have a 3px red border*/
 input{
 	border: 3px solid red;
 }

/* Give everything with the class 'hello' a white background*/
.hello{
	background: white;
}

/* Give the element with id 'special' a 2px solid blue border(pick your own rgb blue)*/
#special{
	border: 2px solid rgb(0,12,255);
}

/*Make all the <p>'s that are nested inside of divs 25px font(font-size: 25px)*/

div p {
	font-size: 25px;
}
/*Make only inputs with type 'text' have a gray background*/
input[type = "text"]{
	background: gray; 
}

/* Give both <p>'s inside the 3rd <div> a pink background*/
 div:nth-of-type(3) p{
 	background-color:pink;
 }
 
/* Give the 2nd <p> inside the 3rd <div> a 5px white border*/
 div:nth-of-type(3) p:nth-of-type(2){
 	border: 5px solid white;
 } 

/* Make the <em> in the 3rd <div> element white and 20px font(font-size:20px)*/
div:nth-of-type(3) em{
	color: white;
	font-size: 20px;
}


/*BONUS CHALLENGES*/
/*You may need to research some other selectors and properties*/
 
/*Make all "checked" checkboxes have a left margin of 50px(margin-left: 50px)*/
/*It will add some space on the left margin of checkbox when checked*/
 input[type="checkbox"]:checked {
	margin-left: 50px;
}

/* Make the <label> elements all UPPERCASE without changing the HTML(definitely look this one up*/
label {
  text-transform: uppercase;
}

/*Make the first letter of the element with id 'special' green and 100px font size(font-size: 100)*/
#special:first-letter {
  color: green;
  font-size: 100px;
}

/*Make the <h1> element's color change to blue when hovered over */
h1:hover {
  color: blue;
}

/*Make the <a> element's that have been visited gray */
a:visited {
  color: gray;
}



```



