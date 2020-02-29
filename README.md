# radius to area converter
      <p>  Enter the radius of circle:</p>
       <input type="text" name="txtRadius" size=10></article>
       <br>
       <input type="button" value="Calculate" onClick='CalculateArea();'>  
       
   JS is-----
function CalculateArea(){
    var radius =document.form1.txtRadius.value;
    document.write("<P>The area of the circle is " + (radius * radius * Math.PI) + "</p>");
    document.write("<P>The circumference of the circle is " + (2 * radius * Math.PI) + "</p>")
}
---------------------
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
JS is -----
function convertkms() {
    if (document.getElementById("c").value != " ") {
    var f = document.getElementById("c").value * 1.6;
      document.getElementById("d").value = Math.round(f);
    } else {
      
      document.getElementById("d").value = "please enter the miles in above textbox";
    }
  }
  -----------------------
## Grams to Kilograms converter
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
  
 JS is ---- 
function weightConverter(valNum) {
    document.getElementById("outputKilograms").innerHTML=valNum/1000;
  }
 CSS for above is -----
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
 -------------------
 ## fahrenheit to celsius converter
 <!DOCTYPE html>
<html lang="en">

<head>
    <title> APP CHALLENGE</title>
    <meta charset="UTF-8" />
    <link rel="stylesheet" href="gundu.css">
    <script src="main.js"></script>
</head>

<body>
    <h1 style=text-align:center>CONVERTER</h1>
    <br></br>
  
  </div>
     <main>
       <br>
       <br>
       <div>
         <br>
       </br>
    
  <br>
  <br>
    <h2 style=text-align:center>JavaScript Celsius to Fahrenheit </h2>
    <p><input id="c" onkeyup="convert('C')"> degrees Celsius</p>
    <p><input id="f" onkeyup="convert('F')"> degrees Fahrenheit</p> 
       <body>
    </html>
    ## JS is ---
    function convert(degree) {
    var x;
    if (degree == "C") {
      x = document.getElementById("c").value * 9 / 5 + 32;
      document.getElementById("f").value = Math.round(x);
    } else {
      x = (document.getElementById("f").value -32) * 5 / 9;
      document.getElementById("c").value = Math.round(x);
    }
  }
-------------------------------
## pounds to kilograms
  <h2> Weight Converter</h2>
    <p> Type a value in the pounds field to convert the value to Kilograms:</p>
    <p>
        <label>Pounds</label>
        <input id="inputPounds" type="number" placeholder="Pounds" oninput=" weightConverter(this.value)"
            onchange="weightConverter(this.value)"
    </p>
    <p>Kilograms: <span id="outputKilograms"></span></p>
    <footer>
        <p class="footerText">This site was coded by Gundu pooja</p>
    </footer>
    JS IS ------
    <script>
        function weightConverter(valNum) {
            document.getElementById("outputKilograms").innerHTML = valNum / 2.2046;
        }
    </script>
    -----------------------------------
    ## TAKING USERINPUT AND PASSWORD
  <!DOCTYPE html>
<html>
<body>

<h2>Password field</h2>

<p>The <strong>input type="password"</strong> defines a password field:</p>

<form action="/action_page.php">
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>
  <label for="pwd">Password:</label><br>
  <input type="password" id="pwd" name="pwd"><br><br>
  <input type="submit" value="Submit">
</form>

<p>The characters in a password field are masked (shown as asterisks or circles).</p>

</body>
</html>

## MAITRE D APP CHALLENGE

<!DOCTYPE html>
<html lang="en">
<head>
    <title> Maitre D Practice App Gundu pooja</title>
    <meta charset = "UTF-8"/>
    <link rel = "stylesheet" href= "gundu.css">
</head>
<body>
  <h1 style="font: size 50px",align="center">Maitre D</h1>
  <br></br>

</div>
   <main>
     <br>
     <br>
     <div>
       <br>
     </br>
  <div> <label>Total : </label>
 <input id = "total-field" type= "text" placeholder= "input total" value= ""></div>
<br>
<div><label>Rate:</label>
<input id ="rate-field" type ="field-rate" placeholder="input rate" value=""></div>
<br>
</div><label>Tip: </label><span id = "Tip">$0.00</span></div>
</br>
<br>
<div><label>Tax: </label><span id ="Tax">$0.00</span></div>
</br>

<div></label>Grand Total: </label><span id ="Total"> $0.00</span></div>
<br>

<button id="calc-Button">Calculate</button>

<br>
<br>
</main>
<script src = "main.js"></script>
</div>

</body>
</html>
JS-------------
function app()
{
     const Total = parseFloat(document.querySelector('#total-field').value)
     const Rate = parseFloat(document.querySelector('#rate-field').value)
     console.log(Rate);
     const Tip = Total*(Rate/100)
     const TaxRate = 5.5
     const Tax = Total*(TaxRate/100)
     const GrandTotal = Total +Tip + Tax;
     document.querySelector('#Tip').innerHTML =`$${Tip.toFixed(2)}`
     document.querySelector('#Tax').innerHTML=`$${Tax.toFixed(2)}`
     document.querySelector('#Total').innerHTML=`$${GrandTotal.toFixed(2)}`
}
     document.querySelector('#calc-Button').addEventListener('click',app)
    CSS --------------------
    body{
   flex-basis: 100%;
   font-family:Arial, Helvetica, sans-serif;
   display : flex;
   flex-wrap : wrap;
   justify-content: center;
   color : blue;
    background-image: url(https://files.123freevectors.com/wp-content/original/112575-plain-white-blurred-background-vector.jpg);
    height: 100%;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  


h1{
  text-align: center;
  color: darkkhaki;
  flex-basis: 100%;

  
}
#total-field {
 padding: 9px;
 border-radius: 10px;
 box-sizing: border-box;
 color: green;
 text-transform: capitalize;
 text-align: center;
 flex-basis: 100%;

}
#rate-field{
   text-align: center;
  padding: 9px;
  border-radius: 10px;
  box-sizing: border-box;
  color : green;
  flex-basis: 100%;

}

#calc-Button{

  padding: 2px;
  border-radius: 0px;
  box-sizing: border-box;
  color : saddlebrown;
  background-color: cornsilk;
  flex-basis: 5%;
}
------------------------------------------------------















  







































