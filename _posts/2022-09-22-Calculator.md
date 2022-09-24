---
title: Less than or Greater Than
comments: true
layout: default
permalink: /java/calculator
description: This program checks if a number is greater or less than a number.
categories: [week5]
---

{% include nav_javascript.html %}
<html> 
<head>
    <title>JavaScript program to calculate multiplication and division of two numbers </title>
    <style type="text/css">
    body {margin: 30px;}
    </style> 
</head>
<body>

<form>
    <h1>Here is a simple calculator made by Sophia Tang!</h1>
    <mark>Enter two numbers in the following boxes, and then you can perform calculations :)<br></mark>
    1st Number: <input type="text" id="firstNumber" /><br>
    2nd Number: <input type="text" id="secondNumber" /><br>
    <input type="button" onClick="multiplyBy()" Value="Multiply"/>
    <input type="button" onClick="divideBy()" Value="Divide"/>
    <input type="button" onClick="subtract()" Value="Subtract"/>
    <input type="button" onClick="add()" Value="Add"/>
</form>
    <p>The Result is: <br>
    <span id = "result"></span>
</p>


<script>
    function multiplyBy() {
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result").innerHTML = num1 * num2;
    }
    function divideBy() { 
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result").innerHTML = num1 / num2;
    }
    function subtract() {
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result").innerHTML = num1 - num2;
    }
    function add() { 
        num1 = parseInt(document.getElementById("firstNumber").value);
        num2 = parseInt(document.getElementById("secondNumber").value);
        document.getElementById("result").innerHTML = (num1 + num2);
    }
</script>

</body>
</html>