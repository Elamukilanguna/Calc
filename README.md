# Ex.08 Design of a Standard Calculator
## Date:21/12/2023

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
~~~
calc.html

<!DOCTYPE html>
<html lang="en">
    <head>
        <title>CALCULATOR </title>
        
        <script>
        function calculate(args)
        {
            res = document.getElementById("result");
            expression = res.innerText;
            cmd = args.srcElement.innerText;
            if(cmd == "=")
            {
                expression = "" + eval(expression)
            }
            else if(cmd == "C")
            {
                expression=""
            }
            else if(cmd == "DEL")
            {
                expression = expression.slice(0, -1);

            }
            else if(cmd == "√")
            {
                expression = "" + Math.sqrt(eval(expression));
            }
            else if(cmd == "%")
            {
                expression = expression % 1;
            }
            else if(cmd == "log")
             {
        expression = Math.log10(expression);
           }
       
            else{
                expression = expression + cmd;
            }
            res.innerText = expression;
            

        }
         
        </script>

        <style>
          
            .calculator-container {
                width: 550px;
                background-color:rgb(196, 18, 152);
                margin: 0 auto; 
                margin-top: 120px;
                text-align: center;
                
            }

           
            button {
                width: 60px;
                height: 60px;
                margin: 10px; 
                font-size: 20px; 
                
                background-color: rgb(16, 216, 72); 
                color: white; 
                border: black;
            }

          
            #result {
                
       background-color:#ABFFBA;
    text-align: right;
    padding-right: 90px;
    font-size: 25px;
    margin-bottom: 25px; 
    border: solid black 0.8px;
    color: blue;
    width: 410px;
    height: 55px;
    display: flex;
    align-items: center;
    justify-content: flex-end;

            }
            h1 {
                padding-top: 10px;
                color:white;
                font-size: 50px;
            }
            .redd {
                background-color: blue;
            }
            .bluee {
                
                background-color: cornflowerblue;
            }
            body {
                background-color: rgb(247, 240, 240);
            }
        </style>

    </head>
<body>
    <div class="calculator-container">
        <h1>ELAMUKILAN.G</h1>
        <h2>REGISTER NO.:23003756</h2>
        <div id="result">0.</div>
        <button onclick="calculate(event);">7</button>
        <button onclick="calculate(event);">8</button>
        <button onclick="calculate(event);">9</button>
        <button class="bluee"  onclick="calculate(event);">/</button>
        <button class="bluee"  onclick="calculate(event);"> DEL </button><br>
        <button onclick="calculate(event);">4</button>
        <button onclick="calculate(event);">5</button>
        <button onclick="calculate(event);">6</button>
        <button class="bluee"  onclick="calculate(event);">*</button>
        <button class="bluee"  onclick="calculate(event);">&radic; </button><br>
        <button onclick="calculate(event);">1</button>
        <button onclick="calculate(event);">2</button>
        <button onclick="calculate(event);">3</button>
        <button class="bluee"  onclick="calculate(event);">-</button>
        <button class="bluee"  onclick="calculate(event);">log</button><br>
        <button onclick="calculate(event);">0</button>
        <button onclick="calculate(event);">.</button>
        <button class="redd" onclick="calculate(event);">C</button>
        <button class="bluee"  onclick="calculate(event);">+</button>
        <button class="bluee" onclick="calculate(event);">=</button><br>
    </div>
    </body>
</html>

~~~

## OUTPUT:
![Screenshot (37)](https://github.com/Elamukilanguna/Calc/assets/144870462/92fd4adb-7acc-49f6-9e75-1d2ec3bdefa
![Screenshot (38)](https://github.com/Elamukilanguna/Calc/assets/144870462/dd89d2d0-607e-44cb-8c93-58565317c37c)


## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
