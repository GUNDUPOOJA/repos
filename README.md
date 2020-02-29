# repos1
radius to area converter
      <p>  Enter the radius of circle:</p>
       <input type="text" name="txtRadius" size=10></article>
       <br>
       <input type="button" value="Calculate" onClick='CalculateArea();'>  
       JS is 
function CalculateArea(){
    var radius =document.form1.txtRadius.value;
    document.write("<P>The area of the circle is " + (radius * radius * Math.PI) + "</p>");
    document.write("<P>The circumference of the circle is " + (2 * radius * Math.PI) + "</p>")
}
## miles to kilometers converter
<html>
<head>
<title>Find the area and circumference of a circle</title>
<script src=main.js></script>
</head>
<body>
    <main style="text-align: center;">
    <h2>Convert miles to kilometers</h2>
    <h3>Enter Miles :</h3>  <input id="c" type="text">
 </br>
</br>
<h3>kilometers :</h3><input type="text" id="d" readonly="true">
</br>
</br>
<button type="button" id="convert" onclick="convertkms()">Convert</button>
 </main> 
 </body>
</html> 
JS is : 
function convertkms() {
    if (document.getElementById("c").value != " ") {
    var f = document.getElementById("c").value * 1.6;
      document.getElementById("d").value = Math.round(f);
    } else {
      
      document.getElementById("d").value = "please enter the miles in above textbox";
    }
  }
##Grams to Kilograms converter
<!DOCTYPE html>
<html lang="en">
<meta charset="UTF-8" />
<link rel="stylesheet" href="gundu.css">
<title>Grams to Kilograms Weight Converter</title>
<body>
  <h2>Weight Converter</h2>
  <div>
  </div>
  <br>
  <br>
  </br>
  </div>
  <div><label>Grams</label>
    <input id="inputGrams" type="number" placeholder="Grams" oninput="weightConverter(this.value)"
      onchange="weightConverter(this.value)">
    <br>
    <div><label>Kilograms</label>
      <span id="outputKilograms"></span></div>
  </div>
  </main>
  JS is : 
function weightConverter(valNum) {
    document.getElementById("outputKilograms").innerHTML=valNum/1000;
  }
 CSS for above is 
body{
    flex-basis: 100%;
    font-family:Arial, Helvetica, sans-serif;
    display : flex;
    flex-wrap : wrap;
    justify-content: center;
    color : blue;
    
     text-align: vertical;
   }
   
 
 
 h2{
   text-align: center;
   color: darkkhaki;
   flex-basis: 100%;
 
   
 }
 #inputGrams{
    padding: 9px;
    border-radius: 10px;
    box-sizing: border-box;
    color: green;
    text-transform: capitalize;
    text-align: left;
    flex-basis: 100%;
    margin-left: 0;
 
 }
 #outputkilograms{
    padding: 9px;
    border-radius: 10px;
    box-sizing: border-box;
    color: green;
    text-transform: capitalize;
    text-align: center;
    flex-basis: 100%;
    margin-left: 0;
 }
 
 p{
 
   margin-left: left;
    display: ruby-base-container;
    text-align:center;
    display: flex;
    flex-direction: column;
    flex-wrap: no-wrap;
 }
 
  







































