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


