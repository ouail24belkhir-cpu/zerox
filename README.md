[gz.html](https://github.com/user-attachments/files/35302150/gz.html)

<!DOCTYPE html>
<html lang="fr" dir="ltr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GZ — GAMING ZONE | Matériel Gaming Pro · Alger & Sétif</title>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700;900&family=Rajdhani:wght@500;600;700&family=Cairo:wght@600;700;900&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
<style>
:root{
  --red:#ff1f2e; --red-d:#c90010; --red-l:#ff5c3c;
  --bg:#0a0a0a; --card:#141417; --card2:#1b1b20;
  --line:#2a2a31; --txt:#f2f2f4; --muted:#8f8f99;
  --grad:linear-gradient(120deg,#ff1f2e,#ff5c3c,#ff1f2e,#ff1f2e);
  --ease:cubic-bezier(.2,1.2,.3,1);
}
*{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth}
body{font-family:'Rajdhani',sans-serif;background:var(--bg);color:var(--txt);overflow-x:hidden;line-height:1.6}
html[dir="rtl"] body{font-family:'Cairo',sans-serif}
html[dir="rtl"] h1,html[dir="rtl"] h2,html[dir="rtl"] h3,html[dir="rtl"] .word,html[dir="rtl"] .price,html[dir="rtl"] .gz,html[dir="rtl"] .av,html[dir="rtl"] .tot b{font-family:'Cairo',sans-serif;letter-spacing:0}
body.locked{overflow:hidden}
::selection{background:var(--red);color:#fff}
::-webkit-scrollbar{width:10px}
::-webkit-scrollbar-track{background:#111}
::-webkit-scrollbar-thumb{background:var(--red);border:2px solid #111}

#loader{position:fixed;inset:0;z-index:9999;background:var(--bg);display:grid;place-items:center;transition:.7s var(--ease)}
#loader.gone{opacity:0;visibility:hidden;clip-path:inset(0 0 100% 0)}
#loader .lg{width:80px;height:80px;display:grid;place-items:center;background:var(--red);color:#fff;border:3px solid #fff;font-family:'Orbitron';font-weight:900;font-size:1.7rem;letter-spacing:-2px;animation:pulseL 1s infinite}
@keyframes pulseL{0%,100%{transform:scale(1) rotate(0)}50%{transform:scale(.9) rotate(-4deg)}}

#prog{position:fixed;top:0;left:0;height:3px;width:0;background:var(--grad);background-size:300% 100%;z-index:6000;animation:shift 3s linear infinite}
@keyframes shift{to{background-position:300% 0}}

.cur,.cur-d{position:fixed;top:0;left:0;pointer-events:none;z-index:5500;border-radius:50%;mix-blend-mode:difference}
.cur{width:38px;height:38px;border:1.5px solid #fff;transition:transform .18s var(--ease),opacity .3s}
.cur-d{width:6px;height:6px;background:#fff}
.cur.hot{transform:scale(1.9);background:rgba(255,255,255,.12)}

header{position:fixed;top:0;left:0;right:0;z-index:1000;padding:16px 48px;background:rgba(10,10,10,.8);backdrop-filter:blur(16px) saturate(160%);border-bottom:2px solid var(--line);transition:.35s var(--ease)}
header.small{padding:9px 48px;background:rgba(10,10,10,.96);box-shadow:0 8px 30px rgba(0,0,0,.6)}
.nav{max-width:1400px;margin:0 auto;display:flex;align-items:center;justify-content:space-between;gap:20px}

.brand{display:flex;align-items:center;gap:12px;text-decoration:none;color:var(--txt)}
.gz{width:46px;height:46px;display:grid;place-items:center;flex:none;background:var(--red);color:#fff;border:2px solid #000;font-family:'Orbitron';font-weight:900;font-size:1.05rem;letter-spacing:-1px;box-shadow:3px 3px 0 rgba(255,31,46,.35);transition:.3s var(--ease);position:relative;overflow:hidden}
.gz::after{content:'';position:absolute;inset:0;background:linear-gradient(120deg,transparent 30%,rgba(255,255,255,.55),transparent 70%);transform:translateX(-120%);transition:.6s}
.brand:hover .gz{transform:translate(-3px,-3px) rotate(-4deg);box-shadow:6px 6px 0 rgba(255,31,46,.5)}
.brand:hover .gz::after{transform:translateX(120%)}
.word{font-family:'Orbitron';font-weight:900;font-size:1.05rem;letter-spacing:2px;line-height:1}
.word small{display:block;font-family:'Rajdhani';font-weight:700;font-size:.62rem;letter-spacing:3.4px;color:var(--muted)}

.menu{display:flex;gap:30px;list-style:none}
.menu a{color:var(--txt);text-decoration:none;font-weight:700;font-size:.88rem;letter-spacing:1.6px;text-transform:uppercase;position:relative;padding-bottom:4px;transition:.25s}
.menu a::after{content:'';position:absolute;left:0;bottom:0;width:0;height:3px;background:var(--grad);background-size:200% 100%;animation:shift 3s linear infinite;transition:width .3s var(--ease)}
.menu a:hover{color:var(--red)}
.menu a:hover::after{width:100%}
.nav-right{display:flex;align-items:center;gap:12px}

.langs{display:flex;align-items:center;gap:6px;padding:5px;border:2px solid var(--line);background:var(--card);box-shadow:3px 3px 0 rgba(255,31,46,.3)}
.langs button{width:38px;height:30px;padding:0;border:2px solid transparent;background:var(--card);cursor:pointer;display:grid;place-items:center;transition:.25s var(--ease);position:relative;overflow:hidden}
.langs button svg{width:100%;height:100%;display:block;border:1px solid rgba(255,255,255,.12)}
.langs button:hover{transform:translateY(-3px);border-color:var(--red)}
.langs button.on{border-color:var(--red);box-shadow:0 0 0 2px rgba(255,31,46,.3);transform:translateY(-2px)}
.langs button.on::after{content:'';position:absolute;bottom:0;left:0;right:0;height:3px;background:var(--red)}

.cart{position:relative;width:46px;height:46px;display:grid;place-items:center;border:2px solid var(--line);background:var(--card);color:var(--txt);cursor:pointer;transition:.25s var(--ease);font-size:1rem;box-shadow:3px 3px 0 rgba(255,31,46,.3)}
.cart:hover{background:var(--red);border-color:var(--red);color:#fff;transform:translate(-2px,-2px);box-shadow:5px 5px 0 rgba(255,31,46,.45)}
.cart b{position:absolute;top:-9px;right:-9px;min-width:21px;height:21px;background:var(--red);color:#fff;border:2px solid #000;border-radius:50%;font-size:.68rem;display:grid;place-items:center;font-weight:800;padding:0 3px}
.cart.bump{animation:bump .5s var(--ease)}
@keyframes bump{0%{transform:scale(1)}35%{transform:scale(1.3) rotate(-8deg)}70%{transform:scale(.94)}100%{transform:scale(1)}}
.burger{display:none;background:var(--card);border:2px solid var(--line);width:46px;height:46px;font-size:1.1rem;cursor:pointer;color:var(--txt)}

.btn{display:inline-flex;align-items:center;gap:10px;padding:15px 30px;font-family:'Rajdhani';font-weight:800;font-size:.9rem;letter-spacing:1.9px;text-transform:uppercase;text-decoration:none;cursor:pointer;border:2px solid #000;transition:.3s var(--ease);position:relative;overflow:hidden}
html[dir="rtl"] .btn{font-family:'Cairo';letter-spacing:0;font-weight:700}
.btn::before{content:'';position:absolute;top:0;left:-100%;width:60%;height:100%;background:linear-gradient(100deg,transparent,rgba(255,255,255,.45),transparent);transition:.6s}
.btn:hover::before{left:140%}
.btn-red{background:var(--red);color:#fff;box-shadow:5px 5px 0 rgba(255,31,46,.35)}
.btn-red:hover{transform:translate(-3px,-3px);box-shadow:8px 8px 0 rgba(255,31,46,.55);background:var(--red-d)}
.btn-ghost{background:var(--card);color:var(--txt);border-color:var(--line);box-shadow:5px 5px 0 rgba(255,31,46,.3)}
.btn-ghost:hover{background:var(--red);border-color:var(--red);color:#fff;transform:translate(-3px,-3px);box-shadow:8px 8px 0 rgba(255,31,46,.5)}
.btn:active{transform:translate(0,0);box-shadow:2px 2px 0 rgba(255,31,46,.4)}

.hero{min-height:100vh;display:grid;place-items:center;text-align:center;padding:150px 24px 90px;position:relative;overflow:hidden;
  background:
    repeating-linear-gradient(0deg,transparent 0 59px,rgba(255,255,255,.045) 59px 60px),
    repeating-linear-gradient(90deg,transparent 0 59px,rgba(255,255,255,.045) 59px 60px),
    radial-gradient(ellipse at 50% 0%,#18181c,#08080a 62%);
  background-size:60px 60px,60px 60px,100% 100%;
  animation:gridDrift 22s linear infinite}
@keyframes gridDrift{to{background-position:0 60px,60px 0,0 0}}
.hero::before{content:'';position:absolute;width:760px;height:760px;background:radial-gradient(circle,rgba(255,31,46,.28),transparent 65%);top:-260px;left:50%;transform:translateX(-50%);pointer-events:none;animation:breathe 8s ease-in-out infinite}
@keyframes breathe{0%,100%{transform:translateX(-50%) scale(1);opacity:.85}50%{transform:translateX(-50%) scale(1.18);opacity:1}}
.orb{position:absolute;border-radius:50%;filter:blur(60px);opacity:.4;pointer-events:none}
.orb.a{width:280px;height:280px;background:var(--red);left:-90px;top:26%;animation:floatA 13s ease-in-out infinite}
.orb.b{width:230px;height:230px;background:#ff8a3c;right:-70px;bottom:16%;animation:floatB 16s ease-in-out infinite}
@keyframes floatA{0%,100%{transform:translate(0,0)}50%{transform:translate(60px,-50px)}}
@keyframes floatB{0%,100%{transform:translate(0,0)}50%{transform:translate(-50px,40px)}}
.hero-in{max-width:960px;position:relative;z-index:2}
.tag{display:inline-flex;align-items:center;gap:9px;padding:8px 18px;margin-bottom:26px;background:var(--card);border:2px solid var(--line);color:var(--txt);font-size:.74rem;letter-spacing:2.4px;text-transform:uppercase;font-weight:800;box-shadow:4px 4px 0 var(--red)}
html[dir="rtl"] .tag{letter-spacing:0}
.hero h1{font-family:'Orbitron';font-weight:900;font-size:clamp(2.5rem,8.4vw,6.4rem);line-height:.96;text-transform:uppercase;letter-spacing:-2px;margin-bottom:22px;position:relative}
html[dir="rtl"] .hero h1{line-height:1.15;font-size:clamp(2.2rem,7.4vw,5.4rem)}
.hero h1 em{font-style:normal;background:var(--grad);background-size:300% 100%;-webkit-background-clip:text;background-clip:text;color:transparent;animation:shift 4s linear infinite}
.hero p{color:var(--muted);font-size:1.12rem;max-width:590px;margin:0 auto 36px;font-weight:600}
.hero-btns{display:flex;gap:14px;justify-content:center;flex-wrap:wrap}
.hero-stats{display:flex;gap:54px;justify-content:center;margin-top:64px;flex-wrap:wrap}
.hero-stats div{text-align:center;transition:.3s}
.hero-stats div:hover{transform:translateY(-5px)}
.hero-stats b{display:block;font-family:'Orbitron';font-size:2rem;font-weight:900;color:var(--txt)}
.hero-stats small{color:var(--muted);letter-spacing:2px;text-transform:uppercase;font-size:.7rem;font-weight:700}
html[dir="rtl"] .hero-stats small{letter-spacing:0}
.scroll-hint{position:absolute;bottom:26px;left:50%;transform:translateX(-50%);font-size:.68rem;letter-spacing:3px;text-transform:uppercase;color:var(--muted);font-weight:800;display:grid;gap:8px;justify-items:center}
.scroll-hint span{width:2px;height:34px;background:linear-gradient(var(--red),transparent);animation:down 1.6s ease-in-out infinite}
@keyframes down{0%,100%{transform:scaleY(.4);opacity:.4;transform-origin:top}50%{transform:scaleY(1);opacity:1}}

.marquee{background:var(--red);color:#fff;overflow:hidden;padding:14px 0;border-block:2px solid #000}
.marquee div{display:flex;gap:60px;width:max-content;animation:slide 26s linear infinite}
.marquee:hover div{animation-play-state:paused}
.marquee span{font-family:'Orbitron';font-size:.9rem;letter-spacing:3.6px;text-transform:uppercase;white-space:nowrap;color:#fff}
html[dir="rtl"] .marquee span{font-family:'Cairo';letter-spacing:0}
.marquee span i{color:#0a0a0a;margin-right:8px}
@keyframes slide{to{transform:translateX(-50%)}}

section{padding:96px 48px;position:relative}
.wrap{max-width:1400px;margin:0 auto}
.head{text-align:center;margin-bottom:56px}
.head .tag{margin-bottom:16px}
.head h2{font-family:'Orbitron';font-size:clamp(1.85rem,4.5vw,3.3rem);font-weight:900;text-transform:uppercase;line-height:1.04;letter-spacing:-1px;position:relative;display:inline-block;color:var(--txt)}
.head h2 span{color:var(--red)}
.head h2::after{content:'';position:absolute;left:50%;bottom:-12px;width:0;height:4px;background:var(--red);transform:translateX(-50%);transition:width .8s var(--ease) .2s}
.head.in h2::after{width:90px}
.head p{color:var(--muted);max-width:540px;margin:20px auto 0;font-size:1.02rem;font-weight:600}

.filters{display:flex;gap:10px;justify-content:center;flex-wrap:wrap;margin-bottom:42px}
.filters button{padding:10px 22px;cursor:pointer;background:var(--card);border:2px solid var(--line);color:var(--txt);font-family:'Rajdhani';font-weight:800;letter-spacing:1.5px;text-transform:uppercase;font-size:.78rem;transition:.25s var(--ease)}
html[dir="rtl"] .filters button{font-family:'Cairo';letter-spacing:0;font-weight:700}
.filters button:hover{background:var(--card2);border-color:var(--red);color:var(--red);transform:translate(-2px,-2px);box-shadow:3px 3px 0 rgba(255,31,46,.35)}
.filters button.on{background:var(--red);border-color:var(--red);color:#fff;box-shadow:4px 4px 0 rgba(255,31,46,.4)}

.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:22px}
.card{background:var(--card);border:2px solid var(--line);display:flex;flex-direction:column;transition:.35s var(--ease);position:relative;overflow:hidden}
.card::after{content:'';position:absolute;inset:0;pointer-events:none;opacity:0;transition:.35s;background:radial-gradient(320px circle at var(--mx,50%) var(--my,50%),rgba(255,31,46,.16),transparent 60%)}
.card:hover{transform:translate(-4px,-6px);border-color:var(--red);box-shadow:0 16px 44px rgba(255,31,46,.22)}
.card:hover::after{opacity:1}
.thumb{height:200px;display:grid;place-items:center;font-size:4rem;color:var(--muted);position:relative;overflow:hidden;border-bottom:2px solid var(--line);background:#101014}
.thumb img{width:100%;height:100%;object-fit:cover;display:block;transition:.55s var(--ease);position:relative;z-index:2}
.thumb.fitbg{background:radial-gradient(circle at 50% 45%,#1d1d24,#0b0b0e 72%)}
.thumb img.fit{object-fit:contain;padding:14px}
.card:hover .thumb img{transform:scale(1.07)}
.thumb .ph{position:relative;z-index:2;transition:.45s var(--ease)}
.card:hover .thumb .ph{transform:scale(1.18) rotate(-8deg);color:var(--red)}
.thumb::before{content:'';position:absolute;inset:-40%;background:conic-gradient(from 0deg,transparent,rgba(255,31,46,.35),transparent 40%);opacity:0;transition:.5s;animation:spin 6s linear infinite;z-index:1}
.card:hover .thumb::before{opacity:1}
.badge{position:absolute;top:10px;left:10px;padding:5px 11px;font-size:.63rem;font-weight:900;letter-spacing:1.5px;text-transform:uppercase;background:#0a0a0a;color:#fff;z-index:4;border:1px solid rgba(255,255,255,.15)}
html[dir="rtl"] .badge{left:auto;right:10px;letter-spacing:0}
.badge.new{background:var(--red);color:#fff;border-color:var(--red);animation:blink 1.6s ease-in-out infinite}
@keyframes blink{0%,100%{opacity:1}50%{opacity:.55}}
.card-body{padding:18px;display:flex;flex-direction:column;flex:1;position:relative;z-index:2}
.card-body h3{font-family:'Orbitron';font-size:.98rem;margin-bottom:7px;letter-spacing:.4px;color:var(--txt)}
.spec{color:var(--muted);font-size:.84rem;margin-bottom:14px;flex:1;font-weight:600}
.stars{color:var(--red);font-size:.72rem;margin-bottom:12px;letter-spacing:2px}
.price-row{display:flex;align-items:center;justify-content:space-between;gap:10px;margin-top:auto}
.price{font-family:'Orbitron';font-weight:900;font-size:1.1rem;line-height:1.15;color:var(--txt)}
.price s{display:block;font-size:.7rem;color:var(--muted);font-weight:500}
.price .da{font-size:.62rem;letter-spacing:1px;color:var(--muted);font-family:'Rajdhani';font-weight:800}
.add{width:42px;height:42px;border:2px solid var(--line);background:var(--card2);color:var(--txt);cursor:pointer;font-size:.95rem;display:grid;place-items:center;transition:.25s var(--ease);flex:none}
.add:hover{background:var(--red);color:#fff;border-color:var(--red);transform:rotate(90deg) scale(1.08)}

.build{display:grid;grid-template-columns:1fr 1fr;gap:56px;align-items:center;background:#050506;color:#fff;padding:56px;border:2px solid var(--red);position:relative;overflow:hidden}
.build::before{content:'';position:absolute;inset:0;background:radial-gradient(600px circle at 80% 20%,rgba(255,31,46,.22),transparent 60%)}
.build>*{position:relative;z-index:2}
.build h2{font-family:'Orbitron';font-size:clamp(1.75rem,4vw,2.8rem);text-transform:uppercase;line-height:1.04;margin-bottom:16px;letter-spacing:-1px}
.build h2 span{color:var(--red)}
.build .tag{box-shadow:4px 4px 0 var(--red)}
.build>div>p{color:rgba(255,255,255,.7);margin-bottom:26px;font-weight:600}
.speclist{list-style:none;display:grid;gap:13px;margin-bottom:32px}
.speclist li{display:flex;gap:12px;align-items:flex-start;color:rgba(255,255,255,.85);font-size:.94rem;font-weight:600;transition:.3s}
.speclist li:hover{transform:translateX(6px);color:#fff}
html[dir="rtl"] .speclist li:hover{transform:translateX(-6px)}
.speclist i{color:var(--red);margin-top:5px;font-size:.82rem}
.build-visual{aspect-ratio:1;display:grid;place-items:center;border:2px solid var(--red);position:relative;overflow:hidden;background:radial-gradient(circle,rgba(255,31,46,.22),transparent 68%)}
.build-visual i{font-size:8.5rem;color:#fff;animation:floaty 5s ease-in-out infinite;position:relative;z-index:3;text-shadow:0 0 40px rgba(255,31,46,.8)}
@keyframes floaty{0%,100%{transform:translateY(0)}50%{transform:translateY(-16px)}}
.ring{position:absolute;border:2px solid rgba(255,31,46,.4);border-radius:50%;animation:spin 18s linear infinite}
.ring.r1{width:72%;height:72%}
.ring.r2{width:94%;height:94%;animation-duration:26s;animation-direction:reverse;border-style:dashed}
.ring.r3{width:50%;height:50%;animation-duration:11s;border-color:rgba(255,255,255,.2)}
@keyframes spin{to{transform:rotate(360deg)}}

.why{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:20px}
.why .box{background:var(--card);border:2px solid var(--line);padding:30px;transition:.3s var(--ease);position:relative;overflow:hidden}
.why .box::before{content:'';position:absolute;left:0;bottom:0;width:100%;height:0;background:rgba(255,31,46,.08);transition:.35s var(--ease)}
.why .box:hover{transform:translate(-4px,-6px);border-color:var(--red);box-shadow:9px 11px 0 rgba(255,31,46,.25)}
.why .box:hover::before{height:100%}
.why .box>*{position:relative;z-index:2}
.why .box .ic{width:52px;height:52px;display:grid;place-items:center;background:var(--red);color:#fff;border:2px solid #000;font-size:1.25rem;margin-bottom:18px;transition:.35s var(--ease)}
.why .box:hover .ic{transform:rotate(-10deg) scale(1.1);background:#fff;color:var(--red)}
.why .box h3{font-family:'Orbitron';font-size:.95rem;margin-bottom:9px;text-transform:uppercase;color:var(--txt)}
.why .box p{color:var(--muted);font-size:.9rem;font-weight:600}

.stores{display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:22px}
.store{position:relative;border:2px solid var(--line);background:var(--card);overflow:hidden;transition:.35s var(--ease)}
.store:hover{transform:translate(-4px,-6px);border-color:var(--red);box-shadow:0 16px 44px rgba(255,31,46,.2)}
.store-top{height:120px;background:#050506;display:grid;place-items:center;position:relative;overflow:hidden;border-bottom:2px solid var(--red)}
.store-top::after{content:'';position:absolute;width:200%;height:200%;background:conic-gradient(from 0deg,transparent,rgba(255,31,46,.5),transparent 35%);animation:spin 7s linear infinite}
.store-top i{font-size:2.6rem;color:#fff;position:relative;z-index:2}
.store-body{padding:22px}
.store-body .city{font-family:'Orbitron';font-size:.7rem;letter-spacing:3px;text-transform:uppercase;color:var(--red);margin-bottom:6px;font-weight:900}
.store-body h3{font-family:'Orbitron';font-size:1.05rem;text-transform:uppercase;margin-bottom:10px;line-height:1.2;color:var(--txt)}
.store-body p{color:var(--muted);font-size:.9rem;font-weight:600;margin-bottom:16px}
.store-body .tel{display:inline-flex;align-items:center;gap:8px;font-weight:800;font-size:.95rem;color:var(--txt);text-decoration:none;border-bottom:2px solid var(--red);padding-bottom:2px;transition:.25s}
.store-body .tel:hover{color:var(--red);gap:12px}

.reviews{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:20px}
.review{background:var(--card);border:2px solid var(--line);padding:28px;position:relative;transition:.3s var(--ease)}
.review:hover{transform:translate(-4px,-6px);border-color:var(--red);box-shadow:0 16px 40px rgba(255,31,46,.18)}
.review .q{position:absolute;top:12px;right:18px;font-size:2.3rem;color:var(--red);font-family:'Orbitron';line-height:1;opacity:.5}
html[dir="rtl"] .review .q{right:auto;left:18px}
.review .stars{margin-bottom:12px}
.review p{color:#cfcfd6;font-size:.93rem;margin-bottom:20px;font-weight:600}
.who{display:flex;align-items:center;gap:12px}
.av{width:42px;height:42px;display:grid;place-items:center;background:var(--red);color:#fff;font-weight:900;font-family:'Orbitron';font-size:.82rem;border:2px solid #000;transition:.3s}
.review:hover .av{background:#fff;color:var(--red);transform:rotate(-6deg)}
.who b{display:block;font-size:.9rem;color:var(--txt)}
.who small{color:var(--muted);font-size:.76rem;font-weight:600}

.news{background:var(--grad);background-size:300% 100%;animation:shift 6s linear infinite;color:#fff;border:2px solid #000;padding:60px;text-align:center;box-shadow:10px 10px 0 rgba(255,31,46,.35);position:relative;overflow:hidden}
.news h2{font-family:'Orbitron';font-size:clamp(1.65rem,4vw,2.7rem);text-transform:uppercase;margin-bottom:12px}
.news p{color:rgba(255,255,255,.95);max-width:500px;margin:0 auto 26px;font-weight:600}
.news form{display:flex;gap:10px;max-width:500px;margin:0 auto;flex-wrap:wrap;justify-content:center;position:relative;z-index:2}
.news input{flex:1;min-width:210px;padding:14px 18px;border:2px solid #000;background:#0a0a0a;color:#fff;font-family:'Rajdhani';font-size:.98rem;font-weight:600}
.news input::placeholder{color:#8f8f99}
.news input:focus{outline:3px solid #000;outline-offset:2px}
.news button{padding:14px 28px;border:2px solid #000;cursor:pointer;background:#0a0a0a;color:#fff;font-family:'Rajdhani';font-weight:800;letter-spacing:1.8px;text-transform:uppercase;font-size:.85rem;transition:.22s}
html[dir="rtl"] .news button{font-family:'Cairo';letter-spacing:0;font-weight:700}
.news button:hover{background:#fff;color:#0a0a0a}

.contact{display:grid;grid-template-columns:1fr 1fr;gap:46px;align-items:start}
.contact-info h2{font-family:'Orbitron';font-size:clamp(1.65rem,4vw,2.6rem);text-transform:uppercase;margin-bottom:14px;line-height:1.05;letter-spacing:-1px;color:var(--txt)}
.contact-info h2 span{color:var(--red)}
.contact-info>p{color:var(--muted);margin-bottom:28px;font-weight:600}
.info-row{display:flex;gap:14px;align-items:center;padding:14px 0;border-bottom:2px solid var(--line);transition:.3s}
.info-row:hover{transform:translateX(6px);border-color:var(--red)}
html[dir="rtl"] .info-row:hover{transform:translateX(-6px)}
.info-row .ic{width:44px;height:44px;display:grid;place-items:center;flex:none;background:var(--red);color:#fff;border:2px solid #000}
.info-row small{display:block;color:var(--muted);font-size:.72rem;letter-spacing:1.6px;text-transform:uppercase;font-weight:800}
html[dir="rtl"] .info-row small{letter-spacing:0}
.info-row b{font-size:.96rem;font-weight:700;color:var(--txt)}
form.cform{background:var(--card);border:2px solid var(--line);padding:32px;box-shadow:8px 8px 0 rgba(255,31,46,.25)}
.fg{margin-bottom:16px}
.fg label{display:block;font-size:.76rem;letter-spacing:1.6px;text-transform:uppercase;color:var(--muted);margin-bottom:7px;font-weight:800}
html[dir="rtl"] .fg label{letter-spacing:0}
.fg input,.fg textarea,.fg select{width:100%;padding:13px 15px;border:2px solid var(--line);background:#0d0d10;color:var(--txt);font-family:'Rajdhani';font-size:.96rem;font-weight:600;transition:.25s}
.fg input::placeholder,.fg textarea::placeholder{color:#6b6b75}
html[dir="rtl"] .fg input,html[dir="rtl"] .fg textarea,html[dir="rtl"] .fg select{font-family:'Cairo'}
.fg input:focus,.fg textarea:focus,.fg select:focus{outline:3px solid var(--red);outline-offset:1px;border-color:var(--red)}
.fg textarea{min-height:105px;resize:vertical}
.cform .btn{width:100%;justify-content:center}

footer{background:#050506;color:#fff;padding:60px 48px 26px;border-top:2px solid var(--red);position:relative;overflow:hidden}
footer::before{content:'';position:absolute;width:600px;height:600px;background:radial-gradient(circle,rgba(255,31,46,.16),transparent 65%);bottom:-300px;right:-150px}
.f-grid{max-width:1400px;margin:0 auto;display:grid;grid-template-columns:1.6fr 1fr 1fr 1fr;gap:36px;margin-bottom:42px;position:relative;z-index:2}
.f-grid h4{font-family:'Orbitron';font-size:.78rem;letter-spacing:2.4px;text-transform:uppercase;margin-bottom:16px;color:var(--red)}
html[dir="rtl"] .f-grid h4{letter-spacing:0}
.f-grid ul{list-style:none;display:grid;gap:10px}
.f-grid a{color:rgba(255,255,255,.62);text-decoration:none;font-size:.9rem;font-weight:600;transition:.25s}
.f-grid a:hover{color:#fff;padding-left:6px}
html[dir="rtl"] .f-grid a:hover{padding-left:0;padding-right:6px}
.f-about .brand{color:#fff}
.f-about p{color:rgba(255,255,255,.6);font-size:.9rem;margin:16px 0 18px;max-width:280px;font-weight:600}
.socials{display:flex;gap:10px}
.socials a{width:38px;height:38px;display:grid;place-items:center;border:2px solid rgba(255,255,255,.3);color:#fff;transition:.25s var(--ease)}
.socials a:hover{background:var(--red);border-color:var(--red);transform:translateY(-4px) rotate(-6deg)}
.f-bottom{max-width:1400px;margin:0 auto;padding-top:22px;border-top:1px solid rgba(255,255,255,.14);display:flex;justify-content:space-between;gap:14px;flex-wrap:wrap;color:rgba(255,255,255,.45);font-size:.8rem;font-weight:600;position:relative;z-index:2}

.toast{position:fixed;bottom:26px;left:26px;z-index:5600;display:flex;align-items:center;gap:12px;padding:15px 20px;background:#0d0d10;color:#fff;border:2px solid var(--red);font-weight:800;box-shadow:6px 6px 0 rgba(255,31,46,.5);transform:translateY(180%);transition:.5s var(--ease)}
.toast.on{transform:translateY(0)}
.toast i{color:var(--red);font-size:1.1rem}

.wa{position:fixed;right:24px;bottom:24px;z-index:4800;width:58px;height:58px;border-radius:50%;display:grid;place-items:center;background:#25d366;color:#fff;font-size:1.6rem;text-decoration:none;border:2px solid #000;box-shadow:0 8px 24px rgba(37,211,102,.45);transition:.3s var(--ease)}
.wa:hover{transform:scale(1.1) rotate(8deg)}
.wa::before,.wa::after{content:'';position:absolute;inset:0;border-radius:50%;border:2px solid #25d366;animation:ripple 2.4s ease-out infinite}
.wa::after{animation-delay:1.2s}
@keyframes ripple{0%{transform:scale(1);opacity:.8}100%{transform:scale(2.1);opacity:0}}

.scrim{position:fixed;inset:0;background:rgba(0,0,0,.75);backdrop-filter:blur(6px);z-index:5100;opacity:0;visibility:hidden;transition:.35s}
.scrim.on{opacity:1;visibility:visible}
.drawer{position:fixed;top:0;right:0;bottom:0;width:min(430px,100%);background:#0d0d10;border-left:2px solid var(--red);z-index:5200;display:flex;flex-direction:column;transform:translateX(105%);transition:.45s var(--ease)}
html[dir="rtl"] .drawer{right:auto;left:0;border-left:0;border-right:2px solid var(--red);transform:translateX(-105%)}
.drawer.on{transform:none}
.dr-head{padding:22px;border-bottom:2px solid var(--line);display:flex;align-items:center;justify-content:space-between;background:var(--card)}
.dr-head h3{font-family:'Orbitron';font-size:1rem;text-transform:uppercase;letter-spacing:1px;color:var(--txt)}
.x{width:40px;height:40px;border:2px solid var(--line);background:var(--card2);color:var(--txt);cursor:pointer;display:grid;place-items:center;transition:.25s}
.x:hover{background:var(--red);border-color:var(--red);color:#fff;transform:rotate(90deg)}
.dr-list{flex:1;overflow-y:auto;padding:18px;display:grid;gap:14px;align-content:start}
.ci{display:flex;gap:12px;border:2px solid var(--line);background:var(--card);padding:12px;align-items:center;animation:pop .35s var(--ease)}
@keyframes pop{from{opacity:0;transform:translateX(20px)}to{opacity:1;transform:none}}
.ci .ico{width:44px;height:44px;flex:none;display:grid;place-items:center;background:#101014;border:2px solid var(--line);color:var(--muted);font-size:1.1rem;overflow:hidden}
.ci .ico img{width:100%;height:100%;object-fit:cover}
.ci .nm{flex:1;font-weight:800;font-size:.88rem;line-height:1.25;color:var(--txt)}
.ci .nm small{display:block;color:var(--red);font-size:.78rem;font-weight:700;font-family:'Orbitron'}
.qty{display:flex;align-items:center;gap:6px}
.qty button{width:26px;height:26px;border:2px solid var(--line);background:var(--card2);color:var(--txt);cursor:pointer;font-weight:900;line-height:1;display:grid;place-items:center;transition:.2s}
.qty button:hover{background:var(--red);color:#fff;border-color:var(--red)}
.qty span{min-width:18px;text-align:center;font-weight:900;font-family:'Orbitron';font-size:.82rem}
.dr-foot{padding:20px;border-top:2px solid var(--line);background:var(--card)}
.tot{display:flex;justify-content:space-between;align-items:baseline;margin-bottom:14px;font-weight:800;text-transform:uppercase;letter-spacing:1.4px;font-size:.8rem;color:var(--muted)}
.tot b{font-family:'Orbitron';font-size:1.3rem;color:var(--txt);letter-spacing:0}
.dr-foot .btn{width:100%;justify-content:center}
.empty{text-align:center;color:var(--muted);font-weight:700;padding:50px 20px}
.empty i{font-size:2.6rem;display:block;margin-bottom:14px;color:var(--line)}

/* ---- PAGE COMMANDE (blanche, plein écran) ---- */
.checkout{position:fixed;inset:0;z-index:5400;background:#fff;color:#0a0a0a;overflow-y:auto;opacity:0;visibility:hidden;transition:.25s}
.checkout.on{opacity:1;visibility:visible}
.ck-head{position:sticky;top:0;z-index:6;background:var(--red);color:#fff;display:flex;align-items:center;justify-content:space-between;gap:14px;padding:16px 22px;border-bottom:2px solid #000}
.ck-head h3{font-family:'Orbitron';font-size:.9rem;text-transform:uppercase;letter-spacing:1px;display:flex;align-items:center;gap:10px}
html[dir="rtl"] .ck-head h3{font-family:'Cairo';letter-spacing:0}
.ck-head .x{background:transparent;border:2px solid rgba(255,255,255,.55);color:#fff}
.ck-head .x:hover{background:#0a0a0a;border-color:#0a0a0a;color:#fff}
.ck-wrap{max-width:620px;margin:0 auto;padding:26px 22px 70px}
.ck-wrap .fg label{color:#5a5a63}
.ck-wrap .fg input,.ck-wrap .fg textarea,.ck-wrap .fg select{background:#fff;border-color:#e3e3ea;color:#0a0a0a}
.ck-wrap .fg input::placeholder,.ck-wrap .fg textarea::placeholder{color:#9a9aa5}
.ck-wrap .radio-row label{background:#f6f6f8;border-color:#e3e3ea;color:#0a0a0a}
.ck-wrap .radio-row label:hover{background:#ededf2;border-color:var(--red)}
.ck-wrap .radio-row label:has(input:checked){background:var(--red);border-color:var(--red);color:#fff}
.ck-wrap .radio-row label:has(input:checked) input{accent-color:#fff}
.ck-wrap .mnote{color:#5a5a63;background:#f6f6f8;border:2px solid #e3e3ea;padding:12px 14px}
.ck-wrap .mnote i{color:#25d366}
.ck-sep{height:2px;background:#ececf1;margin:6px 0 22px}
.two{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.radio-row{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px}
.radio-row label{border:2px solid var(--line);padding:12px;cursor:pointer;font-weight:800;font-size:.82rem;display:flex;gap:9px;align-items:center;transition:.25s;color:var(--txt);background:var(--card)}
.radio-row input{accent-color:var(--red);width:16px;height:16px}
.mnote{font-size:.8rem;font-weight:700;margin-bottom:18px;display:flex;gap:9px;align-items:flex-start}
.mnote i{margin-top:3px}

.rv{opacity:0;transform:translateY(34px);transition:.8s var(--ease)}
.rv.in{opacity:1;transform:none}

@media(max-width:1080px){
  .menu{gap:18px}
  .menu a{font-size:.78rem;letter-spacing:1px}
}
@media(max-width:1000px){
  .build,.contact{grid-template-columns:1fr}
  .build{padding:36px}
  .build-visual{max-width:400px;margin:0 auto}
  .f-grid{grid-template-columns:1fr 1fr}
  .menu{display:none}
  .burger{display:grid;place-items:center}
  header{padding:12px 20px}
  section{padding:72px 20px}
  .news{padding:40px 22px}
  form.cform{padding:24px}
  .cur,.cur-d{display:none}
}
@media(max-width:620px){
  .hero-stats{gap:30px}
  .f-grid{grid-template-columns:1fr}
  .hero{padding-top:132px}
  .f-bottom{flex-direction:column;text-align:center}
  .two{grid-template-columns:1fr}
  .toast{left:16px;right:16px;bottom:16px}
  .langs button{width:32px;height:26px}
  .langs{padding:4px;gap:4px}
  header .word{display:none}
}
@media(prefers-reduced-motion:reduce){
  *{animation-duration:.01ms!important;animation-iteration-count:1!important;transition-duration:.01ms!important}
}
</style>
</head>
<body>

<div id="loader"><div class="lg">GZ</div></div>
<div id="prog"></div>
<div class="cur" id="cur"></div><div class="cur-d" id="curd"></div>

<header id="hdr">
  <nav class="nav">
    <a href="#top" class="brand">
      <span class="gz">GZ</span>
      <span class="word">GAMING ZONE<small>PRO GEAR</small></span>
    </a>
    <ul class="menu" id="menu">
      <li><a href="#shop" data-i18n="nav.shop">Boutique</a></li>
      <li><a href="#builds" data-i18n="nav.custom">Sur mesure</a></li>
      <li><a href="#stores" data-i18n="nav.stores">Magasins</a></li>
      <li><a href="#why" data-i18n="nav.why">Pourquoi nous</a></li>
      <li><a href="#contact" data-i18n="nav.contact">Contact</a></li>
    </ul>
    <div class="nav-right">
      <div class="langs" id="langs">
        <button data-lang="en" title="English" aria-label="English">
          <svg viewBox="0 0 60 40"><rect width="60" height="40" fill="#012169"/><path d="M0,0 L60,40 M60,0 L0,40" stroke="#fff" stroke-width="9"/><path d="M0,0 L60,40 M60,0 L0,40" stroke="#C8102E" stroke-width="4.5"/><path d="M30,0 V40 M0,20 H60" stroke="#fff" stroke-width="14"/><path d="M30,0 V40 M0,20 H60" stroke="#C8102E" stroke-width="8"/></svg>
        </button>
        <button data-lang="fr" class="on" title="Français" aria-label="Français">
          <svg viewBox="0 0 30 20"><rect width="10" height="20" fill="#0055A4"/><rect x="10" width="10" height="20" fill="#fff"/><rect x="20" width="10" height="20" fill="#EF4135"/></svg>
        </button>
        <button data-lang="ar" title="العربية" aria-label="العربية">
          <svg viewBox="0 0 60 40"><rect width="30" height="40" fill="#006233"/><rect x="30" width="30" height="40" fill="#fff"/><circle cx="30" cy="20" r="9.5" fill="none" stroke="#D21034" stroke-width="3"/><path d="M33.2 13.6 l1.7 4.9 5.1 .1-4.2 3 1.6 4.9-4.2-3-4.2 3 1.6-4.9-4.2-3 5.1-.1z" fill="#D21034"/></svg>
        </button>
      </div>
      <div class="cart" id="cartBtn"><i class="fas fa-shopping-cart"></i><b id="cartCount">0</b></div>
      <button class="burger" id="burger" aria-label="Menu"><i class="fas fa-bars"></i></button>
    </div>
  </nav>
</header>

<section class="hero" id="top">
  <div class="orb a"></div><div class="orb b"></div>
  <div class="hero-in">
    <span class="tag"><i class="fas fa-bolt"></i> <span data-i18n="hero.tag">Matériel gaming premium · Algérie</span></span>
    <h1 id="heroTitle"></h1>
    <p data-i18n="hero.p">Composants et périphériques gaming triés sur le volet. Monte ton PC pièce par pièce. Livraison 58 wilayas, garantie 3 ans.</p>
    <div class="hero-btns">
      <a href="#shop" class="btn btn-red"><i class="fas fa-bolt"></i> <span data-i18n="hero.b1">Acheter</span></a>
      <a href="#builds" class="btn btn-ghost"><i class="fas fa-microchip"></i> <span data-i18n="hero.b2">Config sur mesure</span></a>
    </div>
    <div class="hero-stats">
      <div><b id="c1">0</b><small data-i18n="stat.1">Configs livrées</small></div>
      <div><b id="c2">0</b><small data-i18n="stat.2">Gamers satisfaits</small></div>
      <div><b id="c3">0</b><small data-i18n="stat.3">Références</small></div>
    </div>
  </div>
  <div class="scroll-hint"><span></span><em data-i18n="hero.scroll" style="font-style:normal">Scroll</em></div>
</section>

<div class="marquee">
  <div id="marquee"></div>
</div>

<section id="shop">
  <div class="wrap">
    <div class="head rv">
      <span class="tag"><i class="fas fa-layer-group"></i> <span data-i18n="shop.tag">Catalogue</span></span>
      <h2 data-i18n-html="shop.h2">Composants <span>&amp; Gear</span></h2>
      <p data-i18n="shop.p">Chaque pièce à l'unité. Choisis tes composants et construis ta machine.</p>
    </div>

    <div class="filters rv">
      <button class="on" data-f="all" data-i18n="f.all">Tout</button>
      <button data-f="gpu" data-i18n="f.gpu">Cartes graphiques</button>
      <button data-f="cpu" data-i18n="f.cpu">Processeurs</button>
      <button data-f="ram" data-i18n="f.ram">RAM</button>
      <button data-f="ssd" data-i18n="f.ssd">SSD</button>
      <button data-f="psu" data-i18n="f.psu">Alimentations</button>
      <button data-f="mobo" data-i18n="f.mobo">Cartes mères</button>
      <button data-f="case" data-i18n="f.case">Boîtiers</button>
      <button data-f="cool" data-i18n="f.cool">Refroidissement</button>
      <button data-f="keyboard" data-i18n="f.kb">Claviers</button>
      <button data-f="mouse" data-i18n="f.mouse">Souris</button>
      <button data-f="audio" data-i18n="f.audio">Casques</button>
      <button data-f="display" data-i18n="f.display">Écrans</button>
      <button data-f="chair" data-i18n="f.chair">Chaises</button>
      <button data-f="desk" data-i18n="f.desk">Tapis</button>
    </div>

    <div class="grid" id="grid">

      <article class="card rv" data-c="gpu" data-id="g1" data-name="GZ FORGE RTX 3060" data-price="49900">
        <div class="thumb fitbg"><span class="badge" data-i18n="b.best">Best Seller</span><img class="fit" src="https://dlcdnwebimgs.asus.com/gain/7FD5645D-78C6-4A60-88B9-1E8D8A0D18B9/w1000/h732" data-icon="fa-microchip" onerror="imgFail(this)" alt="Carte graphique RTX 3060 triple ventilateur"></div>
        <div class="card-body">
          <h3>GZ FORGE RTX 3060</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s1">12GB GDDR6 · Triple ventilateur · 1080p</p>
          <div class="price-row"><span class="price">49 900 <span class="da">DA</span><s>58 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="gpu" data-id="g2" data-name="GZ FORGE RTX 4070 Ti" data-price="142000">
        <div class="thumb fitbg"><span class="badge new" data-i18n="b.new">Nouveau</span><img class="fit" src="https://press.asus.com/assets/w_2000,h_1470/e4a7a3c4-260b-41d6-a52a-e75eafb0d2f2/Angled%20top%20down%20view%20of%20the%20ROG%20Strix%20GeForce%20RTX%204070TI%20graphics%20card%20highlighting%20the%20fans,%20ARGB%20element-1.png" data-icon="fa-microchip" onerror="imgFail(this)" alt="Carte graphique RTX 4070 Ti double ventilateur"></div>
        <div class="card-body">
          <h3>GZ FORGE RTX 4070 Ti</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s2">12GB GDDR6X · Double ventilateur · 1440p</p>
          <div class="price-row"><span class="price">142 000 <span class="da">DA</span><s>165 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="cpu" data-id="c1" data-name="AMD RYZEN 7 7800X3D" data-price="76500">
        <div class="thumb"><span class="badge" data-i18n="b.hot">Hot</span><img src="https://plus.unsplash.com/premium_photo-1683121716061-3faddf4dc504?fm=jpg&q=60&w=1200&auto=format&fit=crop" data-icon="fa-microchip" onerror="imgFail(this)" alt="AMD Ryzen AM5"></div>
        <div class="card-body">
          <h3>AMD RYZEN 7 7800X3D</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s3">8 cœurs · 3D V-Cache · Socket AM5</p>
          <div class="price-row"><span class="price">76 500 <span class="da">DA</span><s>89 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="cpu" data-id="c2" data-name="INTEL CORE i9-14900K" data-price="98000">
        <div class="thumb"><span class="badge" data-i18n="b.pro">Pro</span><img src="https://plus.unsplash.com/premium_photo-1683121716061-3faddf4dc504?fm=jpg&q=60&w=1200&auto=format&fit=crop" data-icon="fa-microchip" onerror="imgFail(this)" alt="Intel Core i9"></div>
        <div class="card-body">
          <h3>INTEL CORE i9-14900K</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s4">24 cœurs · 6.0 GHz · Socket LGA1700</p>
          <div class="price-row"><span class="price">98 000 <span class="da">DA</span><s>112 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="ram" data-id="r1" data-name="GZ VENOM DDR5 32GB 6000MHz" data-price="24500">
        <div class="thumb"><span class="badge" data-i18n="b.hot">Hot</span><img src="https://www.shutterstock.com/image-photo/closeup-modern-ddr5-random-access-260nw-2722093203.jpg" data-icon="fa-memory" onerror="imgFail(this)" alt="RAM DDR5"></div>
        <div class="card-body">
          <h3>GZ VENOM DDR5 32GB</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s5">2×16GB · 6000MHz CL30 · RGB</p>
          <div class="price-row"><span class="price">24 500 <span class="da">DA</span><s>29 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="ram" data-id="r2" data-name="GZ VENOM DDR5 16GB 5600MHz" data-price="13900">
        <div class="thumb"><img src="https://www.shutterstock.com/image-photo/closeup-modern-ddr5-random-access-260nw-2722093203.jpg" data-icon="fa-memory" onerror="imgFail(this)" alt="RAM DDR5"></div>
        <div class="card-body">
          <h3>GZ VENOM DDR5 16GB</h3>
          <div class="stars">★★★★☆</div>
          <p class="spec" data-i18n="s6">2×8GB · 5600MHz CL36</p>
          <div class="price-row"><span class="price">13 900 <span class="da">DA</span></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="ssd" data-id="s1" data-name="GZ RAPID NVMe 2TB Gen4" data-price="26500">
        <div class="thumb"><span class="badge new" data-i18n="b.new">Nouveau</span><img src="https://c1.neweggimages.com/sellingpilot/modules/product/a-plus/7e5d75528426c2609abccccc3f07e7b7196d499d44d0449e9c40382705cb73c9.jpg" data-icon="fa-hard-drive" onerror="imgFail(this)" alt="SSD NVMe"></div>
        <div class="card-body">
          <h3>GZ RAPID NVMe 2TB</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s7">Gen4 · 7400 MB/s · Dissipateur</p>
          <div class="price-row"><span class="price">26 500 <span class="da">DA</span><s>31 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="ssd" data-id="s2" data-name="GZ RAPID NVMe 1TB Gen4" data-price="14500">
        <div class="thumb"><img src="https://c1.neweggimages.com/sellingpilot/modules/product/a-plus/7e5d75528426c2609abccccc3f07e7b7196d499d44d0449e9c40382705cb73c9.jpg" data-icon="fa-hard-drive" onerror="imgFail(this)" alt="SSD NVMe"></div>
        <div class="card-body">
          <h3>GZ RAPID NVMe 1TB</h3>
          <div class="stars">★★★★☆</div>
          <p class="spec" data-i18n="s8">Gen4 · 7000 MB/s · M.2</p>
          <div class="price-row"><span class="price">14 500 <span class="da">DA</span></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="psu" data-id="pu1" data-name="GZ POWER 850W Gold" data-price="21900">
        <div class="thumb"><span class="badge" data-i18n="b.pro">Pro</span><img src="https://www.silentiumpc.com/wp-content/uploads/2020/04/product-page-hero-spc268-1920x600.jpg" data-icon="fa-plug" onerror="imgFail(this)" alt="Alimentation 850W"></div>
        <div class="card-body">
          <h3>GZ POWER 850W GOLD</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s9">80+ Gold · Modulaire · ATX 3.0</p>
          <div class="price-row"><span class="price">21 900 <span class="da">DA</span><s>25 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="psu" data-id="pu2" data-name="GZ POWER 650W Bronze" data-price="10900">
        <div class="thumb"><img src="https://www.silentiumpc.com/wp-content/uploads/2020/04/product-page-hero-spc268-1920x600.jpg" data-icon="fa-plug" onerror="imgFail(this)" alt="Alimentation 650W"></div>
        <div class="card-body">
          <h3>GZ POWER 650W BRONZE</h3>
          <div class="stars">★★★★☆</div>
          <p class="spec" data-i18n="s10">80+ Bronze · Semi-modulaire</p>
          <div class="price-row"><span class="price">10 900 <span class="da">DA</span></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="mobo" data-id="mb1" data-name="GZ STRIKE Z790" data-price="48700">
        <div class="thumb"><img src="https://i.ebayimg.com/images/g/yyYAAeSwLDFqXUZv/s-l400.jpg" data-icon="fa-microchip" onerror="imgFail(this)" alt="Carte mère Z790"></div>
        <div class="card-body">
          <h3>GZ STRIKE Z790</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s11">LGA1700 · DDR5 · PCIe 5.0 · Wi-Fi 6E</p>
          <div class="price-row"><span class="price">48 700 <span class="da">DA</span><s>56 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="mobo" data-id="mb2" data-name="GZ STRIKE B650" data-price="28900">
        <div class="thumb"><img src="https://i.ebayimg.com/images/g/yyYAAeSwLDFqXUZv/s-l400.jpg" data-icon="fa-microchip" onerror="imgFail(this)" alt="Carte mère B650"></div>
        <div class="card-body">
          <h3>GZ STRIKE B650</h3>
          <div class="stars">★★★★☆</div>
          <p class="spec" data-i18n="s12">AM5 · DDR5 · PCIe 4.0</p>
          <div class="price-row"><span class="price">28 900 <span class="da">DA</span></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="case" data-id="cs1" data-name="GZ NEXUS Tower" data-price="17900">
        <div class="thumb"><span class="badge" data-i18n="b.hot">Hot</span><img src="https://www.jawa.gg/images/production-listing-deee5a24230c2deeceadfb405b375f89/width=1200,height=900,quality=80,format=auto,fit=cover" data-icon="fa-server" onerror="imgFail(this)" alt="Boîtier PC"></div>
        <div class="card-body">
          <h3>GZ NEXUS TOWER</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s13">Verre trempé · 3 ventilateurs RGB · ATX</p>
          <div class="price-row"><span class="price">17 900 <span class="da">DA</span><s>21 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="cool" data-id="co1" data-name="GZ GLACIER 360 AIO" data-price="32500">
        <div class="thumb"><span class="badge" data-i18n="b.pro">Pro</span><img src="https://www.pccasegear.com/images/SKELETON-360-ARGB-B-ftr1.jpg" data-icon="fa-fan" onerror="imgFail(this)" alt="Watercooling AIO 360"></div>
        <div class="card-body">
          <h3>GZ GLACIER 360 AIO</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s14">Radiateur 360mm · ARGB · 2500 RPM</p>
          <div class="price-row"><span class="price">32 500 <span class="da">DA</span><s>38 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="keyboard" data-id="k1" data-name="APEX K70 RGB" data-price="24500">
        <div class="thumb"><span class="badge" data-i18n="b.best">Best Seller</span><img src="http://iqunix.com/cdn/shop/files/04_ee0aad70-2530-4881-9fab-5e08f198c0cf.jpg?v=1794391116" data-icon="fa-keyboard" onerror="imgFail(this)" alt="Clavier mécanique"></div>
        <div class="card-body">
          <h3>APEX K70 RGB</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s15">Hot-swap · Switches linéaires · Châssis alu</p>
          <div class="price-row"><span class="price">24 500 <span class="da">DA</span><s>29 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="mouse" data-id="m1" data-name="VIPER LIGHT 8K" data-price="21500">
        <div class="thumb"><span class="badge new" data-i18n="b.new">Nouveau</span><img src="https://thumbs.dreamstime.com/b/image-presents-black-computer-mouse-red-light-its-top-resting-dark-surface-mouse-positioned-slightly-388711293.jpg" data-icon="fa-computer-mouse" onerror="imgFail(this)" alt="Souris gaming"></div>
        <div class="card-body">
          <h3>VIPER LIGHT 8K</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s16">58g · Polling 8000Hz · Capteur 32K DPI</p>
          <div class="price-row"><span class="price">21 500 <span class="da">DA</span><s>25 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="audio" data-id="a1" data-name="ECHO 7 WIRELESS" data-price="28900">
        <div class="thumb"><span class="badge" data-i18n="b.best">Best Seller</span><img src="https://dlcdnwebimgs.asus.com/files/media/202610/665f84ab-9801-4afa-824e-85075d5b9ecb/v1/images/delta-ii/di-42x.webp" data-icon="fa-headset" onerror="imgFail(this)" alt="Casque gaming"></div>
        <div class="card-body">
          <h3>ECHO 7 WIRELESS</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s17">Surround 7.1 · Drivers 50mm · Batterie 60h</p>
          <div class="price-row"><span class="price">28 900 <span class="da">DA</span><s>34 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="display" data-id="d1" data-name="VORTEX 27 240Hz" data-price="62000">
        <div class="thumb"><span class="badge" data-i18n="b.pro">Pro</span><img src="https://www.lg.com/content/dam/channelbtb/lgcom/ca_en/images/monitors/34g600a-b/features/ultragear-gaming-34g600a-2025-feature-15-m.jpg" data-icon="fa-tv" onerror="imgFail(this)" alt="Écran gaming"></div>
        <div class="card-body">
          <h3>VORTEX 27 240Hz</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s18">27" QHD · 240Hz · 0.5ms · Dalle IPS</p>
          <div class="price-row"><span class="price">62 000 <span class="da">DA</span><s>72 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="chair" data-id="ch1" data-name="THRONE ELITE" data-price="54900">
        <div class="thumb"><span class="badge" data-i18n="b.comfort">Confort</span><img src="https://gtracing.com/cdn/shop/files/099_5.png?v=1792640227" data-icon="fa-chair" onerror="imgFail(this)" alt="Chaise gaming"></div>
        <div class="card-body">
          <h3>THRONE ELITE</h3>
          <div class="stars">★★★★★</div>
          <p class="spec" data-i18n="s19">Accoudoirs 4D · Soutien lombaire · Inclinaison 160°</p>
          <div class="price-row"><span class="price">54 900 <span class="da">DA</span><s>63 000 DA</s></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

      <article class="card rv" data-c="desk" data-id="dm1" data-name="GZ ARENA Desk Mat XXL" data-price="4900">
        <div class="thumb"><img src="https://m.media-amazon.com/images/I/71wNqvwG-nS._AC_UF894,1000_QL80_.jpg" data-icon="fa-border-all" onerror="imgFail(this)" alt="Tapis de bureau XXL"></div>
        <div class="card-body">
          <h3>GZ ARENA DESK MAT XXL</h3>
          <div class="stars">★★★★☆</div>
          <p class="spec" data-i18n="s20">900×400mm · Base antidérapante · Bords cousus</p>
          <div class="price-row"><span class="price">4 900 <span class="da">DA</span></span><button class="add" aria-label="Ajouter"><i class="fas fa-plus"></i></button></div>
        </div>
      </article>

    </div>
  </div>
</section>

<section id="builds">
  <div class="wrap">
    <div class="build rv">
      <div>
        <span class="tag"><i class="fas fa-wrench"></i> <span data-i18n="build.tag">Config sur mesure</span></span>
        <h2 data-i18n-html="build.h2">Monté Selon <span>Tes Specs</span></h2>
        <p data-i18n="build.p">Dis-nous ton budget et les jeux auxquels tu joues. Nos techs choisissent les pièces, montent, stress-testent et expédient — configuré, câblé proprement et prêt à brancher.</p>
        <ul class="speclist">
          <li><i class="fas fa-check"></i> <span data-i18n="build.l1">Session live gratuite avec un technicien</span></li>
          <li><i class="fas fa-check"></i> <span data-i18n="build.l2">Test de burn-in 48h avant expédition</span></li>
          <li><i class="fas fa-check"></i> <span data-i18n="build.l3">Cable management + réglage du profil RGB</span></li>
          <li><i class="fas fa-check"></i> <span data-i18n="build.l4">Garantie 3 ans pièces &amp; main d'œuvre</span></li>
        </ul>
        <a href="#contact" class="btn btn-red"><i class="fas fa-paper-plane"></i> <span data-i18n="build.btn">Démarrer ma config</span></a>
      </div>
      <div class="build-visual">
        <div class="ring r1"></div><div class="ring r2"></div><div class="ring r3"></div>
        <i class="fas fa-microchip"></i>
      </div>
    </div>
  </div>
</section>

<section id="stores">
  <div class="wrap">
    <div class="head rv">
      <span class="tag"><i class="fas fa-store"></i> <span data-i18n="stores.tag">Nos magasins</span></span>
      <h2 data-i18n-html="stores.h2">Viens <span>Tester</span></h2>
      <p data-i18n="stores.p">Deux showrooms, deux wilayas. Viens essayer le matos avant d'acheter.</p>
    </div>
    <div class="stores">
      <div class="store rv">
        <div class="store-top"><i class="fas fa-location-dot"></i></div>
        <div class="store-body">
          <div class="city" data-i18n="st1.city">Alger</div>
          <h3 data-i18n="st1.name">Mohammadia Mall</h3>
          <p data-i18n="st1.p">Showroom niveau 2 — démos, tests de configs et retrait de commande sur place.</p>
          <a class="tel" href="tel:+213555588784"><i class="fas fa-phone"></i> 0555 588 784</a>
        </div>
      </div>
      <div class="store rv">
        <div class="store-top"><i class="fas fa-location-dot"></i></div>
        <div class="store-body">
          <div class="city" data-i18n="st2.city">Sétif</div>
          <h3 data-i18n="st2.name">ParkMall Sétif</h3>
          <p data-i18n="st2.p">Espace gaming — setup de test, accessoires en stock et conseil technique direct.</p>
          <a class="tel" href="tel:+213555588785"><i class="fas fa-phone"></i> 0555 588 785</a>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="why">
  <div class="wrap">
    <div class="head rv">
      <span class="tag"><i class="fas fa-shield-halved"></i> <span data-i18n="why.tag">Pourquoi Gaming Zone</span></span>
      <h2 data-i18n-html="why.h2">Zéro Compromis. <span>Jamais.</span></h2>
      <p data-i18n="why.p">On ne stocke que du matos qu'on mettrait dans nos propres configs.</p>
    </div>
    <div class="why">
      <div class="box rv"><div class="ic"><i class="fas fa-truck-fast"></i></div><h3 data-i18n="why.1t">Livraison Express</h3><p data-i18n="why.1p">Livraison 58 wilayas, suivi de bout en bout, paiement à la réception.</p></div>
      <div class="box rv"><div class="ic"><i class="fas fa-shield-halved"></i></div><h3 data-i18n="why.2t">Garantie 3 ans</h3><p data-i18n="why.2p">Pièces et main d'œuvre couvertes. Pas de petites lignes, pas de pièges.</p></div>
      <div class="box rv"><div class="ic"><i class="fas fa-headset"></i></div><h3 data-i18n="why.3t">Experts 24/7</h3><p data-i18n="why.3p">De vrais gamers au support, jour et nuit — chat, téléphone ou WhatsApp.</p></div>
      <div class="box rv"><div class="ic"><i class="fas fa-rotate-left"></i></div><h3 data-i18n="why.4t">Retour 30 jours</h3><p data-i18n="why.4p">Tu changes d'avis ? Renvoie sous 30 jours, sans justification.</p></div>
    </div>
  </div>
</section>

<section id="reviews">
  <div class="wrap">
    <div class="head rv">
      <span class="tag"><i class="fas fa-star"></i> <span data-i18n="rev.tag">Avis</span></span>
      <h2 data-i18n-html="rev.h2">Les Joueurs <span>Parlent</span></h2>
      <p data-i18n="rev.p">4.9/5 sur plus de 12 400 commandes vérifiées.</p>
    </div>
    <div class="reviews">
      <div class="review rv"><span class="q">"</span><div class="stars">★★★★★</div><p data-i18n="rev.1">Commandé le TITAN X9. Livré en 2 jours à Alger, câblage parfait, fiche de benchmark dans le carton. Les FPS sont fous.</p><div class="who"><div class="av">KA</div><div><b>Karim A.</b><small data-i18n="rev.1s">Acheteur vérifié · Alger</small></div></div></div>
      <div class="review rv"><span class="q">"</span><div class="stars">★★★★★</div><p data-i18n="rev.2">Le support m'a aidé à choisir les pièces selon mon budget au lieu de m'upseller. Premier shop qui est vraiment de mon côté.</p><div class="who"><div class="av">ML</div><div><b>Mehdi L.</b><small data-i18n="rev.2s">Acheteur vérifié · Sétif</small></div></div></div>
      <div class="review rv"><span class="q">"</span><div class="stars">★★★★★</div><p data-i18n="rev.3">Le casque Echo 7 est irréel, le micro est clair et la batterie dure une éternité. L'emballage aussi est premium.</p><div class="who"><div class="av">SF</div><div><b>Sara F.</b><small data-i18n="rev.3s">Acheteur vérifié · Oran</small></div></div></div>
    </div>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="news rv">
      <h2 data-i18n="news.h2">Sois Le Premier Informé</h2>
      <p data-i18n="news.p">Restocks, guides de build et offres réservées aux membres. Zéro spam.</p>
      <form id="newsForm">
        <input type="email" data-i18n-ph="news.ph" placeholder="ton@email.com" required>
        <button type="submit" data-i18n="news.btn">S'abonner</button>
      </form>
    </div>
  </div>
</section>

<section id="contact">
  <div class="wrap contact">
    <div class="contact-info rv">
      <span class="tag"><i class="fas fa-comments"></i> <span data-i18n="nav.contact">Contact</span></span>
      <h2 data-i18n-html="ct.h2">Parle À Un <span>Vrai Gamer</span></h2>
      <p data-i18n="ct.p">Une question sur une config, la livraison ou la garantie ? On répond en moins de 2h sur WhatsApp.</p>
      <div class="info-row"><div class="ic"><i class="fas fa-phone"></i></div><div><small data-i18n="ct.call">Appelle-nous</small><b>0555 588 784 · 0555 588 785</b></div></div>
      <div class="info-row"><div class="ic"><i class="fas fa-envelope"></i></div><div><small data-i18n="ct.mail">Email</small><b>support@gamingzone.gg</b></div></div>
      <div class="info-row"><div class="ic"><i class="fas fa-location-dot"></i></div><div><small data-i18n="ct.show">Showrooms</small><b>Mohammadia Mall Alger · ParkMall Sétif</b></div></div>
      <div class="info-row"><div class="ic"><i class="fas fa-clock"></i></div><div><small data-i18n="ct.hours">Horaires</small><b data-i18n="ct.hoursv">En ligne 24/7</b></div></div>
    </div>
    <form class="cform rv" id="cform">
      <div class="fg"><label data-i18n="fm.name">Ton nom</label><input type="text" name="nom" data-i18n-ph="fm.nameph" placeholder="Karim Benali" required></div>
      <div class="fg"><label data-i18n="fm.tel">Téléphone</label><input type="tel" name="tel" data-i18n-ph="fm.telph" placeholder="0555 00 00 00" required></div>
      <div class="fg"><label data-i18n="fm.budget">Budget</label><input type="text" name="budget" data-i18n-ph="fm.budgetph" placeholder="ex : 150 000 DA"></div>
      <div class="fg"><label data-i18n="fm.msg">Message</label><textarea name="msg" data-i18n-ph="fm.msgph" placeholder="Dis-nous à quoi tu joues et ce qu'il te faut..." required></textarea></div>
      <button class="btn btn-red" type="submit"><i class="fab fa-whatsapp"></i> <span data-i18n="fm.btn">Envoyer sur WhatsApp</span></button>
    </form>
  </div>
</section>

<footer>
  <div class="f-grid">
    <div class="f-about">
      <a href="#top" class="brand"><span class="gz">GZ</span><span class="word">GAMING ZONE<small>PRO GEAR</small></span></a>
      <p data-i18n="ft.p">Composants et gear pro pour les joueurs qui prennent ça au sérieux. Testé et expédié par des gamers.</p>
      <div class="socials">
        <a href="https://wa.me/213555588784" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a>
        <a href="#" aria-label="Discord"><i class="fab fa-discord"></i></a>
        <a href="#" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
        <a href="#" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
        <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
      </div>
    </div>
    <div><h4 data-i18n="ft.shop">Boutique</h4><ul><li><a href="#shop" data-i18n="f.gpu">Cartes graphiques</a></li><li><a href="#shop" data-i18n="f.cpu">Processeurs</a></li><li><a href="#shop" data-i18n="f.ram">RAM</a></li><li><a href="#shop" data-i18n="f.ssd">SSD</a></li><li><a href="#shop" data-i18n="f.psu">Alimentations</a></li></ul></div>
    <div><h4 data-i18n="ft.sup">Support</h4><ul><li><a href="#contact" data-i18n="nav.contact">Contact</a></li><li><a href="#stores" data-i18n="nav.stores">Magasins</a></li><li><a href="#" data-i18n="ft.ship">Livraison</a></li><li><a href="#" data-i18n="ft.war">Garantie</a></li><li><a href="#" data-i18n="ft.ret">Retours</a></li></ul></div>
    <div><h4 data-i18n="ft.co">Société</h4><ul><li><a href="#why" data-i18n="ft.about">À propos</a></li><li><a href="#reviews" data-i18n="rev.tag">Avis</a></li><li><a href="#builds" data-i18n="ft.custom">Configs sur mesure</a></li><li><a href="#" data-i18n="ft.car">Carrières</a></li><li><a href="#" data-i18n="ft.press">Presse</a></li></ul></div>
  </div>
  <div class="f-bottom"><span data-i18n="ft.copy">© 2026 Gaming Zone — Mohammadia Mall Alger · ParkMall Sétif</span><span data-i18n="ft.legal">Confidentialité · CGV · Cookies</span></div>
</footer>

<a class="wa" id="waBubble" href="https://wa.me/213555588784" target="_blank" rel="noopener" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a>

<div class="toast" id="toast"><i class="fas fa-circle-check"></i><span id="toastTxt">Ajouté au panier</span></div>

<div class="scrim" id="scrim"></div>
<aside class="drawer" id="drawer">
  <div class="dr-head">
    <h3><i class="fas fa-cart-shopping"></i> <span data-i18n="dr.title">Ton panier</span></h3>
    <button class="x" id="drClose" aria-label="Fermer"><i class="fas fa-xmark"></i></button>
  </div>
  <div class="dr-list" id="drList"></div>
  <div class="dr-foot">
    <div class="tot"><span data-i18n="dr.total">Total</span><b id="drTotal">0 DA</b></div>
    <button class="btn btn-red" id="toCheckout"><i class="fab fa-whatsapp"></i> <span data-i18n="dr.order">Commander</span></button>
  </div>
</aside>

<div class="checkout" id="modal">
  <div class="ck-head">
    <h3><i class="fab fa-whatsapp"></i> <span data-i18n="md.title">Finaliser la commande</span></h3>
    <button class="x" id="mClose" aria-label="Fermer"><i class="fas fa-xmark"></i></button>
  </div>
  <div class="ck-wrap">
    <div class="mnote"><i class="fas fa-circle-info"></i><span data-i18n="md.note">Le récap complet sera envoyé directement sur notre WhatsApp. On confirme le stock et les frais de livraison avant expédition.</span></div>
    <div class="fg"><label data-i18n="md.store">Magasin</label>
      <div class="radio-row">
        <label><input type="radio" name="store" value="Alger — Mohammadia Mall" checked> <span data-i18n="st1.city">Alger</span></label>
        <label><input type="radio" name="store" value="Sétif — ParkMall"> <span data-i18n="st2.city">Sétif</span></label>
      </div>
    </div>
    <div class="fg"><label data-i18n="md.name">Nom &amp; prénom</label><input type="text" id="fName" placeholder="Karim Benali" required></div>
    <div class="fg"><label data-i18n="fm.tel">Téléphone</label><input type="tel" id="fTel" data-i18n-ph="fm.telph" placeholder="0555 00 00 00" required></div>
    <div class="two">
      <div class="fg"><label data-i18n="md.wil">Wilaya</label><select id="fWilaya"></select></div>
      <div class="fg"><label data-i18n="md.city">Commune</label><input type="text" id="fCity" placeholder="Bab Ezzouar"></div>
    </div>
    <div class="fg"><label data-i18n="md.addr">Adresse</label><input type="text" id="fAddr" data-i18n-ph="md.addrph" placeholder="Cité, rue, n°..."></div>
    <div class="fg"><label data-i18n="md.ship">Mode de livraison</label>
      <div class="radio-row">
        <label><input type="radio" name="ship" value="domicile" checked> <span data-i18n="md.home">À domicile</span></label>
        <label><input type="radio" name="ship" value="bureau"> <span data-i18n="md.office">Au bureau</span></label>
      </div>
    </div>
    <div class="fg"><label data-i18n="md.opt">Note (optionnel)</label><textarea id="fNote" style="min-height:70px" data-i18n-ph="md.optph" placeholder="Heure d'appel, repère..."></textarea></div>
    <button class="btn btn-red" id="sendWa" style="width:100%;justify-content:center"><i class="fab fa-whatsapp"></i> <span data-i18n="md.send">Envoyer la commande</span></button>
  </div>
</div>

<script>
const $ = s => document.querySelector(s);
const $$ = s => [...document.querySelectorAll(s)];
const fmt = n => n.toLocaleString('fr-FR').replace(/\u202f|\u00a0/g,' ') + ' DA';
const WA = { alger:'213555588784', setif:'213555588785' };

function imgFail(el){
  const wrap = el.parentElement;
  const icon = el.dataset.icon || 'fa-box';
  el.remove();
  const i = document.createElement('i');
  i.className = 'fas ' + icon + ' ph';
  wrap.appendChild(i);
}

const I18N = {
  fr:{
    "nav.shop":"Boutique","nav.custom":"Sur mesure","nav.stores":"Magasins","nav.why":"Pourquoi nous","nav.contact":"Contact",
    "hero.tag":"Composants gaming premium · Algérie","hero.t1":"Monte ta","hero.t2":"Machine Ultime",
    "hero.p":"Composants et périphériques gaming triés sur le volet. Monte ton PC pièce par pièce. Livraison 58 wilayas, garantie 3 ans.",
    "hero.b1":"Acheter","hero.b2":"Config sur mesure","hero.scroll":"Scroll",
    "stat.1":"Configs livrées","stat.2":"Gamers satisfaits","stat.3":"Références",
    "mq.1":"RTX POWERED","mq.2":"LIVRAISON 58 WILAYAS","mq.3":"GARANTIE 3 ANS","mq.4":"SUPPORT 24/7","mq.5":"TESTÉ AU BENCHMARK",
    "shop.tag":"Catalogue","shop.h2":"Composants <span>&amp; Gear</span>","shop.p":"Chaque pièce à l'unité. Choisis tes composants et construis ta machine.",
    "f.all":"Tout","f.gpu":"Cartes graphiques","f.cpu":"Processeurs","f.ram":"RAM","f.ssd":"SSD","f.psu":"Alimentations","f.mobo":"Cartes mères","f.case":"Boîtiers","f.cool":"Refroidissement","f.kb":"Claviers","f.mouse":"Souris","f.audio":"Casques","f.display":"Écrans","f.chair":"Chaises","f.desk":"Tapis",
    "b.best":"Best Seller","b.new":"Nouveau","b.hot":"Hot","b.pro":"Pro","b.comfort":"Confort",
    "s1":"12GB GDDR6 · Triple ventilateur · 1080p","s2":"12GB GDDR6X · Double ventilateur · 1440p",
    "s3":"8 cœurs · 3D V-Cache · Socket AM5","s4":"24 cœurs · 6.0 GHz · Socket LGA1700",
    "s5":"2×16GB · 6000MHz CL30 · RGB","s6":"2×8GB · 5600MHz CL36",
    "s7":"Gen4 · 7400 MB/s · Dissipateur","s8":"Gen4 · 7000 MB/s · M.2",
    "s9":"80+ Gold · Modulaire · ATX 3.0","s10":"80+ Bronze · Semi-modulaire",
    "s11":"LGA1700 · DDR5 · PCIe 5.0 · Wi-Fi 6E","s12":"AM5 · DDR5 · PCIe 4.0",
    "s13":"Verre trempé · 3 ventilateurs RGB · ATX","s14":"Radiateur 360mm · ARGB · 2500 RPM",
    "s15":"Hot-swap · Switches linéaires · Châssis alu","s16":"58g · Polling 8000Hz · Capteur 32K DPI",
    "s17":"Surround 7.1 · Drivers 50mm · Batterie 60h","s18":"27\" QHD · 240Hz · 0.5ms · Dalle IPS",
    "s19":"Accoudoirs 4D · Soutien lombaire · Inclinaison 160°","s20":"900×400mm · Base antidérapante · Bords cousus",
    "build.tag":"Config sur mesure","build.h2":"Monté Selon <span>Tes Specs</span>",
    "build.p":"Dis-nous ton budget et les jeux auxquels tu joues. Nos techs choisissent les pièces, montent, stress-testent et expédient — configuré, câblé proprement et prêt à brancher.",
    "build.l1":"Session live gratuite avec un technicien","build.l2":"Test de burn-in 48h avant expédition","build.l3":"Cable management + réglage du profil RGB","build.l4":"Garantie 3 ans pièces & main d'œuvre","build.btn":"Démarrer ma config",
    "stores.tag":"Nos magasins","stores.h2":"Viens <span>Tester</span>","stores.p":"Deux showrooms, deux wilayas. Viens essayer le matos avant d'acheter.",
    "st1.city":"Alger","st1.name":"Mohammadia Mall","st1.p":"Showroom niveau 2 — démos, tests de configs et retrait de commande sur place.",
    "st2.city":"Sétif","st2.name":"ParkMall Sétif","st2.p":"Espace gaming — setup de test, accessoires en stock et conseil technique direct.",
    "why.tag":"Pourquoi Gaming Zone","why.h2":"Zéro Compromis. <span>Jamais.</span>","why.p":"On ne stocke que du matos qu'on mettrait dans nos propres configs.",
    "why.1t":"Livraison Express","why.1p":"Livraison 58 wilayas, suivi de bout en bout, paiement à la réception.",
    "why.2t":"Garantie 3 ans","why.2p":"Pièces et main d'œuvre couvertes. Pas de petites lignes, pas de pièges.",
    "why.3t":"Experts 24/7","why.3p":"De vrais gamers au support, jour et nuit — chat, téléphone ou WhatsApp.",
    "why.4t":"Retour 30 jours","why.4p":"Tu changes d'avis ? Renvoie sous 30 jours, sans justification.",
    "rev.tag":"Avis","rev.h2":"Les Joueurs <span>Parlent</span>","rev.p":"4.9/5 sur plus de 12 400 commandes vérifiées.",
    "rev.1":"Commandé le TITAN X9. Livré en 2 jours à Alger, câblage parfait, fiche de benchmark dans le carton. Les FPS sont fous.","rev.1s":"Acheteur vérifié · Alger",
    "rev.2":"Le support m'a aidé à choisir les pièces selon mon budget au lieu de m'upseller. Premier shop qui est vraiment de mon côté.","rev.2s":"Acheteur vérifié · Sétif",
    "rev.3":"Le casque Echo 7 est irréel, le micro est clair et la batterie dure une éternité. L'emballage aussi est premium.","rev.3s":"Acheteur vérifié · Oran",
    "news.h2":"Sois Le Premier Informé","news.p":"Restocks, guides de build et offres réservées aux membres. Zéro spam.","news.ph":"ton@email.com","news.btn":"S'abonner",
    "ct.h2":"Parle À Un <span>Vrai Gamer</span>","ct.p":"Une question sur une config, la livraison ou la garantie ? On répond en moins de 2h sur WhatsApp.",
    "ct.call":"Appelle-nous","ct.mail":"Email","ct.show":"Showrooms","ct.hours":"Horaires","ct.hoursv":"En ligne 24/7",
    "fm.name":"Ton nom","fm.nameph":"Karim Benali","fm.tel":"Téléphone","fm.telph":"0555 00 00 00","fm.budget":"Budget","fm.budgetph":"ex : 150 000 DA",
    "fm.msg":"Message","fm.msgph":"Dis-nous à quoi tu joues et ce qu'il te faut...","fm.btn":"Envoyer sur WhatsApp",
    "ft.p":"Composants et gear pro pour les joueurs qui prennent ça au sérieux. Testé et expédié par des gamers.",
    "ft.shop":"Boutique","ft.pc":"PC Gaming","ft.sup":"Support","ft.ship":"Livraison","ft.war":"Garantie","ft.ret":"Retours",
    "ft.co":"Société","ft.about":"À propos","ft.custom":"Configs sur mesure","ft.car":"Carrières","ft.press":"Presse",
    "ft.copy":"© 2026 Gaming Zone — Mohammadia Mall Alger · ParkMall Sétif","ft.legal":"Confidentialité · CGV · Cookies",
    "dr.title":"Ton panier","dr.total":"Total","dr.order":"Commander","dr.empty":"Ton panier est vide.<br>Ajoute du gear pour commencer.",
    "md.title":"Finaliser la commande","md.note":"Le récap complet sera envoyé directement sur notre WhatsApp. On confirme le stock et les frais de livraison avant expédition.",
    "md.store":"Magasin","md.name":"Nom & prénom","md.wil":"Wilaya","md.city":"Commune","md.addr":"Adresse","md.addrph":"Cité, rue, n°...",
    "md.ship":"Mode de livraison","md.home":"À domicile","md.office":"Au bureau","md.opt":"Note (optionnel)","md.optph":"Heure d'appel, repère...","md.send":"Envoyer la commande",
    "t.added":"ajouté au panier","t.empty":"Ton panier est vide","t.req":"Nom et téléphone obligatoires","t.wa":"Redirection vers WhatsApp...",
    "t.sent":"Message prêt sur WhatsApp","t.sub":"Inscrit ! Bienvenue",
    "wa.msg":"Bonjour GAMING ZONE, j'ai une question",
    "ord.title":"🛒 NOUVELLE COMMANDE — GAMING ZONE","ord.store":"Magasin","ord.name":"Nom","ord.tel":"Téléphone","ord.wil":"Wilaya",
    "ord.city":"Commune","ord.addr":"Adresse","ord.ship":"Livraison","ord.items":"── PRODUITS ──","ord.total":"TOTAL","ord.note":"Note",
    "ord.end":"Merci de confirmer ma commande ✅","ord.home":"Domicile","ord.office":"Bureau / stopdesk",
    "msg.title":"📩 MESSAGE — GAMING ZONE","msg.budget":"Budget"
  },
  en:{
    "nav.shop":"Shop","nav.custom":"Custom Build","nav.stores":"Stores","nav.why":"Why Us","nav.contact":"Contact",
    "hero.tag":"Premium gaming components · Algeria","hero.t1":"Build Your","hero.t2":"Ultimate Rig",
    "hero.p":"Hand-picked gaming components and peripherals. Build your PC part by part. Delivery to all 58 wilayas, 3-year warranty.",
    "hero.b1":"Shop Now","hero.b2":"Custom Build","hero.scroll":"Scroll",
    "stat.1":"Builds Delivered","stat.2":"Happy Gamers","stat.3":"SKUs",
    "mq.1":"RTX POWERED","mq.2":"58 WILAYAS DELIVERY","mq.3":"3 YEAR WARRANTY","mq.4":"24/7 SUPPORT","mq.5":"BENCHMARK TESTED",
    "shop.tag":"Catalog","shop.h2":"Components <span>&amp; Gear</span>","shop.p":"Every part sold separately. Pick your components and build your machine.",
    "f.all":"All","f.gpu":"Graphics Cards","f.cpu":"Processors","f.ram":"RAM","f.ssd":"SSD","f.psu":"Power Supplies","f.mobo":"Motherboards","f.case":"Cases","f.cool":"Cooling","f.kb":"Keyboards","f.mouse":"Mice","f.audio":"Headsets","f.display":"Monitors","f.chair":"Chairs","f.desk":"Desk Mats",
    "b.best":"Best Seller","b.new":"New","b.hot":"Hot","b.pro":"Pro","b.comfort":"Comfort",
    "s1":"12GB GDDR6 · Triple fan · 1080p","s2":"12GB GDDR6X · Dual fan · 1440p",
    "s3":"8 cores · 3D V-Cache · AM5 socket","s4":"24 cores · 6.0 GHz · LGA1700 socket",
    "s5":"2×16GB · 6000MHz CL30 · RGB","s6":"2×8GB · 5600MHz CL36",
    "s7":"Gen4 · 7400 MB/s · Heatsink","s8":"Gen4 · 7000 MB/s · M.2",
    "s9":"80+ Gold · Modular · ATX 3.0","s10":"80+ Bronze · Semi-modular",
    "s11":"LGA1700 · DDR5 · PCIe 5.0 · Wi-Fi 6E","s12":"AM5 · DDR5 · PCIe 4.0",
    "s13":"Tempered glass · 3 RGB fans · ATX","s14":"360mm radiator · ARGB · 2500 RPM",
    "s15":"Hot-swap · Linear switches · Full aluminum","s16":"58g · 8000Hz polling · 32K DPI optical",
    "s17":"7.1 surround · 50mm drivers · 60h battery","s18":"27\" QHD · 240Hz · 0.5ms · IPS",
    "s19":"4D armrests · Lumbar support · Recline 160°","s20":"900×400mm · Non-slip base · Stitched edges",
    "build.tag":"Custom Config","build.h2":"Built To <span>Your Spec</span>",
    "build.p":"Tell us your budget and the games you play. Our techs pick parts, assemble, stress-test and ship — fully configured, cable-managed and ready to plug in.",
    "build.l1":"Free live build session with a technician","build.l2":"48-hour burn-in test before shipping","build.l3":"Cable management + RGB profile tuning","build.l4":"3-year parts & labour warranty","build.btn":"Start My Build",
    "stores.tag":"Our Stores","stores.h2":"Come <span>Test It</span>","stores.p":"Two showrooms, two wilayas. Try the gear before you buy.",
    "st1.city":"Algiers","st1.name":"Mohammadia Mall","st1.p":"Level 2 showroom — demos, build testing and in-store order pickup.",
    "st2.city":"Sétif","st2.name":"ParkMall Sétif","st2.p":"Gaming space — test setup, accessories in stock and direct technical advice.",
    "why.tag":"Why Gaming Zone","why.h2":"No Compromise. <span>Ever.</span>","why.p":"We only stock hardware we would put in our own rigs.",
    "why.1t":"Express Delivery","why.1p":"Delivery to all 58 wilayas, tracked door to door, cash on delivery.",
    "why.2t":"3-Year Cover","why.2p":"Parts and labour covered. No fine print, no restocking games.",
    "why.3t":"24/7 Experts","why.3p":"Real gamers on support, day or night — chat, phone or WhatsApp.",
    "why.4t":"30-Day Returns","why.4p":"Changed your mind? Send it back within 30 days, no questions asked.",
    "rev.tag":"Reviews","rev.h2":"Players <span>Talk</span>","rev.p":"4.9/5 from 12,400+ verified orders.",
    "rev.1":"Ordered the TITAN X9. Arrived in 2 days in Algiers, cable managed perfectly, benchmark sheet in the box. Frames are insane.","rev.1s":"Verified buyer · Algiers",
    "rev.2":"Support helped me pick parts for my budget instead of upselling. First shop that actually felt on my side.","rev.2s":"Verified buyer · Sétif",
    "rev.3":"The Echo 7 headset is unreal, the mic is clear and the battery lasts forever. Packaging felt premium too.","rev.3s":"Verified buyer · Oran",
    "news.h2":"Get The Drop First","news.p":"Restocks, build guides and members-only deals. No spam.","news.ph":"you@email.com","news.btn":"Subscribe",
    "ct.h2":"Talk To A <span>Real Gamer</span>","ct.p":"Questions about a build, delivery or warranty? We answer in under 2h on WhatsApp.",
    "ct.call":"Call us","ct.mail":"Email","ct.show":"Showrooms","ct.hours":"Hours","ct.hoursv":"Online 24/7",
    "fm.name":"Your name","fm.nameph":"John Doe","fm.tel":"Phone","fm.telph":"0555 00 00 00","fm.budget":"Budget","fm.budgetph":"e.g. 150,000 DA",
    "fm.msg":"Message","fm.msgph":"Tell us what you play and what you need...","fm.btn":"Send on WhatsApp",
    "ft.p":"Pro components and gear for players who take it seriously. Tested and shipped by gamers.",
    "ft.shop":"Shop","ft.pc":"Gaming PCs","ft.sup":"Support","ft.ship":"Shipping","ft.war":"Warranty","ft.ret":"Returns",
    "ft.co":"Company","ft.about":"About","ft.custom":"Custom Builds","ft.car":"Careers","ft.press":"Press",
    "ft.copy":"© 2026 Gaming Zone — Mohammadia Mall Algiers · ParkMall Sétif","ft.legal":"Privacy · Terms · Cookies",
    "dr.title":"Your cart","dr.total":"Total","dr.order":"Order","dr.empty":"Your cart is empty.<br>Add some gear to start.",
    "md.title":"Complete your order","md.note":"The full summary will be sent straight to our WhatsApp. We confirm stock and delivery fees before shipping.",
    "md.store":"Store","md.name":"Full name","md.wil":"Wilaya","md.city":"City","md.addr":"Address","md.addrph":"Street, number...",
    "md.ship":"Delivery method","md.home":"To my door","md.office":"To office","md.opt":"Note (optional)","md.optph":"Call time, landmark...","md.send":"Send order",
    "t.added":"added to cart","t.empty":"Your cart is empty","t.req":"Name and phone required","t.wa":"Redirecting to WhatsApp...",
    "t.sent":"Message ready on WhatsApp","t.sub":"Subscribed! Welcome aboard",
    "wa.msg":"Hello GAMING ZONE, I have a question",
    "ord.title":"🛒 NEW ORDER — GAMING ZONE","ord.store":"Store","ord.name":"Name","ord.tel":"Phone","ord.wil":"Wilaya",
    "ord.city":"City","ord.addr":"Address","ord.ship":"Delivery","ord.items":"── ITEMS ──","ord.total":"TOTAL","ord.note":"Note",
    "ord.end":"Please confirm my order ✅","ord.home":"Home","ord.office":"Office / stopdesk",
    "msg.title":"📩 MESSAGE — GAMING ZONE","msg.budget":"Budget"
  },
  ar:{
    "nav.shop":"المتجر","nav.custom":"تجميع خاص","nav.stores":"المتاجر","nav.why":"لماذا نحن","nav.contact":"اتصل بنا",
    "hero.tag":"قطع قيمينغ بريميوم · الجزائر","hero.t1":"ابنِ","hero.t2":"جهازك المثالي",
    "hero.p":"قطع وملحقات قيمينغ مختارة بعناية. جمّع جهازك قطعة قطعة. توصيل لكل 58 ولاية، ضمان 3 سنوات.",
    "hero.b1":"اشترِ الآن","hero.b2":"تجميع على المقاس","hero.scroll":"انزل",
    "stat.1":"جهاز تم تسليمه","stat.2":"لاعب راضٍ","stat.3":"منتج",
    "mq.1":"بقوة RTX","mq.2":"توصيل 58 ولاية","mq.3":"ضمان 3 سنوات","mq.4":"دعم 24/7","mq.5":"مُختبَر بالبنشمارك",
    "shop.tag":"الكتالوغ","shop.h2":"قطع <span>وإكسسوارات</span>","shop.p":"كل قطعة وحدها. اختر قطعك وابنِ جهازك.",
    "f.all":"الكل","f.gpu":"كروت شاشة","f.cpu":"معالجات","f.ram":"رام","f.ssd":"أقراص SSD","f.psu":"مزوّدات طاقة","f.mobo":"لوحات أم","f.case":"صناديق","f.cool":"تبريد","f.kb":"كيبورد","f.mouse":"فأرة","f.audio":"سماعات","f.display":"شاشات","f.chair":"كراسي","f.desk":"موائد",
    "b.best":"الأكثر مبيعًا","b.new":"جديد","b.hot":"مطلوب","b.pro":"احترافي","b.comfort":"راحة",
    "s1":"12GB GDDR6 · 3 مراوح · 1080p","s2":"12GB GDDR6X · مروحتان · 1440p",
    "s3":"8 أنوية · 3D V-Cache · مقبس AM5","s4":"24 نواة · 6.0 GHz · مقبس LGA1700",
    "s5":"2×16GB · 6000MHz CL30 · RGB","s6":"2×8GB · 5600MHz CL36",
    "s7":"Gen4 · 7400 MB/s · مشتت","s8":"Gen4 · 7000 MB/s · M.2",
    "s9":"80+ Gold · معياري · ATX 3.0","s10":"80+ Bronze · نصف معياري",
    "s11":"LGA1700 · DDR5 · PCIe 5.0 · Wi-Fi 6E","s12":"AM5 · DDR5 · PCIe 4.0",
    "s13":"زجاج مقسى · 3 مراوح RGB · ATX","s14":"رادياتور 360mm · ARGB · 2500 RPM",
    "s15":"تبديل سريع · مفاتيح لينة · هيكل ألمنيوم","s16":"58 غرام · 8000Hz · مستشعر 32K DPI",
    "s17":"محيط 7.1 · درايفر 50mm · بطارية 60 ساعة","s18":"27\" QHD · 240Hz · 0.5ms · IPS",
    "s19":"مساند 4D · دعم قطني · استلقاء 160°","s20":"900×400mm · قاعدة مانعة للانزلاق · حواف مخيطة",
    "build.tag":"تجميع خاص","build.h2":"مبني <span>حسب مواصفاتك</span>",
    "build.p":"قلنا ميزانيتك والألعاب اللي تلعبها. تقنيّونا يختاروا القطع، يجمّعوا، يجربوا الضغط ويعيّطوا — مجهّز ومنظّم وجاهز للتوصيل.",
    "build.l1":"جلسة مباشرة مجانية مع تقني","build.l2":"اختبار تحمّل 48 ساعة قبل الإرسال","build.l3":"تنظيم الكوابل وضبط إضاءة RGB","build.l4":"ضمان 3 سنوات على القطع واليد العاملة","build.btn":"ابدأ تجميعي",
    "stores.tag":"متاجرنا","stores.h2":"تعال <span>جرّب</span>","stores.p":"صالتان عرض، ولايتان. جرّب العتاد قبل ما تشري.",
    "st1.city":"الجزائر","st1.name":"محمدية مول","st1.p":"صالة عرض الطابق الثاني — تجارب، اختبار أجهزة واستلام الطلبات في المكان.",
    "st2.city":"سطيف","st2.name":"بارك مول سطيف","st2.p":"فضاء قيمينغ — تجهيزة للتجربة، إكسسوارات متوفرة ونصيحة تقنية مباشرة.",
    "why.tag":"لماذا قيمينغ زون","why.h2":"بلا تنازلات. <span>أبدًا.</span>","why.p":"نخزّن غير العتاد اللي نحطوه في أجهزتنا.",
    "why.1t":"توصيل سريع","why.1p":"توصيل لكل 58 ولاية، تتبّع كامل، والدفع عند الاستلام.",
    "why.2t":"ضمان 3 سنوات","why.2p":"القطع واليد العاملة مغطاة. بلا شروط خفية.",
    "why.3t":"خبراء 24/7","why.3p":"قيمرز حقيقيين في الدعم، ليل ونهار — شات، تيليفون ولا واتساب.",
    "why.4t":"إرجاع 30 يوم","why.4p":"بدّلت رأيك؟ رجّعها في 30 يوم بلا أسئلة.",
    "rev.tag":"آراء","rev.h2":"اللاعبون <span>يتكلمون</span>","rev.p":"4.9/5 من أكثر من 12400 طلب موثّق.",
    "rev.1":"طلبت TITAN X9. وصل في يومين للجزائر، تنظيم كوابل مثالي، وورقة بنشمارك في الكرطون. الإطارات جنونية.","rev.1s":"مشترٍ موثّق · الجزائر",
    "rev.2":"الدعم عاوني نختار القطع حسب ميزانيتي بلا ما يبيعلي الغالي. أول محل حسيته معايا.","rev.2s":"مشترٍ موثّق · سطيف",
    "rev.3":"سماعة Echo 7 خارقة، المايك واضح والبطارية تدوم بزاف. التغليف حتى هو بريميوم.","rev.3s":"مشترٍ موثّق · وهران",
    "news.h2":"كن أول من يعرف","news.p":"إعادة التوفير، أدلة التجميع وعروض للأعضاء فقط. بلا سبام.","news.ph":"بريدك@إيميل.com","news.btn":"اشترك",
    "ct.h2":"اهدر مع <span>قيمر حقيقي</span>","ct.p":"سؤال على جهاز، توصيل ولا ضمان؟ نجاوبو في أقل من ساعتين على واتساب.",
    "ct.call":"اتصل بنا","ct.mail":"الإيميل","ct.show":"صالات العرض","ct.hours":"أوقات العمل","ct.hoursv":"متصلين 24/7",
    "fm.name":"اسمك","fm.nameph":"كريم بن علي","fm.tel":"الهاتف","fm.telph":"0555 00 00 00","fm.budget":"الميزانية","fm.budgetph":"مثال: 150000 دج",
    "fm.msg":"الرسالة","fm.msgph":"قلنا واش تلعب وواش تحتاج...","fm.btn":"أرسل على واتساب",
    "ft.p":"قطع وعتاد احترافي للاعبين اللي ياخدوها بجدية. مختبَر ومرسَل من قيمرز.",
    "ft.shop":"المتجر","ft.pc":"أجهزة","ft.sup":"الدعم","ft.ship":"التوصيل","ft.war":"الضمان","ft.ret":"الإرجاع",
    "ft.co":"الشركة","ft.about":"من نحن","ft.custom":"تجميع خاص","ft.car":"وظائف","ft.press":"صحافة",
    "ft.copy":"© 2026 قيمينغ زون — محمدية مول الجزائر · بارك مول سطيف","ft.legal":"الخصوصية · الشروط · الكوكيز",
    "dr.title":"سلّتك","dr.total":"المجموع","dr.order":"اطلب","dr.empty":"سلّتك فارغة.<br>زيد عتاد باش تبدا.",
    "md.title":"إتمام الطلب","md.note":"الملخص الكامل يُرسل مباشرة لواتساب. نأكدوا التوفر ومصاريف التوصيل قبل الإرسال.",
    "md.store":"المتجر","md.name":"الاسم الكامل","md.wil":"الولاية","md.city":"البلدية","md.addr":"العنوان","md.addrph":"حي، شارع، رقم...",
    "md.ship":"طريقة التوصيل","md.home":"للباب","md.office":"للمكتب","md.opt":"ملاحظة (اختياري)","md.optph":"وقت الاتصال، علامة...","md.send":"أرسل الطلب",
    "t.added":"أُضيف للسلة","t.empty":"سلّتك فارغة","t.req":"الاسم والهاتف إلزاميين","t.wa":"جارٍ التحويل لواتساب...",
    "t.sent":"الرسالة جاهزة على واتساب","t.sub":"تم الاشتراك! مرحبًا بك",
    "wa.msg":"مرحبا قيمينغ زون، عندي سؤال",
    "ord.title":"🛒 طلب جديد — قيمينغ زون","ord.store":"المتجر","ord.name":"الاسم","ord.tel":"الهاتف","ord.wil":"الولاية",
    "ord.city":"البلدية","ord.addr":"العنوان","ord.ship":"التوصيل","ord.items":"── المنتجات ──","ord.total":"المجموع","ord.note":"ملاحظة",
    "ord.end":"رجاءً أكّدوا طلبي ✅","ord.home":"للباب","ord.office":"مكتب / ستوب ديسك",
    "msg.title":"📩 رسالة — قيمينغ زون","msg.budget":"الميزانية"
  }
};

let lang = localStorage.getItem('gz_lang') || 'fr';
const t = k => (I18N[lang] && I18N[lang][k]) || (I18N.fr[k] || k);

function applyLang(l){
  lang = l;
  localStorage.setItem('gz_lang', l);
  const rtl = l === 'ar';
  document.documentElement.lang = l;
  document.documentElement.dir = rtl ? 'rtl' : 'ltr';

  $$('[data-i18n]').forEach(el=> el.textContent = t(el.dataset.i18n));
  $$('[data-i18n-html]').forEach(el=> el.innerHTML = t(el.dataset.i18nHtml));
  $$('[data-i18n-ph]').forEach(el=> el.placeholder = t(el.dataset.i18nPh));

  $('#heroTitle').innerHTML = t('hero.t1') + '<br><em>' + t('hero.t2') + '</em>';

  const mq = [];
  for(let i=0;i<2;i++) for(let n=1;n<=5;n++) mq.push('<span><i class="fas fa-bolt"></i>' + t('mq.'+n) + '</span>');
  $('#marquee').innerHTML = mq.join('');

  $('#waBubble').href = 'https://wa.me/' + WA.alger + '?text=' + encodeURIComponent(t('wa.msg'));

  $$('.langs button').forEach(b=> b.classList.toggle('on', b.dataset.lang === l));
  renderCart();
}

$$('.langs button').forEach(b=> b.onclick = ()=> applyLang(b.dataset.lang));

addEventListener('load', ()=> setTimeout(()=>$('#loader').classList.add('gone'), 500));

addEventListener('scroll', ()=>{
  const h = document.documentElement;
  $('#prog').style.width = (h.scrollTop / (h.scrollHeight - h.clientHeight) * 100) + '%';
  $('#hdr').classList.toggle('small', scrollY > 40);
});

$('#burger').onclick = ()=>{
  const m = $('#menu'), open = m.style.display === 'flex';
  m.style.display = open ? 'none' : 'flex';
  if(!open) m.style.cssText = 'display:flex;position:absolute;top:100%;left:0;right:0;flex-direction:column;gap:0;background:#141417;padding:18px 24px;border-bottom:2px solid #ff1f2e';
};

const io = new IntersectionObserver(e=>e.forEach(x=>{ if(x.isIntersecting){ x.target.classList.add('in'); io.unobserve(x.target); }}),{threshold:.12});
$$('.rv').forEach(el=>io.observe(el));

const cur = $('#cur'), curd = $('#curd');
let cx=0, cy=0, dx=0, dy=0;
addEventListener('mousemove', e=>{ cx=e.clientX; cy=e.clientY; curd.style.transform=`translate(${cx-3}px,${cy-3}px)`; });
(function loop(){ dx+=(cx-dx)*.16; dy+=(cy-dy)*.16; cur.style.transform=`translate(${dx-19}px,${dy-19}px)`; requestAnimationFrame(loop); })();
$$('a,button,.card,.box,.review').forEach(el=>{
  el.addEventListener('mouseenter',()=>cur.classList.add('hot'));
  el.addEventListener('mouseleave',()=>cur.classList.remove('hot'));
});

$$('.card').forEach(c=>{
  c.addEventListener('mousemove', e=>{
    const r = c.getBoundingClientRect();
    c.style.setProperty('--mx', (e.clientX-r.left)+'px');
    c.style.setProperty('--my', (e.clientY-r.top)+'px');
  });
});

function count(id, end){
  const el = $(id); let n = 0; const step = end/70;
  const tm = setInterval(()=>{ n+=step; if(n>=end){ el.textContent = end.toLocaleString('fr-FR')+'+'; clearInterval(tm);} else el.textContent = Math.floor(n).toLocaleString('fr-FR'); }, 22);
}
new IntersectionObserver((e,o)=>e.forEach(x=>{ if(x.isIntersecting){ count('#c1',18400); count('#c2',15200); count('#c3',640); o.disconnect(); }}),{threshold:.4}).observe($('.hero-stats'));

const toast = $('#toast');
function showToast(msg){ $('#toastTxt').textContent = msg; toast.classList.add('on'); clearTimeout(showToast.t); showToast.t = setTimeout(()=>toast.classList.remove('on'), 2400); }

let cart = {};
try { cart = JSON.parse(localStorage.getItem('gz_cart') || '{}'); } catch(e){ cart = {}; }
const save = ()=> localStorage.setItem('gz_cart', JSON.stringify(cart));

function totalQty(){ return Object.values(cart).reduce((a,b)=>a+b.qty,0); }
function totalPrice(){ return Object.values(cart).reduce((a,b)=>a+b.qty*b.price,0); }

function renderCart(){
  const list = $('#drList');
  const items = Object.entries(cart);
  $('#cartCount').textContent = totalQty();
  $('#drTotal').textContent = fmt(totalPrice());
  if(!items.length){
    list.innerHTML = '<div class="empty"><i class="fas fa-cart-shopping"></i>' + t('dr.empty') + '</div>';
    return;
  }
  list.innerHTML = items.map(([id,it])=>`
    <div class="ci">
      <div class="ico">${it.img ? `<img src="${it.img}" alt="">` : '<i class="fas fa-box"></i>'}</div>
      <div class="nm">${it.name}<small>${fmt(it.price)}</small></div>
      <div class="qty">
        <button data-dec="${id}">−</button><span>${it.qty}</span><button data-inc="${id}">+</button>
      </div>
    </div>`).join('');
}

$('#drList').addEventListener('click', e=>{
  const inc = e.target.closest('[data-inc]'), dec = e.target.closest('[data-dec]');
  if(inc){ const id = inc.dataset.inc; cart[id].qty++; save(); renderCart(); }
  if(dec){ const id = dec.dataset.dec; cart[id].qty--; if(cart[id].qty<=0) delete cart[id]; save(); renderCart(); }
});

$$('.add').forEach(b=>b.onclick = ()=>{
  const card = b.closest('.card');
  const {id, name, price} = card.dataset;
  const img = card.querySelector('.thumb img')?.getAttribute('src') || '';
  cart[id] = cart[id] || {name, price:+price, qty:0, img};
  cart[id].qty++; save(); renderCart();
  const cc = $('#cartCount'); cc.parentElement.classList.add('bump');
  setTimeout(()=>cc.parentElement.classList.remove('bump'), 500);
  showToast(name + ' ' + t('t.added'));
});

function openDrawer(){ renderCart(); $('#drawer').classList.add('on'); $('#scrim').classList.add('on'); document.body.classList.add('locked'); }
function closeDrawer(){ $('#drawer').classList.remove('on'); $('#scrim').classList.remove('on'); document.body.classList.remove('locked'); }
$('#cartBtn').onclick = openDrawer;
$('#drClose').onclick = closeDrawer;
$('#scrim').onclick = closeDrawer;

const wilayas = ["Adrar","Chlef","Laghouat","Oum El Bouaghi","Batna","Béjaïa","Biskra","Béchar","Blida","Bouira","Tamanrasset","Tébessa","Tlemcen","Tiaret","Tizi Ouzou","Alger","Djelfa","Jijel","Sétif","Saïda","Skikda","Sidi Bel Abbès","Annaba","Guelma","Constantine","Médéa","Mostaganem","M'Sila","Mascara","Ouargla","Oran","El Bayadh","Illizi","Bordj Bou Arreridj","Boumerdès","El Tarf","Tindouf","Tissemsilt","El Oued","Khenchela","Souk Ahras","Tipaza","Mila","Aïn Defla","Naâma","Aïn Témouchent","Ghardaïa","Relizane","Timimoun","Bordj Badji Mokhtar","Ouled Djellal","Béni Abbès","In Salah","In Guezzam","Touggourt","Djanet","El M'Ghair","El Meniaa"];
$('#fWilaya').innerHTML = wilayas.map(w=>`<option${w==='Alger'?' selected':''}>${w}</option>`).join('');

$('#toCheckout').onclick = ()=>{
  if(!totalQty()) return showToast(t('t.empty'));
  closeDrawer();
  $('#modal').classList.add('on');
  document.body.classList.add('locked');
};
function closeModal(){ $('#modal').classList.remove('on'); document.body.classList.remove('locked'); }
$('#mClose').onclick = closeModal;

$('#sendWa').onclick = ()=>{
  const name = $('#fName').value.trim();
  const tel = $('#fTel').value.trim();
  const wil = $('#fWilaya').value;
  const city = $('#fCity').value.trim();
  const addr = $('#fAddr').value.trim();
  const note = $('#fNote').value.trim();
  const store = document.querySelector('input[name="store"]:checked').value;
  const ship = document.querySelector('input[name="ship"]:checked').value === 'office' ? t('ord.office') : t('ord.home');

  if(!name || !tel){ showToast(t('t.req')); return; }
  if(!Object.keys(cart).length){ showToast(t('t.empty')); return; }

  let msg = '*' + t('ord.title') + '*\n\n';
  msg += '*' + t('ord.store') + ' :* ' + store + '\n';
  msg += '*' + t('ord.name') + ' :* ' + name + '\n';
  msg += '*' + t('ord.tel') + ' :* ' + tel + '\n';
  msg += '*' + t('ord.wil') + ' :* ' + wil + '\n';
  if(city) msg += '*' + t('ord.city') + ' :* ' + city + '\n';
  if(addr) msg += '*' + t('ord.addr') + ' :* ' + addr + '\n';
  msg += '*' + t('ord.ship') + ' :* ' + ship + '\n';
  msg += '\n*' + t('ord.items') + '*\n';
  Object.values(cart).forEach(it=>{ msg += `• ${it.qty} x ${it.name} — ${fmt(it.price*it.qty)}\n`; });
  msg += '\n*' + t('ord.total') + ' : ' + fmt(totalPrice()) + '*\n';
  if(note) msg += '\n*' + t('ord.note') + ' :* ' + note + '\n';
  msg += '\n' + t('ord.end');

  const num = store.startsWith('Sétif') ? WA.setif : WA.alger;
  window.open('https://wa.me/' + num + '?text=' + encodeURIComponent(msg), '_blank');
  showToast(t('t.wa'));
  setTimeout(()=>{ closeModal(); cart = {}; save(); renderCart(); }, 900);
};

$('#cform').onsubmit = e=>{
  e.preventDefault();
  const f = e.target;
  const msg = '*' + t('msg.title') + '*\n\n' + t('ord.name') + ' : ' + f.nom.value + '\n' + t('ord.tel') + ' : ' + f.tel.value + '\n' + t('msg.budget') + ' : ' + (f.budget.value || '—') + '\n\n' + f.msg.value;
  window.open('https://wa.me/' + WA.alger + '?text=' + encodeURIComponent(msg), '_blank');
  f.reset();
  showToast(t('t.sent'));
};

$('#newsForm').onsubmit = e=>{ e.preventDefault(); e.target.reset(); showToast(t('t.sub')); };

$$('.filters button').forEach(b=>b.onclick = ()=>{
  $$('.filters button').forEach(x=>x.classList.remove('on'));
  b.classList.add('on');
  const f = b.dataset.f;
  $$('.card').forEach(c=>{
    const ok = f === 'all' || c.dataset.c === f;
    c.style.display = ok ? 'flex' : 'none';
    if(ok){ c.classList.remove('in'); requestAnimationFrame(()=>c.classList.add('in')); }
  });
});

$$('a[href^="#"]').forEach(a=>a.onclick = e=>{
  const tgt = document.querySelector(a.getAttribute('href'));
  if(tgt){ e.preventDefault(); tgt.scrollIntoView({behavior:'smooth'}); }
});

applyLang(lang);
</script>
</body>
</html>
