<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Valentine</title>

<style>

body{
    background: linear-gradient(135deg,#ffd6e7,#ffeef5);
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    font-family: Arial, Helvetica, sans-serif;
    overflow:hidden;
}

/* CARD */

.card{
    background:white;
    padding:30px;
    border-radius:20px;
    text-align:center;
    width:320px;
    box-shadow:0 10px 30px rgba(0,0,0,0.1);
    position:relative;
}

img{
    width:45%;
    border-radius:15px;
    margin-bottom:15px;
}

h1{
    font-size:22px;
}

/* BUTTONS */

button{
    padding:10px 22px;
    border-radius:25px;
    border:none;
    cursor:pointer;
    font-size:16px;
    margin:10px;
    transition:.3s;
}

#yes{
    background:#ff4d8d;
    color:white;
}

#yes:hover{
    transform:scale(1.1);
}

#no{
    background:white;
    border:2px solid #ff4d8d;
    position:absolute;
    left:50%;
    top:70%;
    transform:translateX(-50%);
}

</style>
</head>

<body>

<div class="card" id="card">

    <img src="angel.jpeg" alt="image">

    <h1 id="question">Will you be my Valentine? ❤️</h1>

    <button id="yes">Yes 💕</button>
    <button id="no">No 🙅</button>

</div>

<script>

// YES CLICK
document.getElementById("yes").onclick = function(){
    document.getElementById("card").innerHTML = `
        <img src="angel.jpeg" alt="image">
        <h1>I knew you'd say yes! 😍</h1>
        <p>And yet they say I got no angel 😎</p>
    `;
}

// CLICK-ONLY MOVEMENT FOR NO BUTTON
const noBtn = document.getElementById("no");
const card = document.querySelector(".card");

// Move function
function moveNoBtn() {
    const maxX = card.clientWidth - noBtn.offsetWidth;
    const maxY = card.clientHeight - noBtn.offsetHeight;

    const x = Math.random() * maxX;
    const y = Math.random() * maxY;

    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
}

// Gagalaw lang kapag na-click
noBtn.addEventListener("click", (e) => {
    e.preventDefault();
    moveNoBtn();
});

</script>

</body>
</html>
