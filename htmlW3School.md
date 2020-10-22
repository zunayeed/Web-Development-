```html
<!DOCTYPE html>
<html>
<head>
	<title>Hello Custom Food Subsidy</title>
	<style type="text/css">
		p{
			color:red;
			text-align: center;
		}
		#para2{
			color:green;
			text-align:left;
		}
		p.center{
			text-align: center;
			color:blue;
		}

	</style>

</head>
<body>
	<h1 class="center"> This heading will not get affected by heading by class attribute</h1>

    <p>This is a custom food subsidy side for all people. </p>

    <p id ="para2">Id selector uses iid attribute of HTML element to select a specific element. 
	    The id of an element is unique within a page, so id selector is used to select one unique element.
	    To select an element with a specific id, write a hash(#) character, followed by the id of the element.</p>

    <p class="center">This paragraph will get affected by class attribute
    
    </p>

</body>
</html>
```
```html
<!DOCTYPE html>
<html>
<head>
	<title>Hello Custom Food Subsidy</title>
	<style type="text/css">
		p.center{
			text-align: center;
			color:red;
		}
		p.large{
			font-size: 200%;
		}

	</style>

</head>
<body>
	<h1 class="center"> This heading will not get affected by heading by class attribute</h1>

    <p class="center">This paragraph will be red and center-aligned.</p>
    <p class="center large">This paragraph will be red, center aligned, and in a large font size</p>

</body>
</html>
```
```html
<!DOCTYPE html>
<html>
<head>
	<title>Hello Custom Food Subsidy</title>
	<style type="text/css">
		*{
			text-align: center;
			color:blue;
		}
	</style>

</head>
<body>
<h1>Hello World to universal selectors</h1>
<p>Every element on on this page will get affected by the style</p>
<p id="para1">This para with id para1 will get affected by universal selectors as well</p>
<h5>this heading h5 will also get affected</h5>

</body>
</html>
```
```html 
<!DOCTYPE html>
<html>
<head>
	<title>Hello Custom Food Subsidy</title>
	<style type="text/css">
	h1,h2,p,h5{
		text-align: center;
		color:red;
	}
	</style>

</head>
<body>
<h1>Hello World of group selectors</h1>
<h2>Smaller heading of selectors</h2>
<p>this is a paragraph to demonstrate groupnig selectors of different elements</p>
<h5>this heading h5 will also get affected</h5>

</body>
</html>
```

-------------------------------------------------
## external css file 
- Inside mystyle.css file : in html link attribure is used to address the file
```css
body{
	background-color: lightblue;
}
h1{
	color: navy;
	margin-left:20px;
}
h2,p,h5{
		text-align: center;
		color:red;
	}
```
```html
<!DOCTYPE html>
<html>
<head>
	<title>Hello Custom html</title>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<body>
<h3>external html are defined with link tag inside head section of html page</h3>
<h1>Hello World of group selectors</h1>
<h2>Smaller heading of selectors</h2>
<p>this is a paragraph to demonstrate groupnig selectors of different elements</p>
<h5>this heading h5 will also get affected</h5>

</body>
</html>
```
- Inline styles are defined within the "style" attribute of the relevant element:
```html
<!DOCTYPE html>
<html>
<head>
	<title>Inline Style CSS</title>
</head>
<body>
<h1 style="color:blue;text-align: center">This is a heading</h1>
<p style="color:red">This is a paragraph</p>
</body>
</html>
```
```html
<!DOCTYPE html>
<html>
<head>
	<title>multiple style practice sheet</title>
	<link rel="stylesheet" type="text/css" href="mystyle.css">
	<style type="text/css">
		body{background-color: linen;}
	</style>
</head>
<body style="background-color: lavender">
	<h1>Multiple style cascaded into one </h1>
	<p>here the background color of the page is set with inline css, and also with an internal css, and also with external css</p>

</body>
</html>
```
```css

body{
	background-color: lightblue;
}
h1{
	color: navy;
	margin-left: 20px;
}
```

