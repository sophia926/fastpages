---
title: Binary Operations
layout: default
description: Binary Operations calculator
permalink: /frontend/binaryoperations
categories: [week13]
---

<html> 
<head>
    <title>Binary Operations</title>
    <style type="text/css">
    body {margin: 30px;}
    </style> 
</head>
<body>

<form>
    <h1>Binary Operations by Sophia Tang!</h1>
    <mark>Enter two numbers in the following boxes, and then you can perform binary operations. :)<br></mark>
    1st Number: <input type="text" id="firstNumber"/><br>
    2nd Number: <input type="text" id="secondNumber"/><br>
    <input type="button" onClick="AND()" Value="AND"/>
    <input type="button" onClick="OR()" Value="OR"/>
    <input type="button" onClick="XOR()" Value="XOR"/>
    <input type="button" onClick="ZeroFillLeftShift()" Value="Zero fill left shift"/>
    <input type="button" onClick="SignedRightShift()" Value="Signed right shift"/>
    <input type="button" onClick="ZeroFillRightShift()" Value="Zero fill right shift"/>
</form>
    <p>The Result is: <br>
    <span id = "result2"></span>
</p>


<script>
    function AND() {
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result2").innerHTML = num1 & num2;
    }
    function OR() {
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result2").innerHTML = num1 | num2;
    }
    function XOR() {
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result2").innerHTML = num1 ^ num2;
    }
    function ZeroFillLeftShift() {
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result2").innerHTML = num1 << num2;
    }
    function SignedRightShift() {
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result2").innerHTML = num1 >> num2;
    }
    function ZeroFillRightShift() {
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result2").innerHTML = num1 >> num2;
    }
</script>

</body>
</html>