# Ex.08 Design of a Standard Calculator
## Date:

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
Register Number:212223230009
Developed By: AJITHKUMAR A

<title>Calculator</title>
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
            width: 400px;
            background-color:rgb(187, 69, 14);
            margin: 0 auto; 
            margin-top: 100px;
            text-align: center;
            
        }

       
        button {
            width: 50px;
            height: 50px;
            margin: 10px; 
            font-size: 25px; 
            
            background-color: blue; 
            color: black (255, 255, 255); 
            border: none;
        }

      
        #result {
            
   background-color:rgb(211, 218, 8);
text-align: right;
padding-right: 50px;
font-size: 25px;
margin-bottom: 20px; 
border: solid black 0.5px;
color: black;
width: 348px;
height: 50px;
display: flex;
align-items: center;
justify-content: flex-end;

        }
        h1 {
            padding-top: 10px;
            color:rgb(7, 7, 7);
            font-size: 50px;
        }
        .redd {
            background-color:black(244, 240, 240);
            color: rgb(12, 11, 11)
        }
        .bluee {
            
            background-color:rgb(20, 183, 79);
            color: rgb(49, 25, 165) (218, 188, 188);
            font-size: 17px;
        }
        body {
            background-color: palevioletred
        }
    </style>

</head>
~~~
## OUTPUT:
![image](https://github.com/Ajith1413/Calc/assets/139842524/d4b34443-7945-41fd-a41d-77c8b9b6a4c5)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
