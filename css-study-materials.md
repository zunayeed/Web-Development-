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
<h3 style="color: pink;">blah blah blah </h3>
<h3 style="color: pink;">knock knock </h3>
<p style="color: yellow;">blah blah blah </p>

 2.  <style> Tag: need to be placed inside <head> tag
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


 
