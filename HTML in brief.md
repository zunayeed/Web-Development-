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











