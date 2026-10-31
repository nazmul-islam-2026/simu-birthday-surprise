
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Happy Birthday Simu ❤️</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&family=Great+Vibes&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box}
html,body{width:100%;height:100%;overflow:hidden;background:#fff5f7;font-family:'Poppins',sans-serif;-webkit-tap-highlight-color:transparent}
.page{position:fixed;inset:0;display:none;flex-direction:column;align-items:center;justify-content:center;padding:20px 18px;text-align:center}
.page.active{display:flex;animation:fade .5s}
@keyframes fade{from{opacity:0}to{opacity:1}}
.pink{background:linear-gradient(180deg,#ffd6e6 0%,#fff2f6 40%,#fff8d9 100%)}
.hot{background:#ff2e6d}
.badge{border:1.5px solid #ffb6c9;background:#fff;color:#ff4a7a;border-radius:100px;padding:7px 18px;font-size:11px;letter-spacing:1.5px;font-weight:600}
.time{font-size:72px;font-weight:800;color:#ff2e6d;margin:16px 0 6px}
.time small{font-size:22px}
.txt{font-size:14px;line-height:1.6;max-width:340px;color:#333}
.txt b{color:#ff2e6d}
.btn{margin-top:26px;background:linear-gradient(180deg,#ff4a7a,#ff2e6d);color:#fff;border:none;padding:15px 26px;border-radius:100px;font-weight:700;font-size:14px;cursor:pointer;box-shadow:0 14px 32px rgba(255,46,109,.35);min-width:300px;max-width:90vw}
.gift{width:200px;height:122px;background:linear-gradient(180deg,#ff8aa3,#ff4a7a);border-radius:12px;position:relative;cursor:pointer;margin-top:60px;box-shadow:0 20px 40px rgba(255,46,109,.25)}
.gift .lid{position:absolute;top:-22px;left:-10px;right:-10px;height:32px;background:linear-gradient(180deg,#ff9fb5,#ff5a86);border-radius:12px;transition:transform .8s cubic-bezier(.68,-0.55,.265,1.55)}
.gift.open .lid{transform:translateY(-110px) rotate(-25deg) translateX(20px)}
.gift .ribbon{position:absolute;left:50%;top:0;bottom:0;width:18px;background:linear-gradient(#ffe68a,#ffcc33);transform:translateX(-50%)}
.gift .tag{position:absolute;bottom:-30px;left:50%;transform:translateX(-50%) rotate(-2deg);background:#fff;padding:8px 14px;border-radius:10px;font-size:10px;font-weight:700;box-shadow:0 8px 20px rgba(0,0,0,.12);white-space:nowrap;text-align:center}
.heart{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%) scale(0);font-size:44px;transition:transform .6s cubic-bezier(.175,.885,.32,1.275)}
.gift.open .heart{transform:translate(-50%,-140%) scale(1)}
.zoom{position:fixed;inset:0;background:radial-gradient(circle,#ff9fbb,#ff2e6d);display:none;align-items:center;justify-content:center;z-index:99;font-size:100px}
.zoom.show{display:flex;animation:zoom 1.2s forwards}
@keyframes zoom{0%{transform:scale(0)}40%{transform:scale(1.5)}100%{transform:scale(30);opacity:0}}
canvas{position:fixed;inset:0;pointer-events:none;z-index:10}
.cake{width:160px;height:70px;background:#fff;border-radius:18px 18px 10px 10px;position:relative;margin-top:40px;box-shadow:0 0 0 6px #fff,0 20px 40px rgba(0,0,0,.12);cursor:pointer}
.candle{position:absolute;bottom:70px;left:50%;transform:translateX(-50%);width:10px;height:46px;background:#fff;border-radius:6px}
.flame{position:absolute;top:-22px;left:50%;transform:translateX(-50%);width:18px;height:26px;background:radial-gradient(#ffffa0,#ffcc00 45%,#ff6a00);border-radius:50%;box-shadow:0 0 18px #ffcc00;animation:flick .15s infinite alternate}
@keyframes flick{to{transform:translateX(-50%) scale(1.15) rotate(2deg)}}
.balloons{display:flex;gap:12px;margin-top:22px;position:relative}
.b{width:56px;height:72px;border-radius:50% 50% / 60% 60%;box-shadow:inset -6px -8px 10px rgba(0,0,0,.15),0 8px 16px rgba(0,0,0,.12);transition:.4s;position:relative}
.b:after{content:'';position:absolute;bottom:-7px;left:24px;border-left:5px solid transparent;border-right:5px solid transparent;border-bottom:0;border-top:8px solid #ff8aa3}
.b:before{content:'';position:absolute;top:70px;left:27px;height:45px;border-left:1px solid rgba(100,70,80,.4)}
.bow{margin-top:36px;width:72px;height:72px;background:#fff;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:36px;box-shadow:0 12px 28px rgba(0,0,0,.12);cursor:pointer;position:relative;z-index:4}
.card{background:#fff;padding:16px 18px;border-radius:22px;box-shadow:0 14px 36px rgba(0,0,0,.12);max-width:340px;width:90vw;font-size:14px;display:none;margin-top:16px;border:1px solid #ffe1e9;text-align:left}
.ticket{background:#fff;border:2.5px dashed #ff9ab5;border-radius:24px;padding:22px 18px;max-width:360px;width:92vw;box-shadow:0 20px 50px rgba(0,0,0,.1);text-align:left}
.item{display:flex;justify-content:space-between;align-items:center;padding:12px 0;border-bottom:1px solid #fff0f4;font-size:13px}
.del{background:#ff2e6d;color:#fff;font-size:8px;padding:4px 8px;border-radius:20px;font-weight:700;white-space:nowrap}
.letter{background:#fffdf8;border-radius:20px;padding:24px 20px;max-width:380px;width:94vw;max-height:88vh;overflow:auto;text-align:left;box-shadow:0 30px 80px rgba(0,0,0,.5)}

/* NEW ARROW SHOOTING ANIMATION */
.arrow{
 position:fixed;z-index:20;font-size:34px;
 pointer-events:none;display:none;
 filter:drop-shadow(0 3px 5px rgba(0,0,0,.3));
}
.arrow.fly{display:block;animation:arrowFly .65s cubic-bezier(.2,.7,.4,1) forwards}
@keyframes arrowFly{
 0%{transform:translate(0,0) rotate(0) scale(.8);opacity:1}
 75%{opacity:1}
 100%{transform:translate(var(--dx),var(--dy)) rotate(0) scale(1);opacity:1}
}
@keyframes burst{
 0%{transform:scale(1);opacity:1}
 30%{transform:scale(1.5);opacity:1}
 100%{transform:scale(0);opacity:0}
}
.burst{animation:burst .35s forwards}
.heartPop{position:fixed;z-index:30;font-size:28px;pointer-events:none;animation:heartRise 1.1s forwards}
@keyframes heartRise{
 0%{transform:translateY(0) scale(.4);opacity:0}
 30%{opacity:1}
 100%{transform:translateY(-100px) scale(1.5);opacity:0}
}
</style>
</head>
<body>
<canvas id="conf"></canvas>

<div class="page active pink" id="p1">
<div class="badge">✨ 12:00 AM - MIDNIGHT WISH ✨</div>
<div class="time">12:00<small> AM</small></div>
<div class="txt">Raat ke 12 baj gaye 🌙<br>Is khas pal ki shuruat tumhare saath karna chahti thi...<br><b>Yeh dil se ek chota sa surprise sirf Simu ke liye hai ❤️</b></div>
<button class="btn" onclick="go(2)">Happy Birthday My Simu 🎂 ✨<br><span style="font-size:11px;font-weight:400">TAP TO OPEN YOUR MIDNIGHT GIFT 🎁</span></button>
</div>

<div class="page pink" id="p2">
<div style="font-size:10px;letter-spacing:3px;opacity:.6;font-weight:600">A SPECIAL SURPRISE • WITH ALL MY LOVE</div>
<h2 style="font-size:32px;margin-top:14px">A little something for<br><span style="color:#ff2e6d;font-family:'Great Vibes';font-size:38px">My Simu.</span></h2>
<div class="gift" id="gift" onclick="openGift()"><div class="lid"></div><div class="ribbon"></div><div class="tag">TO<br><b>Simu</b><br>WITH ALL MY HEART</div><div class="heart">💖</div></div>
</div>

<div class="zoom" id="zoom">💖</div>

<div class="page hot" id="p3" style="color:#fff">
<h1 style="font-size:46px;font-weight:800;line-height:.9">Happy Birthday<br><span style="font-family:'Great Vibes';color:#ffe27a;font-size:56px;display:block;margin-top:4px">My Simu!</span></h1>
<div class="badge" style="margin-top:18px">WITH ALL MY LOVE</div>
</div>

<div class="page pink" id="p4">
<div class="badge">✨ MAKE A WISH ✨</div>
<h3 style="margin-top:14px">Blow out the candle to celebrate Simu! 🎂</h3>
<p style="font-size:11px;opacity:.6;margin-top:6px">Tap the cake to light & blow out the flame</p>
<div style="position:relative;margin-top:40px"><div class="cake" onclick="doCake()"></div><div class="candle"><div class="flame" id="fl"></div></div></div>
<p id="cmsg" style="margin-top:20px;color:#ff2e6d;font-weight:600;font-size:13px"></p>
</div>

<div class="page pink" id="p5">
<h3>Pop each balloon to reveal a<br><span style="color:#ff2e6d">reason! ✨</span></h3>
<p style="font-size:11px;opacity:.6">Tap the bow below to shoot Cupid's arrow 🏹</p>
<div class="balloons" id="bln"></div>
<div class="card" id="card"></div>
<div class="bow" id="bow" onclick="shoot()">🏹</div>
<button class="btn" id="nxt" style="display:none;min-width:200px;margin-top:18px" onclick="go(6)">Continue →</button>
</div>

<div class="page pink" id="p6">
<div class="ticket">
<div style="text-align:center;font-size:9px;letter-spacing:2px;color:#ff4a7a;font-weight:700">CUPID EXPRESS - WISHES FOR MY SIMU</div>
<div class="item"><div>✨ Endless smiles every day for Simu</div><span class="del">DELIVERED ✓</span></div>
<div class="item"><div>🌙 Peaceful magical moments</div><span class="del">DELIVERED ✓</span></div>
<div class="item"><div>💖 A heart feeling deeply loved</div><span class="del">DELIVERED ✓</span></div>
<div class="item"><div>🌹 Every wish of Simu coming true</div><span class="del">DELIVERED ✓</span></div>
<div class="item"><div>🤝 Forever by Simu's side</div><span class="del">DELIVERED ✓</span></div>
<button class="btn" style="width:100%;min-width:0;margin-top:16px" onclick="go(7)">Open Birthday Letter for Simu 💌 →</button>
</div>
</div>

<div class="page" id="p7" style="background:radial-gradient(ellipse at 50% 0%,#2a0f2a,#140814 70%,#0a040a 100%)">
<div class="letter">
<div style="text-align:center;font-size:9px;letter-spacing:2.5px;color:#ff7aa2;font-weight:700">✨ GRAND FINALE • FOR SIMU ✨</div>
<h2 style="text-align:center;margin:12px 0">Happy Birthday <span style="font-family:'Great Vibes';color:#ff2e6d;font-size:28px">My Simu! 🌹</span></h2>
<p>My Dearest Simu,</p>
<p>As the clock struck 12:00 AM, my entire world lit up thinking of you, Simu. In a world full of noise, your smile is my quiet peace and my happiest home.</p>
<p>Thank you for being the most beautiful, sweet and caring person in my life, Simu. Every moment shared with you is a memory I treasure deeply.</p>
<p>On your special day, my Simu, I wish you endless laughter, warmth, peace and all your heart's desires coming true today and forever.</p>
<p style="text-align:right">With all my heart & love,<br><b style="color:#ff2e6d">Forever Yours ❤️<br>For My Simu</b></p>
<button class="btn" style="width:100%;min-width:0;margin-top:16px" onclick="go(1)">✨ Celebrate Again Simu! ✨</button>
</div>
</div>

<div class="arrow" id="arrow">➶</div>

<script>
const colors=['#ff4a7a','#7a8cff','#3ec9a8','#ffcc33','#ff6b6b'];

const reasons=[
"REASON 1 OF 5<br><b>Your beautiful smile, Simu, makes every ordinary day feel magical ✨❤️</b>",
"REASON 2 OF 5<br><b>Every little conversation with you becomes my favorite memory 🌙💗</b>",
"REASON 3 OF 5<br><b>Your caring heart makes the world feel softer and brighter 🌸</b>",
"REASON 4 OF 5<br><b>Your laughter is my favorite melody, and your happiness means everything 💖</b>",
"REASON 5 OF 5<br><b>Because you are special, Simu, and you deserve endless love and happiness 🌹❤️</b>"
];

let bi=0,cs=0,shooting=false;

function go(n){
 document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
 document.getElementById('p'+n).classList.add('active');
 if(n==3||n==5)confetti(200);
 if(n==5)initB();
}

function openGift(){
 document.getElementById('gift').classList.add('open');
 setTimeout(()=>{
  document.getElementById('zoom').classList.add('show');
  setTimeout(()=>{
   document.getElementById('zoom').classList.remove('show');
   go(3);
   setTimeout(()=>go(4),2500);
  },1000);
 },600);
}

function doCake(){
 const f=document.getElementById('fl');
 const m=document.getElementById('cmsg');
 if(cs==0){
  f.style.display='block';
  m.innerText='✨ Candle lit for Simu! Tap again to blow! ✨';
  cs=1;
 }else{
  f.style.display='none';
  m.innerText='✨ Wish made! Candle blown out for Simu! 💖';
  confetti(120);
  setTimeout(()=>go(5),1200);
  cs=0;
 }
}

function initB(){
 const r=document.getElementById('bln');
 r.innerHTML='';
 bi=0;
 shooting=false;
 colors.forEach(c=>{
  let d=document.createElement('div');
  d.className='b';
  d.style.background=c;
  r.appendChild(d);
 });
 document.getElementById('card').style.display='none';
 document.getElementById('nxt').style.display='none';
 document.getElementById('bow').style.opacity='1';
 document.getElementById('bow').style.pointerEvents='auto';
}

function heartEffect(x,y){
 const h=document.createElement('div');
 h.className='heartPop';
 h.textContent=['💗','💖','💕','❤️','🌹'][bi];
 h.style.left=x+'px';
 h.style.top=y+'px';
 document.body.appendChild(h);
 setTimeout(()=>h.remove(),1200);
}

function shoot(){
 if(shooting||bi>=5)return;
 const bs=document.querySelectorAll('.b');
 const target=bs[bi];
 if(!target)return;

 shooting=true;
 const rect=target.getBoundingClientRect();
 const bow=document.getElementById('bow').getBoundingClientRect();
 const arrow=document.getElementById('arrow');

 const startX=bow.left+bow.width/2-10;
 const startY=bow.top+bow.height/2-10;
 const endX=rect.left+rect.width/2;
 const endY=rect.top+rect.height/2;

 arrow.style.display='block';
 arrow.style.left=startX+'px';
 arrow.style.top=startY+'px';
 arrow.style.setProperty('--dx',(endX-startX)+'px');
 arrow.style.setProperty('--dy',(endY-startY)+'px');
 arrow.classList.remove('fly');
 void arrow.offsetWidth;
 arrow.classList.add('fly');

 setTimeout(()=>{
  arrow.classList.remove('fly');
  arrow.style.display='none';

  target.classList.add('burst');
  heartEffect(endX,endY);
  confetti(55);

  const cd=document.getElementById('card');
  cd.innerHTML=reasons[bi];
  cd.style.display='block';

  setTimeout(()=>{
   target.style.visibility='hidden';
   bi++;
   shooting=false;

   if(bi===5){
    document.getElementById('nxt').style.display='block';
    document.getElementById('bow').style.opacity='.4';
    document.getElementById('bow').style.pointerEvents='none';
   }
  },400);
 },650);
}

function confetti(count){
 const c=document.getElementById('conf');
 c.width=innerWidth;
 c.height=innerHeight;
 const ctx=c.getContext('2d');
 let ps=[];
 for(let i=0;i<count;i++){
  ps.push({
   x:Math.random()*c.width,
   y:-20,
   r:Math.random()*8+4,
   vy:Math.random()*3+2,
   vx:(Math.random()-.5)*3,
   color:'hsl('+(Math.random()*360)+',100%,65%)'
  });
 }
 let fr=0;
 (function loop(){
  ctx.clearRect(0,0,c.width,c.height);
  ps.forEach(p=>{
   p.y+=p.vy;
   p.x+=p.vx;
   ctx.fillStyle=p.color;
   ctx.fillRect(p.x,p.y,p.r,p.r);
  });
  fr++;
  if(fr<220)requestAnimationFrame(loop);
  else ctx.clearRect(0,0,c.width,c.height);
 })();
}
</script>
</body>
</html>
