<DOCTYPE html>  
<html>
<head>
justify-contentlaylay {
display: flex;

justify-content: centeheadn-items: center;

height: 100vh;

background: radial-gradient(circle,

#2802d3,margincfa);

margin:0;

font-family: 'Courier New', monospace;

}

.clock-container {

background-color:

☐ black;

border: 2px solid ☐ rgba(228, 9, 9, 0.904);

padding: 30px 60px;

border-radius: 100px;

box-shadow: 0 0 25px rgba(255, 251, 0, 0.829); 

}

#digitalClock

color: #f3d111;

font-size: 4em;

text-shadow: 0 0 15px

#ffffff;

letter-spacing: 15px;

<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Digital Watch</title>

<link rel="stylesheet" href="style.css">

</head>

<body>

<div class="clock-container">

| <div id="digitalClock">00:00:00</div>

</div>

<script src="script.js"></script>

</body>

</html>

Function updateClock(){

const now = new Date();

let hours = now.getHours();

let minutes = now.getMinutes();

let seconds = now.getSeconds();

// Add leading zeros

hours = hours < 10 ? "0" + hours: hours;

minutes = minutes < 10 ? "0" + minutes : minutes;

seconds seconds < 10 ? "0" + seconds: seconds;

const timeString = '${hours}:${minutes}:${seconds}`;

document.getElementById("digitalClock").textContent = timeString;

// Update every second

setInterval(updateClock, 1000);

updateClock(); // initial call 
