<div class="card" id="main">

<h1>🎂 Happy Birthday<br>ကိုကို ❤️</h1>

<p>
ဒီ Website လေးက<br>
ကိုကိုတစ်ယောက်တည်းအတွက်<br>
ချစ်လေးရဲ့ နှလုံးသားအပြည့်နဲ့<br>
လုပ်ထားတာပါ... 💖
</p>

<button onclick="nextPage()">
💌 Start My Surprise
</button>

</div>

<div id="letter" style="display:none;padding:25px;font-size:22px;line-height:2;max-width:700px;">

<h2>💖 ကိုကို 💖</h2>

<p id="typing"></p>

</div>
const letter = `

ပျော်ရွှင်သော မွေးနေ့ပါ ကိုကို... 🎂❤️

ဒီ Website လေးကို

ချစ်လေးက

ကိုကိုတစ်ယောက်တည်းအတွက်

ချစ်ခြင်းတွေအပြည့်နဲ့

လုပ်ထားတာပါ။

ကိုကိုနဲ့တွေ့ခဲ့ရတာက

ချစ်လေးဘဝရဲ့

အလှဆုံးကံကောင်းခြင်းပါ။

အသက်က ၁၂ နှစ်ကွာပေမယ့်

ချစ်လေးအတွက်တော့

ကိုကိုက

အနီးဆုံးလူပါ။

ကိုကိုပြုံးရင်

ချစ်လေးလည်းပျော်တယ်။

ကိုကိုပင်ပန်းရင်

ချစ်လေးက

အားပေးချင်တယ်။

မွေးနေ့မှာ

ဆုတောင်းအားလုံး

ပြည့်ပါစေ။

❤️

ချစ်လေး
`;

function start(){

let pass = prompt("🔒 Password ရိုက်ထည့်ပါ");

if(pass!="2909"){
alert("Password မှားနေပါတယ် 💔");
return;
}

document.getElementById("page1").innerHTML = `
<h1>💖 ကိုကို 💖</h1>

<p id="typing"></p>

<br>

<button onclick="finish()">

🎁 Last Surprise

</button>
`;

let i=0;

function type(){

if(i<letter.length){

document.getElementById("typing").innerHTML+=letter.charAt(i);

i++;

setTimeout(type,45);

}

}

type();

}
function finish(){

document.getElementById("page1").innerHTML = `

<h1>🎂 Happy Birthday ❤️</h1>

<h2>ကိုကို</h2>

<p>

ချစ်လေး...

ကိုကိုကို

အရမ်းချစ်တယ်။

Happy Birthday ❤️

Forever & Always

</p>

<br>

<button onclick="location.reload()">

❤️ Read Again

</button>

`;

}

setInterval(()=>{

let heart=document.createElement("div");

heart.className="heart";

heart.innerHTML="❤️";

heart.style.left=Math.random()*100+"vw";

heart.style.animationDuration=(Math.random()*3+3)+"s";

document.body.appendChild(heart);

setTimeout(()=>heart.remove(),7000);

},250);

</script>

</body>

</html>
