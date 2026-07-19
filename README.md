<!DOCTYPE html>
<html lang="my">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Ko Ko ❤️</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:Arial,sans-serif;
background:linear-gradient(135deg,#ff9ecf,#ffd6e8);
overflow:hidden;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
color:white;
}

#loading{
position:fixed;
width:100%;
height:100%;
background:#ff7aa8;
display:flex;
justify-content:center;
align-items:center;
font-size:35px;
z-index:9999;
animation:hideLoading 3s forwards;
}

@keyframes hideLoading{
0%{opacity:1;}
80%{opacity:1;}
100%{
opacity:0;
visibility:hidden;
}
}

.card{
display:none;
padding:30px;
animation:fade 2s forwards;
}

@keyframes fade{
from{
opacity:0;
transform:translateY(30px);
}
to{
opacity:1;
transform:translateY(0);
}
}

h1{
font-size:40px;
margin-bottom:20px;
}

p{
font-size:22px;
line-height:1.8;
}
button{
margin-top:30px;
padding:15px 30px;
font-size:20px;
border:none;
border-radius:50px;
background:#ff3d7f;
color:white;
cursor:pointer;
}
button:hover{
background:#ff0055;
}
</style>
</head>

<body>

<div id="loading">
❤️ Loading...
</div>

<div class="card" id="main">

<h1>🎂 Happy Birthday<br>ကိုကို ❤️</h1>

<p>
ဒီ Page လေးက<br>
ကိုကိုတစ်ယောက်တည်းအတွက်ပါ။ 💖
</p>

<button onclick="nextPage()">
Open My Heart 💌
</button>

</div>

<script>

setTimeout(()=>{
document.getElementById("main").style.display="block";
},3000);

function nextPage(){
alert("ဆက်လက် Surprise တွေရှိသေးတယ် ❤️");
}

</script>

</body>
</html>
