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
```css
p {font-family: Raleway;}
h1 {font-family: Indie Flower;}

```
# Box Model( padding, Marging, Border and more ) 
- Box Model
"In a document, each element is represented as a rectangular box.

In CSS, each of these rectangular boxes is described using the standard box model.

Each box has four edges: the margin edge, border edge, padding edge, and content edge."

Box Model
**Content**: whatever is written
**Padding**: space between content and border. it can be top, bottom, right, left
**Border**: it is width of content plus border
**Margin**: space outside of border between elements. between the order and outside anything else. If you want two paragraphs to be further apart, use margins
> width is content(written content) border.
> without padding, width and border resembles same.
>  `width <padding <border<margin`

## box model additional 
- [ ] Margin
- [ ] Outline
- [ ] Border
- [ ] Padding
- [ ] Content


