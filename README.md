<!DOCTYPE html > 
<html> 
    <head></head>      
    <body onload="loadbody()"> 
        <form onsubmit = "load()"> 
            <h1 id="d" onclick="click1()">REGISTRATION FORM</h1>
            First Name:<input type = "text" value = "" id="fname" onblur="blur1()"><br><br>
            Qualification:
               <select onchange="Change(this)">
                  <option value="SSLC" />SSLC
                  <option value="Plus Two" />Plus Two
                  <option value="Degree" />Degree
               </select><br><br>
            <input type = "submit" value = "Submit"> 
        </form> 
      <script type="text/javascript">   
            function loadbody() {
                 alert("Registration Form");
            }
            function click1() {
                  document.getElementById("d").style.color = "red";
            } 
            function blur1() {
                 var x = document.getElementById("fname");
                 x.value = x.value.toUpperCase();
            }
            function Change(select){
                 var selectedOption = select.options[select.selectedIndex];
                 alert ("Qualification is " + selectedOption.value);
            } 
            function load() { 
                alert("Form submitted successfully.") ; 
            } 
        </script >  
    </body> 
</html> 
