*  Deﬁne CSS and the role that it plays in WebDev
 use it to describe how page look -The "adjectives"
*  The General Rule:
 selector {  property: value;  anotherProperty: value; } 
* Examples:  
*  /*Make All h1's purple and 56px font*/ 
  h1 {  color: purple;  font-size: 56px; } 
 * /*Give All img's a 3px red border*/ img {  border-color: red;  border-width: 3px; 
 
 ## where to write styles? 
  1.  Inline
       ```html
		<h3 style="color: pink;">blah blah blah </h3>
		<h3 style="color: pink;">knock knock </h3>
		<p style="color: yellow;">blah blah blah </p>
        ```

 2.  <style> Tag: need to be placed inside <head> tag
		
```html
<html>
<head>
<title>About Rusty</title>
<style type="text/css">
li {
color: red;
}
</style>
</head>
here basic structure is 
selector{
property:value;
}
```
			
 * we want our css to be self contained in its own file. Htlm is structure and css is style
 
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

*  writing css on a separate .css file,  and connecting it with a <link> tag inside <head> tag . For example for app.css file, 
 link tag inside <head> tag should be:
 
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
h1 {color: rgb(0,255,0);}
h2 { color: rgb(100, 0, 100);}
h3 {color: rgb(11, 99, 150);}
#### Color in CSS RGBA
Just like RGB, but with an alpha(transparency) channel.  Ranges from 0.0 - 1.0
h1 {color: rgba(11, 99, 150, 1);}
h2 {color: rgba(11, 99, 150, .6);}
h3 {color: rgba(11, 99, 150, .2);}
## mix of color syntax combiration
h1{color:#FF001A;}
li{color:rgb(0,255,0);}
h4 {color:rgba(0,255,200,.5);}

####  Color and Background
## Use 'color' to set text color and 'background' for background color

body {background: #95a5a6;}
div{background: #3498db;}
p {color: #ecf0f1;}

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
     -  color,
     -  style
     Example: 
 h1{
	color:#FF001A;
	border-color: purple;
	border-width: 5px ; 
	border-style: solid;
}
* shortcut syntax of border:  border: width style color;
   -  example: border: 5px solid purple;
   -   border: 2px dashed purple;
   ...................---------------------------------------
   
   
 Aboutme.htlm:   
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
--------------------------------------------------------------------
in app.css 

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

----------------------------------------------------------------
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
	--------------------------------------
.completed{
	text-decoration: line-through;
}
------------------------------------------------------



-  The text-decoration property specifies the decoration added to text.It can be: 
*  text-decoration: overline;
*  text-decoration: line-through;
*  text-decoration: underline;
*  text-decoration: underline overline;

----------------------------------------------------------
	you can add  "checked" to checkbox in order to make the box checked while loading the page.  
	<input type="checkbox" checked>
-----------------------------------------------------------------
#### Selectors in CSS 
*  /* elements*/  li{}
*  /* class*/    .hello{}
*  /* id */       #name{}
   *selector applies to whole page 
*  /* star*/   *{
		border: 1px solid lightgrey;	
} 
*  Descendended selector: It takes two or more elememt tag name and you select them together. 
    -  For instance, >   li a{ 
    				color: red;
			}    HTML
<ul>
  <li>One</li>
  <li>Two!</li>
  <li>Three</li>
</ul>
       will select all <a> inside <li>
    -  li .hello {} will select all hello inside li
	
*   Adjacent selector 
  The adjacent sibling combinator (+) separates two selectors and matches the second element only if it immediately follows the first element, and both are children of the same parent element.
  /* Paragraphs that come immediately after any image */
img + p {
  font-weight: bold;
}
Syntax
former_element + target_element { style properties }
CSS Example
li:first-of-type + li {
  color: red;
}
HTML
<ul>
  <li>One</li>
  <li>Two!</li>   /*red*/ 
  <li>Three</li>
</ul>


The CSS attribute selector matches elements based on the presence or value of a given attribute.
/* <a> elements with an href matching "https://www.goole.com" */
a[href="https://www.google.com"] {
  color: green;
}
 another example: 
	input[type="checkbox"]{
	background:blue;
	}

-------------------------------------------------------------

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
