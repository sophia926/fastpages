---
title: Food Ratings
comments: true
layout: base
permalink: /java/foodratings
description: This program allows you to increase the rating of a food.
categories: [week5]
---

{% include nav_javascript.html %}
<html> 
<head>
    <style type="text/css">
    body {margin: 30px;}
    </style> 
</head>
<body>
<h1>Here is a food table made by Sophia Tang!</h1>
<h2>How this works:</h2>
<ol>
<li>Enter the EXACT name of the food on the left column in the "Food" box</li>
<li>Enter a new rating of how you rate the food</li>
<li>Press the "Press to Change Rating!" button and then watch the magic happen!</li>
</oL>

<table>
<thead>
  <tr>
    <th>Food Name</th>
    <th>Cuisine</th>
    <th>Rating (/10)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Noodles</td>
    <td>Chinese</td>
    <td id="NoodlesRating">9</td>
  </tr>
  <tr>
    <td>Pasta</td>
    <td>Italian</td>
    <td id="PastaRating">7</td>
  </tr>
  <tr>
    <td>Pancakes</td>
    <td>American</td>
    <td id="PancakesRating">4</td>
  </tr>
</tbody>
</table>

Food: <input type="text" id="food"/><br>
Rating: <input type="text" id="foodRating"/><br>
<input type="button" onClick="change()" Value="Press to Change Rating!"/>

<script>

    function change() {
        var food = document.getElementById("food").value;
        var foodID = food + "Rating";


        var newRating = parseInt(document.getElementById("foodRating").value);
        console.log(newRating);
        document.getElementById(foodID).innerHTML = newRating;

        // console.log(foodID);
        // var currentRating = parseInt(document.getElementById(foodID).value);
        // console.log(currentRating);
        // var newRating = currentRating + 1;
        // document.getElementById(foodID).innerHTML = newRating;
        // document.getElementById("result").innerHTML = food;
    }

</script>

</body>
</html>