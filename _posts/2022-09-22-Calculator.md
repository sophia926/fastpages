---
title: Less than or Greater Than
comments: true
layout: default
description: This program checks if a number is greater or less than a number.
categories: [week5]
---

{% include nav_javascript.html %}

<!doctype html>
<html>
<head>
<script>
function lessThan()
{
  var userVal, compareVal;
  userVal = parseInt(document.getElementById("userNum").value);
  compareVal = parseInt(document.getElementbyId("testNum").value);
  if (userVal<compareVal)
  {
    document.GetElementbyId("result").innerHTML = (userVal, " is less than", compareVal);
  } else{
    document.GetElementbyId("result").innerHTML = (userVal, " is greater than", compareVal);
  }
}
</script>
</head>
<body>

<p>Enter Number A: <input id="userNum">
Enter Number B: <input id="testNum">
<button onclick="lessThan()">Submit</button></p>
<p id="result"></p>

</body>
</html>