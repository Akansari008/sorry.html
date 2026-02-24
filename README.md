<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Forgive Me Kausar ❤️</title>

<style>
body {
    margin: 0;
    padding: 0;
    background: linear-gradient(to right, #ff758c, #ff7eb3);
    font-family: 'Segoe UI', sans-serif;
    text-align: center;
    color: white;
    overflow: hidden;
}

.container {
    position: relative;
    top: 15%;
}

h1 {
    font-size: 45px;
    animation: fadeIn 2s ease-in-out;
}

p {
    font-size: 20px;
    width: 75%;
    margin: auto;
    margin-top: 20px;
    animation: fadeIn 4s ease-in-out;
}

.buttons {
    margin-top: 40px;
}

button {
    padding: 12px 25px;
    font-size: 18px;
    border: none;
    border-radius: 25px;
    cursor: pointer;
    margin: 10px;
    transition: 0.3s;
}

#yesBtn {
    background-color: white;
    color: #ff4e8a;
}

#yesBtn:hover {
    background-color: #ff4e8a;
    color: white;
}

#noBtn {
    background-color: black;
    color: white;
    position: absolute;
}

@keyframes fadeIn {
    from {opacity: 0;}
    to {opacity: 1;}
}

.heart {
    position: absolute;
    color: red;
    font-size: 20px;
    animation: float 6s linear infinite;
}

@keyframes float {
    0% {transform: translateY(100vh);}
    100% {transform: translateY(-10vh);}
}
</style>
</head>
<body>

<div class="container">
    <h1>Kausar, Please Forgive Me ❤️</h1>
    <p>
            My Dearest Wife,<br><br>
            I know I made a mistake and I hurt you. For that, I am deeply sorry.
            You are the most precious person in my life, and seeing you upset
            hurts me more than anything else.
        </p>
        <p>
            Please forgive me for my words and actions. I promise to learn,
            to grow, and to become a better husband for you. Our relationship
            means everything to me, and I never want to lose your smile.
        </p>
        <p>
            Thank you for loving me, supporting me, and standing beside me.
            I am blessed to call you my wife.    
    </p>
    <div class="buttons">
        <button id="yesBtn" onclick="forgive()">YES 💖</button>
        <button id="noBtn" onmouseover="moveButton()">NO 😜</button>
    </div>
</div>

<script>
function forgive() {
    alert("Yayyy ❤️ Kausar forgave me! I love you forever 😘");
}

function moveButton() {
    var button = document.getElementById("noBtn");
    var x = Math.random() * (window.innerWidth - 100);
    var y = Math.random() * (window.innerHeight - 50);
    button.style.left = x + "px";
    button.style.top = y + "px";
}

function createHeart() {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.animationDuration = (Math.random() * 3 + 3) + "s";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 6000);
}

setInterval(createHeart, 300);
</script>

</body>
</html>
