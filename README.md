homework
========
<!-- 1. The user needs to know what type of words to provide. No prompts. They cannot see the story until after.
2. It needs more words than actually needed, enough to cover 2 stories.(i only have one story right now). I will have to use the arrays for both stories. 
3. The script should store words in small arrays devoted to each category(nouns, colors, etc.
4. The user gets to pick story 1 or story 2
5. The story must be hidden until they select a story.
6. I wasn't sure how to connect all of the arrays to the user input on html. I was not sure if the story should be an array or function. I have not done much styling yet. I also have extra credit which i would like to do, but sadly I am running out of time. They are due Sunday night. -->
homework_madlib


<!DOCTYPE HTML>
<html lang = 'en-us'>
<head>
	<meta charset = 'utf-8'>
	<title>Week 5 Madlib</title>
	<script src = 'week5madlibtrialanderror.js'></script>
	<script>
	function connect() {
var message=" finally connected, bitch";
console.log(message);
}
	var $ = function(id) {
	return document.getElementById(id);
}
// I have to sort my variables into arrays.
var nouns = [];
		nouns[0];  // "mythical creature. i had an empty string here, that didnt work either so how do I connect the user input id with this
		nouns[1];   //noun- user chooses one
		nouns[2];   //color -user chooses one
		nouns[3];   //person -user chooses one
		nouns[4];  //body part -user chooses one
//=========================
var adj = []
		adj[0] ;
		adj[1] ;
		adj[2] ;
		adj[3] ;
		adj[4] ;
//===========================
var adv = [];
		adv[0] ;
		adv[1];
		adv[2] ;

var story;
	function story1() 	  { 
			"Dogs are a man's best"  + nouns[0] + ' .' +
			"Dogs are very " + adj[1] + " and can be taught many" + adj[0] + "tricks. "+
		  "A dog can be trained to carry a " + nouns[1] + " in his mouth. "+
		  "If you throw his " + nouns[0] + "  he will run and fetch it. "+
		  "One of the most popular dogs today is the " + nouns[2] + ". "+
		  "They have " + nouns[4] + " and " + adj[3] + " ears. "+
		  "Every home should have a " + adj[1] + nouns[0] + ". ";
$("storydisplay").innerHTML = story1();    
}

	</script>
	<style>
	input[type="text"] {
    width: 250px;
    display: block;
    margin-bottom: 10px;
	margin-top: 10px;
    background-color: pink;
}
	</style>
</head>
	 
<body onload = 'connect()'>	

<h2>Madlibs</h2>
<div><p>In case you need a refresher</p>
        Adjective = Describes someone or something<br />
        Adverb = How something is done (ends in 'ly' like loudly)<br />
        Noun = Name of a person, place or thing<br /><br />
</div>			
<div>
    Here we go! Fill in all of the blanks.
</div>
<table border="1" style="width:25%">
	<tr>
		<td> Mythical creature:
			<input type="text"  id="input0" size="15">
		</td>
	</tr>
	<tr>
			<td> Mythical creature: 
				<input type="text" id="input1" size="15">
			</td>
  </tr>
   <!--in progress <tr>
			<td> Noun:
				<input type="text" name="noun[0]" size="15">
			</td>
  </tr>
   <tr>
			<td> Noun:
				<input type="text" name="noun[0]" size="15">
			</td>
  </tr>
   <tr>
			<td> Color:
			<input type="text" name="noun[0]" size="15">
			</td>
  </tr>
   <tr>
			<td> Color:
			<input type="text" name="noun[0]" size="15">
			</td>
  </tr>
  <tr>
			<td> Person:
			<input type="text" name="noun[0]" size="15">
			</td>
  </tr>
	<tr>
			<td> Person:
			<input type="text" name="noun[0]" size="15">
			</td>
  </tr>
<tr>
			<td> Body part:
			<input type="text" name="noun[1]" size="15">
				</td>
  </tr>
   <tr>
			<td> Body part:
			<input type="text" name="noun[1]" size="15">
			</td>
  </tr>
  <tr>
			<td> Adjective:
			<input type="text" name="adj[0]" size="15">
			</td>
  </tr>
   <tr>
			<td> Adjective:
			<input type="text" name="adj[]" size="15">
			</td>
  </tr>
   <tr>
			<td> Adjective:
			<input type="text" name="adj[]" size="15">
			</td>
  </tr>
   <tr>
			<td> Adjective:
			<input type="text" name="adj[]" size="15">
			</td>
  </tr>
  <tr>
			<td> Adjective:
			<input type="text" name="input7" size="15">
			</td>
  </tr>
  <tr>
			<td> Adverb:
			<input type="text" name="adv[]" size="15">
			</td>
  </tr>
   <tr>
			<td>Adverb:
			<input type="text" name="adv[]" size="15">
			</td>
  </tr>
   <tr>
			<td>Adverb:
			<input type="text" name="adv[]" size="15">
			</td>
  </tr>  -->
 </table>

<h2>What did you create!</h2>

<button onclick="story1()">View Story 1</button>

<p id="storydisplay"></p>

 <input type="reset" name="reset" onclick="document.location.reload(true)" value="Reset">

</body>
</html>
