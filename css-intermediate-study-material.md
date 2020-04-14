# CSS intermediate
 1. Font and text related properties
 1. Include external fonts using google fonts 
 1. Define and manipulate four component of box model 
 1.  Project: Tic Tac Toe Board using box model,Image galary portfolio site, html and css blog
 
CSSfontstack.com
```css
/*font-family: to slelect font*/
p {font-family: Arial;}
h1 {font-family: Georgia;}

/*font-size*/
body {font-size: 10px;}
h1 {font-size: 5.0em;}/*five times larger than body*/
p {font-size: 2.0em;} 
span {font-size: 2.0em;}/*change the font to double based on context*/

/*font-weight: how thick the fonts are: bold, normal, 
some fonts allow you to use number between 100 to 800 with 100 increment:100,200,800
Example: google fonts*/
p{font-weight: normal;}

/*line-height: It confirms the space between lines*/
p {line-height: 1.5;}

/*text-align: It control how the text of a given element is controlled: right, center, left*/
h1 {text-align: right;}
p {text-align: center;}

/*text-decoration*/
p {text-decoration: underline;}
h1 {text-decoration: line-through;}

```

## Custom google fonts: 
* Step 1: add link in `<head>` tag: To embed a font, copy the code into the <head> of your html from embeded
```html
<head>
	<title>Fonts</title>
	<link rel="stylesheet" type="text/css" href="styles.css">
	<link href='https://fonts.googleapis.com/css?family=Raleway:400,700|Indie+Flower' rel='stylesheet' type='text/css'>
</head>
```
* Step 2: in .css file address the font property or CSS rules to specify families from website
/*font-family: 'Indie Flower', cursive; */
