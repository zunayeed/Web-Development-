# Basics of HTML



      <h1>I'm a header </h1>
    <h2>I'm a slightly smaller header </h2>
    <h6>I'm the smallest header </h6>
    <p>I'm a paragraph</p>
    <button>I'm a button!</button>
    <ul>
    	<li>List Item 1</li>
	    <li>List Item 2</li>
    </ul>


    <ol>
	<li>List Item 1</li>
	<li>List Item 2</li>
    </ol>
    
    
        <h1>I need a closing tag </h1>

         <p>Me too! need closing tag</p>
    
       <!-- No closing tag or inner text needed -->

       <img src="corgi.png">

       <link href="style.css">

      <!-- Don't worry about what these tags do yet -->
      
      
 ## What is div  ?   
The HTML Content Division element (<div>) is the generic container for flow content. It has no effect on the content or layout until styled using CSS.
As a "pure" container, the <div> element does not inherently represent anything. Instead, it's used to group content so it can be easily styled using the class or id attributes, marking a section of a document as being written in a different language (using the lang attribute), and so on.
HTML
<div class="shadowbox">
<p>Here's a very interesting note displayed in a
lovely shadowed box.</p>
</div>
Css
.shadowbox {
width: 15em;
border: 1px solid #333;
box-shadow: 8px 8px 5px #444;
padding: 8px 12px;
background-image: linear-gradient(180deg, #fff, #ddd 40%, #ccc);
}

### What is <span>?
	The HTML <span> element is a generic inline container for phrasing content, which does not inherently represent anything. It can be used to group elements for styling purposes (using the class or id attributes).
	<p>Add the <span class="ingredient">basil</span>, <span class="ingredient">pine nuts</span> and <span class="ingredient">garlic</span> to a blender and blend into a paste.</p>

<p>Gradually add the <span class="ingredient">olive oil</span> while running the blender slowly.</p>

----------------------------------
span.ingredient {
    color: #f00;
}
------------------------------------------------------------------------------------------------

#### What is attributes? 
Adding Additional Information To Tags. It is like property: value .   <tag name="value"></tag>
<img src="corgi.png">

<p class="selected">woof woof</p>

<a href="www.google.com">Click me to go to Google</a>

<link rel="stylesheet" type="text/css" href="style.css">

#### what does src attribute do ? 
Answer: The URL of the embeddable content. 
<img src="corgi.png">

#### Links: <a> tag with <href> attribute . it is in-line 
<a href="url">Link Text</a>
<a href="http://www.google.com">Click me to go to Google</a>
<a href="http://www.reddit.com">Click me to go to Reddit</a>
	To create a link of different page : <a href="page2.html"> Go to Page2</a>
	
### show Table Description with border: 	
<table border = "1" >
	<thead>
		<tr>
			<th>Name</th>
			<th>Age</th>
			<th>Job Location</th>
		</tr>
	</thead>
	<tbody>
	
	<tr>
		<td>Zunayeed</td>
		<td>30</td>
		<td>Indiana</td>
	</tr>
	<tr>
		<td>Zinia</td>
		<td>25</td>
		<td>Dhaka</td>
	</tr>
	<tr>
		<td> Nusrat</td>
		<td>34</td>	
		<td>Dhaka</td>
	</tr>
	</tbody>
	
</table>

### another example of table 

<h1>First Generation Pokemon Chart</h1>
<table border = "1">
	<thead>
		<tr>
			<th>Image</th>
			<th>Name</th>
			<th>Type</th>
			<th>Evolves Into</th>
		</tr>
	</thead>
	<tbody>
<!-- Bulbasour	-->
	<tr>
		<td>
			<img width= "70"   src="http://img4.wikia.nocookie.net/__cb20140328190757/pokemon/images/thumb/2/21/001Bulbasaur.png/200px-001Bulbasaur.png">
		</td>
		 <td>Bulbasaur</td> 
		<td>Grass/Poison</td>
		<td>
			 <a href="http://pokemon.wikia.com/wiki/Ivysaur "> Ivysaur </a>  
		</td>
	</tr>


	<!-- Charmander-->
	<tr>
		<td>
			<img width= "70" src="http://img4.wikia.nocookie.net/__cb20140724195345/pokemon/images/thumb/7/73/004Charmander.png/200px-004Charmander.png">
		</td>
		<td>Charmander</td> 
		<td>Fire</td>
		<td>
			<a href="http://pokemon.wikia.com/wiki/Charmeleon "> Charmaleon</a>
		</td>
	</tr>

	<!--Squirlet-->    
	 <tr>
		<td> 
			<img width= "70" src="http://img1.wikia.nocookie.net/__cb20140328191525/pokemon/images/thumb/3/39/007Squirtle.png/200px-007Squirtle.png">
		</td>
		<td>Squirtle</td>
		<td>Water</td>
		<td>
			<a href="http://pokemon.wikia.com/wiki/Wartortle"> Wartortle</a>
		</td>
	</tr>
	</tbody>
	
</table>


### <form> tag 
	Use the <form></form> tag
	       *     <form action="/my-form-submitting-page" method="post">
                      <!-- All our inputs will go in here -->
                      </form>
	       *  action - the URL to send form data to
               *   method - the type of HTTP request 
	google search is a get request 
	post request to send data to database and get data from databsae: facebook loging, twitter login


	
	
      ##  Use the <input> tag
  The HTML <input> element is used to create interactive controls for web-based forms in order to accept data from the user;
      
<input type="text">

<input type="date">

<input type="color">

<input type="file">

<input type="checkbox">
      
      
  ## Use the <label></label> tag
  
  <h1>Sign In</h1>

<form action="/sign-in-url" method="post">
    <input type="text">
    <input type="password">
    <button>Login</button>
</form>

* <input type="text" placeholder="username">
 here, placeholder is used to fill the box temporarily
	
Write Simple Validations
## another form 
<!-- action - where the form send data to-->
<!-- method - what http method(get/post) -->
<h1>Login Form </h1>
<form action= "http://wikipedia.com" method="get">
<input  name= "username" type="text" placeholder="username"><br/><br/>
<input  name= "password" type="password" placeholder="password"><br/><br/>
<input type="date"><br/><br/>
<input type="color"><br/><br/>
<input type="file"><br/><br/>
<input type="checkbox"><br/><br/>
<input type="submit">
</form>

### name attribute: Name of the input form control. Submitted with the form as part of a name/value pair.

<form action="/sign-in-url" method="post">
    <label>Username: <input type="text"></label>
    <label>Password: <input type="password"></label>
    <button>Login</button>
</form>

## Label Syntax : helpful for detection by visually impaired people
<form action="/sign-in-url" method="post">
    <label>Username: <input type="text"></label>
    <label>Password: <input type="password"></label>
    <button>Login</button>
</form>
	### Alternate syntax, using "for" and  "id" attributes: Here for and id need to be matched. for is used inside <label> tag , and id is used inside <input> tag connecting label with input. It will help visually impaired people.
<form action="/sign-in-url" method="post">
    <label for="username">Username:</label>
    <input id="username" type="text">
    <label for="password">Password:</label>
    <input id="password" type="password">
    <button>Login</button>
</form>	
        
# custom validation

- The 'required' attribute validates that an input is not empty
- There are also type validations.  Try changing "type" from "text" to "email"
------------
 <label for="emailforId">Email:</label>
	<input  id ="emailforId" name= "email" type="email" 
	 placeholder="username" required><br/><br/>

---------
<form action="/sign-in-url" method="post">
    <label for="email">Email:</label>
    <input id="email" type="email" required>
    <label for="password">Password:</label>
    <input id="password" type="password" required>
    <button>Login</button>
</form>
---------------------------------

<input type="radio"><br/><br/>
<input type="checkbox"><br/><br/>

To select one radio button out of 2 options, we need to bind it with name attribute, only then <form> tag will select one option. without value attribute, in the browser, you will see only petChoice=on, and we do not want it, so we use value attribute. 

<form>
<label for="dogs"> Dogs:</label>
 <input type="radio" id="dogs" name="PetChoice" value="DogChoice">
 <label for="cats"> Cats:</label>
<input type="radio" id="cats" name="PetChoice" value="CatChoice">
<input type="submit">
</form>

 ## <select> tag 
	-to create dropdown menues. Inside the select tag, we use <option> tag so that we can have lots of menues. name attribute need to be added inside select tag, if we want to see select option in the url. without name attribute, nothing will appear in browser regarding color. 
<p>What is your favorite color?</p>
<select name="color">
	<option>Red</option>
	<option>Green</option>
	<option>Yellow</option>
</select>
	If we use emoji, inside option tag, we will not get proper emotion in url, we will get something like %3a%29 and we don't want it. So, we use value attribute inside <option> tag.
	
<p>What is your mood?</p>
<select name="MoodSelection">
	<option value="happy">:)</option>
	<option value="neutral">:|</option>
	<option value = "sad">:(</option>
</select> </br>

## what is <textarea> ? 

The HTML <textarea> element represents a multi-line plain-text editing control, useful when you want to allow users to enter a sizeable amount of free-form text, for example a comment on a review or feedback form. Need to use name attribute, otherwise it will not be visible to url
Example:  <textarea name="textarea"rows="10" cols="50">
	   Write something here indise textarea</textarea>







