
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>I'm Sorry My Love ❤️</title>

<style>

body{
margin:0;
padding:0;
font-family: 'Segoe UI', sans-serif;
background: linear-gradient(270deg,#ff4e50,#ff758c,#ff7eb3);
background-size:600% 600%;
animation:bgMove 10s infinite alternate;
color:white;
text-align:center;
overflow:hidden;
}

@keyframes bgMove{
0%{background-position:left}
100%{background-position:right}
}

.container{
position:absolute;
top:50%;
left:50%;
transform:translate(-50%,-50%);
}

h1{
font-size:40px;
margin-bottom:20px;
}

button{
padding:15px 30px;
font-size:18px;
border:none;
border-radius:30px;
background:white;
color:#ff4e50;
cursor:pointer;
transition:0.3s;
}

button:hover{
transform:scale(1.1);
}

.message{
display:none;
margin-top:30px;
font-size:22px;
line-height:1.6;
}

.heart{
position:absolute;
color:white;
font-size:20px;
animation:fall 6s linear infinite;
}

@keyframes fall{
0%{transform:translateY(-100px)}
100%{transform:translateY(100vh)}
}

</style>
</head>

<body>

<div class="container">

<h1>💔 I'm Sorry Kausar 💔</h1>

<button onclick="showMessage()">Click to Read My Heart</button>

<div class="message" id="msg">
<p>
My dearest wife <b>Kausar Qureshi</b>, ❤️  
</p>

<p>
I know I made a mistake and hurt you.  
But please believe me, hurting you was never my intention.
</p>

<p>
You are the most beautiful part of my life.  
Without you my world feels empty.
</p>

<p>
I truly apologize from my heart.  
Please forgive me and give me one more chance.  
</p>

<p>
Forever yours,<br>
<b>Anwar Ansari ❤️</b>
</p>

</div>

</div>

<script>

function showMessage(){
document.getElementById("msg").style.display="block";
}

function createHeart(){
const heart=document.createElement("div");
heart.classList.add("heart");
heart.innerHTML="❤️";
heart.style.left=Math.random()*100+"vw";
heart.style.animationDuration=(Math.random()*3+3)+"s";
document.body.appendChild(heart);

setTimeout(()=>{
heart.remove();
},6000);
}

setInterval(createHeart,300);

</script>

</body>
</html>
