<!DOCTYPE HTML>
<html>
<head>
<title> Date & Time </title>
</head>
<body style="background-color:white">
<h1> Date: (MM/DD/YYYY) </h1>
<p> The current date is <span id="datetime"></span> </p>
<script>
var dt = new Date();
document.getElementById("datetime").innerHTML = dt.toLocaleDateString();
</script>
<div> </div>
<h1> Date: (DD.MM.YYYY) </h1>
<p> The current date is <span id="date2"></span> </p>
<script>
var dt = new Date();
document.getElementById("date2").innerHTML = (("0"+dt.getDate()).slice(-2)) +":"+(("0"+(dt.getMonth()+1)).slice(-2)) +"."+(dt.getFullYear())
</script>
<div> </div>
<h1> Time: </h1>
<p> The current time is <span id="time"></span> </p>
<script>
var dt = new Date();
document.getElementById("time").innerHTML = dt.toLocaleTimeString();
</script>
<div> </div>
<button onClick="history.go(0);">Refresh Page</button>
</body>
</html>
