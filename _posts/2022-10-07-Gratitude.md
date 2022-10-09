---
title: Gratitude Questions
comments: true
layout: default
permalink: /api/gratitude
description: This program asks you some questions to get you thinking about gratitudes.
categories: [week5]
---

{% include nav_api.html %}
<html> 
<head>
    <title>What are you grateful for? </title>
    <style type="text/css">
    body {margin: 30px;}
    </style> 
</head>
<body>

<form>
    <input type="button" onClick="gratitudeGen()" Value="Press to generate a gratitude question! :)"/>
</form>
<p>Gratitude question: <br>
    <span id = "result"></span>
</p>
<form>
    Your answer: <input type="text" id="answer" /><br>
    <input type="button" onClick="gratitudeSubmit()" Value="Submit! :)"/>
</form>
<p>You are grateful for.. <br>
    <span id = "userResponse"></span>
</p>
<p><br>
    <span id = "congrats"></span>
</p>


<script>
    function gratitudeGen() {
        const options = {
            method: 'GET',
            headers: {
                'X-RapidAPI-Key': '222daebd02msh197e0db183672fap17cc9djsn8a1f2f813e5b',
                'X-RapidAPI-Host': 'gratitude-questions.p.rapidapi.com'
            }
        };

        fetch('https://gratitude-questions.p.rapidapi.com/question', options)
            .then(response => response.json())
            // .then(response => console.log(response))
            // .then(response => (question = response))
            .then(response => (document.getElementById("result").innerHTML = response['question']))
            .catch(err => console.error(err));
    }
    function gratitudeSubmit() {
        users = document.getElementById("answer").value;
        document.getElementById("userResponse").innerHTML = users;
        document.getElementById("congrats").innerHTML = "Congrats! You are being grateful, that is good for your mental health!";
    }
</script>

</body>
</html>