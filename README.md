<html>
<meta charset='UTF-8' /><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport' /><meta content='IE=edge' http-equiv='X-UA-Compatible' /><link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Shippori+Antique&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script><link href="https://semangat.likeadream.repl.co/style.css" rel="stylesheet" type="text/css" />
<head>
    <title>Happy Birth Day</title>
</head>
<body>
<style>
body{background-image: url("https://i.postimg.cc/mgFWyKXc/IMG-20211212-081951-825.jpg");background-repeat: no-repeat;background-size: 105% 105%;animation:none;transition:all .3s ease;}
</style>
<div id="bodyblur"></div>
<div id="konten">
<div id="fotoloveu"><div class="image">
<img id="animasi" src="https://i.postimg.cc/7hQjgNSM/wing.gif" width="100px" height="100px" /></div><span id="sp2"></span><span id="sp3"></span></div>

<div id="ftawal"><div class="image">
<img src="https://i.postimg.cc/1tYFjC4j/rain-together.gif" width="100px" height="100px" /></div></div>
<div id='subkonten'>
<p data-text='&#9829;' class='catatan sek' onClick='expl();'>
<marquee id="marq">
Hii <b id="kamu"></b> 🦆 <i id="spasi"></i>
Happy~Birth Day! ❤️ I Miss You &#129402;<i id="spasi"></i>
I -Wish Your Birth-Day To Be Full Of Enjoy🥳 & Happiness😀... &#129321;<i id="spasi"></i>
Get Up Cuty & Give This day A Head Start.. &#129303;<i id="spasi"></i>
Your 😍Presence in my life means the worlds to me. <i id="spasi"></i>
Once Again A Very Happy & Blooming Birthday To The Girl Who Filled My Heart With Lots Of Smile. &#128525;</marquee>
</p>
</div>
<br> <br> <br> <br> <br> <br> <br>
<div id="tombWA"><a class='button whatsapp' onClick='bukaWa();'><i class='icon whatsapp'></i>
Somu</a></div>
</div>
<script> 
//Teks klik love
var a=0,finish;
finish = "Happy Birth Day😍";
//Teks klik love
var i=0,finish2;
finish2 = "Some Says That One-Sided Love is Better Than none, But Like Half A Loaf Of Bread, It Is Likely To Grow Hard & moldy Sooner❤️";  
function play() {
//Link Audio Bisa Diganti
  var audio = new Audio('https://lv3000.likeadream.repl.co/musik.mp3');audio.play();
  audio.loop=true;audio.addEventListener('ended', function() {this.currentTime = 0;this.play();}, false);
}         

//Pesan WhatsApp


 function bukaWa(){window.location = "https://api.whatsapp.com/send?phone=&text=" + window.nama + ":- Say Something Something" + "%0A%0A" + "- " + dateTime;} 
</script>
<script type="text/javascript">            
            var today = new Date();var date = today.getDate()+'/'+(today.getMonth()+1)+'/'+today.getFullYear()+'.';var dateTime = date;
            const swals = Swal.mixin({
                allowOutsideClick: false,
            });
            async function mulai(){
                var { value: nama } = await swals.fire({
                    title: 'Your Name🤔?',
                    input: 'text' ,
                    confirmButtonText: 'Next',
                    showCancelButton: false,
                });                           
                if(nama){
                	window.nama = nama;
                    finish = finish + ", " + nama + "!";    
                    document.getElementById("kamu").innerHTML = "" + window.nama;                      
                    await swals.fire(`Happy Birth Day &#10084;&#65039;`);
                    setTimeout(showDiv, 100);play();                                    
                } else {
                    await swals.fire('Nama tidak boleh kosong, ya!');
                    mulai();
                }
            }            
            mulai();
</script>
<script>
  function showDiv() {StartMarquee();document.getElementById('subkonten').style.opacity = "1"; document.getElementById('konten').style.top = "0";document.getElementById('ftawal').style.opacity = "1";document.getElementById('ftawal').style.height = "100px";document.querySelector("body").style.animation = "fanim 9s ease infinite";}
  function tombol() {document.getElementById('tombWA').style.visibility = "visible";document.getElementById('tombWA').style.opacity = "1";}  

async function duar(){
var e1 = document.getElementById('animasi');e1.classList.add("degdeg");
duar2();setInterval(createHeart,200);
document.body.style.backgroundColor = "#000";
document.getElementById('ftawal').style.opacity = "0";document.getElementById('ftawal').style.height = "0";
document.getElementById('fotoloveu').style.opacity = "1";document.getElementById('fotoloveu').style.height = "120px";document.getElementById('fotoloveu').style.margin = "50px 0 0 0";
document.getElementById('subkonten').style.display = "none";
}
function duar2(){
if(a<finish.length){document.getElementById("sp2").innerHTML += finish.charAt(a);a++;setTimeout(duar2,100);}
if(a==finish.length){duar3();}
}
function duar3(){
if(i<finish2.length){document.getElementById("sp3").innerHTML += finish2.charAt(i);i++;setTimeout(duar3,200);}
if(i==finish2.length){setTimeout(tombol,1000);}
}

async function expl(){document.getElementById('bodyblur').style.opacity = "1";document.getElementById('bodyblur').style.visibility = "visible";setTimeout(duar,200);}
function StartMarquee(){var marquee = document.getElementById ("marq");marquee.start();}
function StopMarquee(){var marquee = document.getElementById ("marq");marquee.stop();}
StopMarquee();
</script>
<script>
const body = document.querySelector("body");
function createHeart() {
    const heart = document.createElement("div");
    heart.className = "fas fa-heart";
    heart.style.left = (Math.random() * 90)+"vw";
    heart.style.animationDuration = (Math.random()*3)+2+"s"
    body.appendChild(heart);
}
setInterval(function name(params) {
    var heartArr = document.querySelectorAll(".fa-heart")
    if (heartArr.length > 100) {
       heartArr[0].remove()
    }
},100)
</script>
</body>
</html>
