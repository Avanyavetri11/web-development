# web-development
about the Javasript program to handle events
PROCEDURE:  
Step 1: Create a new html file with basic structural tags and save it using .html or html extensions  
Step 2: Under the <head> tag, define a <title> tag with the element contents as webpage title and close  
the <title> and <head> tag using forward slash  
Step 3: Under the <body> tag, define the following:  
I. Use Heading tags and font properties to place necessary captions  
II. Present the information using basic content tag along with choices and additional information using 
list and table tags  
III. Identify the Element using DOM (Id, Class name, Tag name and CSS Selectors)  
IV. Assign and handle events using Inline and event handler and listener  
V. Add Event Listener method to watch the event of an element  
Step 4: Close all the structural tags  
Step 5: Execute the web page 


events:
  mouseover event 
  keybord event 
  form event 

code:
mouseover event :
<!DOCTYPE html> 
<html lang="en"> 
<head> 
<meta charset="UTF-8"> 
<meta http-equiv="X-UA-Compatible" content="IE=edge"> 
<meta name="viewport" content="width=device-width, initial-scale=1.0"> 
<title>Mouse Events in JavaScript</title> 
<style> 
/*         styling the div tag */ 
                div { 
            height: 200px; 
            width: 200px; 
            margin: 10px; 
            padding: 10px; 
            color: yellow; 
            background-color: rgb(212, 17, 17); 
            border: 7px solid black; 
            display: flex; 
            justify-content: center; 
            align-items: center; 
            font-weight: bolder; 
        } 
</style> 
</head> 
<body> 
<div id="add"></div> 
<script> 
        // selecting the div tag with the id 'add' 
        let div = document.getElementById('add'); 
        // adding event listener on the selected div tag 
div.addEventListener('mouseover',(event) => { 
div.innerText = "Mouseover event is fired" 
        }); 
</script> 
</body></html>


keyboard event :
<!DOCTYPE html>   
<html>   
<head>   
<title> keydown function in javascript </title>   
<style>   
#datas {   
color: green;   
}   
</style>   
</head>   
<body>   
<h2> JavaScript keydown Method </h2>   
<p><div id = "demoDIV" >   
The javascript key
down event works after pressing the key and key in the down position on the specific tag.</div></body></p> 
</div>   
<input type = "text" id = "input_class" placeholder = "write here." onkeydown = "keyDownFunction
 ()">   
<p id = "datas"> </p>   
<script>   
function keyDownFunction() {   
alert("JavaScript keyDown function activates successfully!!!");   
document.getElementById("datas").innerHTML = "JavaScript keyDown function activates successf
 ully!!!";   
}   
</script>   
</body>   
</html>   


form event :
<!DOCTYPE html> 
<html> 
<body> 
<label for="country">Select a country:</label> 
<select id="country" onchange="handleChange()"> 
<option value="USA">USA</option> 
<option value="Canada">Canada</option> 
<option value="UK">UK</option> 
<option value="India">India</option> 
</select> 
<p id="txt"></p> 
<script> 
      function handleChange() { 
         // Perform actions when the dropdown selection changes 
         var selectedCountry = document.getElementById('country').value; 
document.getElementById("txt").textContent= 
   "Selected country: "+selectedCountry; 
     } 
</script> 
</body> 
</html>
