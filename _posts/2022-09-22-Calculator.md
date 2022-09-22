---
title: Less than or Greater Than
comments: true
layout: default
permalink: /java/calculator
description: This program checks if a number is greater or less than a number.
categories: [week5]
---

{% include nav_javascript.html %}

<!doctype html>
<html>
<head>
<meta charset="utf-8">
</head>
<body>

<p>Enter Number A: <input id="userNum"></p>
<p>Enter Number B: <input id="testNum"></p>
<button type="button" onclick="lessThan()">Submit</button>
<p id="a">Value A: </p>
<p id="b">Value B: </p>
<p id="result">hello</p>
<script>
function lessThan() {
  var userVal, compareVal;
  userVal = parseInt(document.getElementById("userNum").value);
  compareVal = parseInt(document.getElementbyId("testNum").value);
  document.GetElementbyId("a").innerHTML = (userVal);
  document.GetElementbyId("b").innerHTML = (compareVal);
  if (userVal<compareVal)
  {
    document.GetElementbyId("result").innerHTML = (userVal, " is less than", compareVal);
  } else{
    document.GetElementbyId("result").innerHTML = (userVal, " is greater than", compareVal);
  }
}
</script>

</body>
</html>