<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Bhadu Solar Energy | Rajasthan, India</title>
<link href="https://fonts.googleapis.com/css2?family=Tiro+Devanagari+Hindi&family=Syne:wght@700;800&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
:root {
  --gold: #F5A623;
  --amber: #E8622A;
  --cream: #FFF8EC;
  --ink: #0C1220;
  --navy: #111C2E;
  --slate: #1A2840;
  --muted: rgba(255,255,255,0.5);
  --border: rgba(255,255,255,0.08);
}
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;font-size:16px;}
body{
  font-family:'DM Sans',sans-serif;
  background:var(--ink);
  color:#fff;
  overflow-x:hidden;
  cursor:none;
}

/* ─── CUSTOM CURSOR ─── */
.cursor{
position:fixed;width:12px;height:12px;border-radius:50%;
background:var(–gold);pointer-events:none;z-index:9999;
transform:translate(-50%,-50%);transition:transform .1s;
mix-blend-mode:difference;
}
.cursor-ring{
position:fixed;width:38px;height:38px;border-radius:50%;
border:1.5px solid rgba(245,166,35,0.5);pointer-events:none;z-index:9998;
transform:translate(-50%,-50%);transition:all .18s ease;
}

/* ─── NOISE OVERLAY ─── */
body::after{
content:’’;position:fixed;inset:0;
background-image:url(“data:image/svg+xml,%3Csvg viewBox=‘0 0 256 256’ xmlns=‘http://www.w3.org/2000/svg’%3E%3Cfilter id=‘n’%3E%3CfeTurbulence type=‘fractalNoise’ baseFrequency=‘0.9’ numOctaves=‘4’ stitchTiles=‘stitch’/%3E%3C/filter%3E%3Crect width=‘100%25’ height=‘100%25’ filter=‘url(%23n)’ opacity=‘0.04’/%3E%3C/svg%3E”);
pointer-events:none;z-index:9990;opacity:.4;
}

/* ─── NAVBAR ─── */
nav{
position:fixed;top:0;width:100%;z-index:1000;
padding:20px 64px;
display:flex;align-items:center;justify-content:space-between;
transition:background .4s,backdrop-filter .4s;
}
nav.scrolled{
background:rgba(11,18,32,0.92);
backdrop-filter:blur(20px);
border-bottom:1px solid var(–border);
}
.logo-wrap{display:flex;align-items:center;gap:14px;}
.logo-icon{
width:44px;height:44px;border-radius:12px;
background:linear-gradient(135deg,var(–gold),var(–amber));
display:flex;align-items:center;justify-content:center;
font-size:1.4rem;flex-shrink:0;
box-shadow:0 0 20px rgba(245,166,35,.35);
}
.logo-text{
font-family:‘Syne’,sans-serif;
font-size:1.15rem;font-weight:800;
letter-spacing:.5px;line-height:1.2;
}
.logo-text small{
display:block;font-size:.65rem;font-weight:400;
color:var(–gold);letter-spacing:2px;text-transform:uppercase;
}
nav ul{list-style:none;display:flex;gap:32px;align-items:center;}
nav ul li a{
color:rgba(255,255,255,.75);text-decoration:none;
font-size:.9rem;font-weight:500;letter-spacing:.5px;
transition:color .25s;
}
nav ul li a:hover{color:var(–gold);}
.nav-btn{
background:linear-gradient(135deg,var(–gold),var(–amber));
color:var(–ink)!important;padding:10px 26px;border-radius:50px;
font-weight:600!important;font-size:.9rem!important;
box-shadow:0 4px 18px rgba(245,166,35,.3);
transition:transform .2s,box-shadow .2s!important;
}
.nav-btn:hover{transform:translateY(-2px);box-shadow:0 8px 28px rgba(245,166,35,.5)!important;}

/* ─── HERO ─── */
#hero{
position:relative;min-height:100vh;
display:grid;grid-template-columns:1fr 1fr;
overflow:hidden;
}

/* left panel – text */
.hero-left{
position:relative;z-index:5;
padding:160px 64px 80px;
display:flex;flex-direction:column;justify-content:center;
background:linear-gradient(135deg,rgba(11,18,32,.98) 0%,rgba(17,28,46,.95) 100%);
}
.hero-eyebrow{
display:inline-flex;align-items:center;gap:10px;
background:rgba(245,166,35,.1);border:1px solid rgba(245,166,35,.25);
padding:7px 18px;border-radius:50px;
font-size:.78rem;letter-spacing:2.5px;color:var(–gold);
text-transform:uppercase;margin-bottom:28px;width:fit-content;
}
.hero-eyebrow::before{content:’’;width:7px;height:7px;border-radius:50%;background:var(–gold);animation:blink 1.5s infinite;}
@keyframes blink{0%,100%{opacity:1;}50%{opacity:.2;}}

h1{
font-family:‘Syne’,sans-serif;
font-size:clamp(3rem,5.5vw,5.2rem);
font-weight:800;line-height:1.06;
margin-bottom:24px;
}
h1 .line-gold{
background:linear-gradient(100deg,#FFD166,var(–gold),var(–amber));
-webkit-background-clip:text;-webkit-text-fill-color:transparent;
}
.hero-desc{
font-size:1.05rem;color:rgba(255,255,255,.6);
line-height:1.75;max-width:480px;margin-bottom:40px;
}
.hero-actions{display:flex;gap:14px;flex-wrap:wrap;margin-bottom:56px;}
.btn-glow{
background:linear-gradient(135deg,var(–gold),var(–amber));
color:var(–ink);padding:15px 38px;border-radius:50px;
font-weight:700;font-size:.95rem;text-decoration:none;
box-shadow:0 8px 28px rgba(245,166,35,.4);
transition:transform .2s,box-shadow .2s;display:inline-block;
}
.btn-glow:hover{transform:translateY(-3px);box-shadow:0 14px 40px rgba(245,166,35,.55);}
.btn-ghost{
color:#fff;padding:15px 38px;border-radius:50px;
font-weight:600;font-size:.95rem;text-decoration:none;
border:1.5px solid rgba(255,255,255,.2);
transition:border-color .25s,background .25s;display:inline-block;
}
.btn-ghost:hover{border-color:var(–gold);background:rgba(245,166,35,.07);}

/* stats bar */
.hero-stats{
display:flex;gap:36px;padding-top:36px;
border-top:1px solid var(–border);flex-wrap:wrap;
}
.hs{flex:1;min-width:100px;}
.hs-num{
font-family:‘Syne’,sans-serif;font-size:2rem;font-weight:800;
background:linear-gradient(135deg,var(–gold),var(–amber));
-webkit-background-clip:text;-webkit-text-fill-color:transparent;
}
.hs-lbl{font-size:.78rem;color:rgba(255,255,255,.45);letter-spacing:1px;margin-top:2px;text-transform:uppercase;}

/* right panel – real image with overlays */
.hero-right{
position:relative;overflow:hidden;
}
.hero-img-main{
position:absolute;inset:0;
background:url(‘https://images.unsplash.com/photo-1509391366360-2e959784a276?w=1200&q=85&auto=format&fit=crop’) center/cover no-repeat;
transition:transform 8s ease;
}
#hero:hover .hero-img-main{transform:scale(1.04);}
.hero-img-overlay{
position:absolute;inset:0;
background:linear-gradient(to right,rgba(11,18,32,.6) 0%,rgba(11,18,32,.1) 60%),
linear-gradient(to top,rgba(11,18,32,.8) 0%,transparent 50%);
}

/* floating stat cards on image */
.float-card{
position:absolute;
background:rgba(11,18,32,.75);backdrop-filter:blur(16px);
border:1px solid rgba(245,166,35,.2);border-radius:16px;
padding:16px 22px;min-width:160px;
animation:floatY 4s ease-in-out infinite;
}
.float-card:nth-child(1){top:22%;right:10%;animation-delay:0s;}
.float-card:nth-child(2){bottom:28%;right:6%;animation-delay:1.5s;}
.float-card:nth-child(3){top:55%;left:4%;animation-delay:3s;}
@keyframes floatY{0%,100%{transform:translateY(0);}50%{transform:translateY(-10px);}}
.fc-label{font-size:.7rem;color:var(–gold);letter-spacing:1.5px;text-transform:uppercase;margin-bottom:4px;}
.fc-value{font-family:‘Syne’,sans-serif;font-size:1.5rem;font-weight:800;}
.fc-sub{font-size:.72rem;color:rgba(255,255,255,.45);margin-top:2px;}

/* live indicator */
.live-badge{
position:absolute;top:30px;left:30px;z-index:10;
display:flex;align-items:center;gap:8px;
background:rgba(11,18,32,.8);backdrop-filter:blur(10px);
border:1px solid rgba(34,197,94,.3);border-radius:50px;
padding:7px 16px;font-size:.78rem;color:rgba(255,255,255,.8);
}
.live-dot{width:8px;height:8px;border-radius:50%;background:#22C55E;animation:blink 1.5s infinite;}

/* scroll indicator */
.scroll-hint{
position:absolute;bottom:36px;left:50%;transform:translateX(-50%);
z-index:10;display:flex;flex-direction:column;align-items:center;gap:8px;
font-size:.72rem;color:rgba(255,255,255,.35);letter-spacing:2px;text-transform:uppercase;
}
.scroll-arrow{
width:24px;height:40px;border:1.5px solid rgba(255,255,255,.2);
border-radius:12px;display:flex;justify-content:center;padding-top:6px;
}
.scroll-arrow::after{
content:’’;width:4px;height:8px;border-radius:2px;
background:var(–gold);animation:scrollDot 1.6s infinite;
}
@keyframes scrollDot{0%{transform:translateY(0);opacity:1;}100%{transform:translateY(14px);opacity:0;}}

/* ─── SECTION COMMONS ─── */
section{padding:100px 64px;}
.tag{
display:inline-block;color:var(–gold);
font-size:.75rem;letter-spacing:3px;text-transform:uppercase;
margin-bottom:14px;font-weight:600;
}
.sec-title{
font-family:‘Syne’,sans-serif;
font-size:clamp(2rem,4vw,3.2rem);font-weight:800;
line-height:1.15;margin-bottom:16px;
}
.sec-sub{color:rgba(255,255,255,.55);font-size:1rem;max-width:540px;line-height:1.8;}

/* ─── ABOUT STRIP ─── */
#about{
background:var(–navy);
padding:60px 64px;
display:grid;grid-template-columns:repeat(4,1fr);gap:2px;
}
.about-item{
padding:40px 36px;
border-right:1px solid var(–border);
transition:background .3s;
}
.about-item:last-child{border-right:none;}
.about-item:hover{background:rgba(245,166,35,.04);}
.ai-num{
font-family:‘Syne’,sans-serif;font-size:3rem;font-weight:800;
background:linear-gradient(135deg,var(–gold),var(–amber));
-webkit-background-clip:text;-webkit-text-fill-color:transparent;
line-height:1;margin-bottom:8px;
}
.ai-title{font-weight:600;font-size:1rem;margin-bottom:6px;}
.ai-desc{color:rgba(255,255,255,.45);font-size:.88rem;line-height:1.6;}

/* ─── SERVICES ─── */
#services{background:var(–ink);}
.services-grid{
display:grid;grid-template-columns:repeat(3,1fr);gap:24px;
margin-top:60px;
}
.svc-card{
border-radius:20px;overflow:hidden;position:relative;
height:380px;cursor:pointer;
transition:transform .4s;
}
.svc-card:hover{transform:scale(1.02);}
.svc-img{
position:absolute;inset:0;background-size:cover;background-position:center;
transition:transform .6s ease;
}
.svc-card:hover .svc-img{transform:scale(1.08);}
.svc-overlay{
position:absolute;inset:0;
background:linear-gradient(to top,rgba(11,18,32,.95) 0%,rgba(11,18,32,.3) 60%,transparent 100%);
}
.svc-content{
position:absolute;bottom:0;left:0;right:0;
padding:32px;
}
.svc-icon{font-size:2rem;margin-bottom:12px;display:block;}
.svc-name{font-family:‘Syne’,sans-serif;font-size:1.3rem;font-weight:700;margin-bottom:8px;}
.svc-desc{color:rgba(255,255,255,.6);font-size:.88rem;line-height:1.6;max-height:0;overflow:hidden;transition:max-height .4s ease,opacity .4s;}
.svc-card:hover .svc-desc{max-height:100px;opacity:1;}
.svc-badge{
position:absolute;top:20px;right:20px;
background:linear-gradient(135deg,var(–gold),var(–amber));
color:var(–ink);font-size:.72rem;font-weight:700;
padding:5px 14px;border-radius:20px;
}

/* ─── PRODUCTS ─── */
#products{background:var(–navy);}
.products-layout{
display:grid;grid-template-columns:1fr 1fr;gap:60px;
align-items:start;margin-top:60px;
}
/* big product showcase */
.product-showcase{
position:relative;border-radius:24px;overflow:hidden;
height:520px;
}
.product-showcase-img{
position:absolute;inset:0;
background:url(‘https://images.unsplash.com/photo-1611365892117-00ac5ef43c90?w=900&q=85&auto=format&fit=crop’) center/cover no-repeat;
}
.product-showcase-grad{
position:absolute;inset:0;
background:linear-gradient(to top,rgba(11,18,32,1) 0%,rgba(11,18,32,.2) 70%);
}
.showcase-info{
position:absolute;bottom:0;left:0;right:0;padding:36px;
}
.showcase-tag{
display:inline-block;
background:rgba(245,166,35,.15);border:1px solid rgba(245,166,35,.3);
color:var(–gold);font-size:.72rem;letter-spacing:2px;text-transform:uppercase;
padding:4px 14px;border-radius:20px;margin-bottom:14px;
}
.showcase-name{font-family:‘Syne’,sans-serif;font-size:2rem;font-weight:800;margin-bottom:8px;}
.showcase-sub{color:rgba(255,255,255,.6);font-size:.9rem;margin-bottom:20px;}
.eff-bar{
background:rgba(255,255,255,.1);border-radius:4px;height:6px;
margin-bottom:6px;overflow:hidden;
}
.eff-fill{
height:100%;border-radius:4px;
background:linear-gradient(to right,var(–gold),var(–amber));
animation:fillBar 1.5s ease both;
}
@keyframes fillBar{from{width:0;}}
.eff-label{font-size:.78rem;color:rgba(255,255,255,.5);display:flex;justify-content:space-between;}

/* product list */
.product-list{display:flex;flex-direction:column;gap:16px;}
.prd{
display:flex;align-items:center;gap:20px;
background:rgba(255,255,255,.03);border:1px solid var(–border);
border-radius:16px;padding:20px 24px;
transition:border-color .3s,background .3s;cursor:pointer;
}
.prd:hover{border-color:rgba(245,166,35,.3);background:rgba(245,166,35,.04);}
.prd.active{border-color:var(–gold);background:rgba(245,166,35,.07);}
.prd-thumb{
width:80px;height:60px;border-radius:10px;
background-size:cover;background-position:center;flex-shrink:0;
border:1px solid var(–border);
}
.prd-info{flex:1;}
.prd-name{font-weight:700;font-size:.95rem;margin-bottom:4px;}
.prd-spec{color:rgba(255,255,255,.45);font-size:.8rem;}
.prd-price{font-family:‘Syne’,sans-serif;font-size:1.1rem;font-weight:800;color:var(–gold);white-space:nowrap;}
.prd-watt{
background:linear-gradient(135deg,var(–gold),var(–amber));
color:var(–ink);font-size:.7rem;font-weight:800;
padding:3px 10px;border-radius:10px;margin-top:4px;display:inline-block;
}

/* ─── GALLERY (Rajasthan Real Images) ─── */
#gallery{background:var(–ink);padding-bottom:0;}
.gallery-header{margin-bottom:48px;}
.gallery-masonry{
display:grid;
grid-template-columns:repeat(4,1fr);
grid-template-rows:auto;
gap:16px;
}
.gal-item{
border-radius:16px;overflow:hidden;position:relative;
background:#111;
transition:transform .4s;cursor:pointer;
}
.gal-item:hover{transform:scale(1.02);z-index:2;}
.gal-item img{
width:100%;height:100%;object-fit:cover;display:block;
transition:transform .6s ease;filter:brightness(.85);
}
.gal-item:hover img{transform:scale(1.06);filter:brightness(1);}
.gal-item.tall{grid-row:span 2;}
.gal-item.wide{grid-column:span 2;}
.gal-caption{
position:absolute;bottom:0;left:0;right:0;
background:linear-gradient(to top,rgba(11,18,32,.9),transparent);
padding:20px 16px 14px;
font-size:.8rem;color:rgba(255,255,255,.7);
transform:translateY(4px);opacity:0;transition:all .3s;
}
.gal-item:hover .gal-caption{transform:none;opacity:1;}

/* ─── RAJASTHAN ADVANTAGE ─── */
#advantage{
background:var(–slate);position:relative;overflow:hidden;
}
#advantage::before{
content:’’;position:absolute;inset:0;
background:url(‘https://images.unsplash.com/photo-1558618666-fcd25c85cd64?w=1600&q=60&auto=format&fit=crop’) center/cover no-repeat;
opacity:.07;
}
.adv-grid{
display:grid;grid-template-columns:1fr 1fr;gap:80px;
align-items:center;position:relative;z-index:1;
}
.adv-img-wrap{
border-radius:24px;overflow:hidden;height:500px;position:relative;
}
.adv-img-wrap img{width:100%;height:100%;object-fit:cover;}
.adv-img-wrap::after{
content:’’;position:absolute;inset:0;
background:linear-gradient(135deg,transparent 60%,rgba(11,18,32,.8));
}
/* sunlight hours badge */
.sun-badge{
position:absolute;bottom:32px;right:32px;z-index:2;
background:rgba(11,18,32,.85);backdrop-filter:blur(12px);
border:1px solid rgba(245,166,35,.3);border-radius:20px;
padding:20px 28px;text-align:center;
}
.sun-big{
font-family:‘Syne’,sans-serif;font-size:3rem;font-weight:800;
background:linear-gradient(135deg,var(–gold),var(–amber));
-webkit-background-clip:text;-webkit-text-fill-color:transparent;
line-height:1;
}
.sun-lbl{font-size:.72rem;color:rgba(255,255,255,.5);letter-spacing:1.5px;text-transform:uppercase;margin-top:4px;}

.adv-points{display:flex;flex-direction:column;gap:32px;}
.adv-pt{display:flex;gap:20px;align-items:flex-start;}
.adv-icon{
width:56px;height:56px;border-radius:16px;flex-shrink:0;
background:linear-gradient(135deg,rgba(245,166,35,.18),rgba(232,98,42,.12));
border:1px solid rgba(245,166,35,.2);
display:flex;align-items:center;justify-content:center;font-size:1.7rem;
}
.adv-txt h3{font-family:‘Syne’,sans-serif;font-size:1.1rem;margin-bottom:6px;}
.adv-txt p{color:rgba(255,255,255,.5);font-size:.9rem;line-height:1.7;}

/* ─── PROCESS ─── */
#process{background:var(–ink);}
.process-track{
display:grid;grid-template-columns:repeat(5,1fr);
gap:0;margin-top:64px;position:relative;
}
.process-track::before{
content:’’;position:absolute;top:40px;left:10%;right:10%;height:1px;
background:linear-gradient(to right,transparent,var(–gold),var(–amber),transparent);
}
.proc{text-align:center;padding:0 16px;position:relative;}
.proc-circle{
width:80px;height:80px;border-radius:50%;margin:0 auto 24px;
background:linear-gradient(135deg,rgba(245,166,35,.15),rgba(232,98,42,.1));
border:1px solid rgba(245,166,35,.3);
display:flex;align-items:center;justify-content:center;
font-size:1.8rem;position:relative;z-index:1;
transition:background .3s,box-shadow .3s;
}
.proc:hover .proc-circle{
background:linear-gradient(135deg,var(–gold),var(–amber));
box-shadow:0 0 30px rgba(245,166,35,.4);
font-size:1.6rem;
}
.proc-n{
position:absolute;top:-8px;right:-8px;
width:26px;height:26px;border-radius:50%;
background:linear-gradient(135deg,var(–gold),var(–amber));
color:var(–ink);font-family:‘Syne’,sans-serif;font-weight:800;
font-size:.72rem;display:flex;align-items:center;justify-content:center;
}
.proc-title{font-family:‘Syne’,sans-serif;font-size:.95rem;font-weight:700;margin-bottom:8px;}
.proc-desc{color:rgba(255,255,255,.45);font-size:.82rem;line-height:1.6;}

/* ─── TESTIMONIALS ─── */
#testimonials{background:var(–navy);}
.test-grid{
display:grid;grid-template-columns:repeat(3,1fr);gap:24px;
margin-top:56px;
}
.test-card{
border-radius:20px;padding:32px;
background:rgba(255,255,255,.025);
border:1px solid var(–border);
position:relative;overflow:hidden;
transition:border-color .3s,transform .3s;
}
.test-card:hover{border-color:rgba(245,166,35,.25);transform:translateY(-4px);}
.test-card::before{
content:‘❝’;position:absolute;top:16px;right:20px;
font-size:4rem;color:rgba(245,166,35,.08);font-family:serif;
line-height:1;
}
.test-stars{color:var(–gold);font-size:.85rem;margin-bottom:16px;}
.test-text{
color:rgba(255,255,255,.7);line-height:1.75;font-size:.92rem;
margin-bottom:24px;
}
.test-author{display:flex;align-items:center;gap:14px;}
.avi{
width:46px;height:46px;border-radius:50%;overflow:hidden;
border:2px solid rgba(245,166,35,.3);flex-shrink:0;
}
.avi img{width:100%;height:100%;object-fit:cover;}
.avi-initials{
width:46px;height:46px;border-radius:50%;flex-shrink:0;
background:linear-gradient(135deg,var(–gold),var(–amber));
color:var(–ink);font-family:‘Syne’,sans-serif;font-weight:800;
display:flex;align-items:center;justify-content:center;font-size:1rem;
}
.aut-name{font-weight:600;font-size:.92rem;}
.aut-loc{color:rgba(255,255,255,.4);font-size:.78rem;margin-top:2px;}

/* ─── CTA SECTION ─── */
#cta{
position:relative;overflow:hidden;padding:0;
min-height:560px;display:flex;align-items:stretch;
}
.cta-bg{
position:absolute;inset:0;
background:url(‘https://images.unsplash.com/photo-1466611653911-95081537e5b7?w=1600&q=80&auto=format&fit=crop’) center/cover no-repeat;
filter:brightness(.35) saturate(1.2);
}
.cta-inner{
position:relative;z-index:2;
display:grid;grid-template-columns:1fr 1fr;
width:100%;
}
.cta-left{
padding:80px 64px;
display:flex;flex-direction:column;justify-content:center;
}
.cta-title{
font-family:‘Syne’,sans-serif;
font-size:clamp(2rem,3.5vw,3rem);font-weight:800;
line-height:1.15;margin-bottom:16px;
}
.cta-title span{
background:linear-gradient(135deg,var(–gold),var(–amber));
-webkit-background-clip:text;-webkit-text-fill-color:transparent;
}
.cta-sub{color:rgba(255,255,255,.6);font-size:1rem;line-height:1.75;margin-bottom:32px;}
.offer-box{
background:rgba(245,166,35,.1);border:1px solid rgba(245,166,35,.3);
border-radius:16px;padding:20px 24px;margin-bottom:36px;
display:flex;gap:16px;align-items:center;
}
.offer-icon{font-size:2rem;}
.offer-txt strong{color:var(–gold);display:block;font-size:1rem;margin-bottom:4px;}
.offer-txt span{color:rgba(255,255,255,.55);font-size:.85rem;}

.cta-right{
padding:80px 64px;
display:flex;flex-direction:column;justify-content:center;
background:rgba(11,18,32,.6);backdrop-filter:blur(20px);
}
.form-title{font-family:‘Syne’,sans-serif;font-size:1.5rem;font-weight:700;margin-bottom:24px;}
.form-group{margin-bottom:16px;}
.form-group label{display:block;font-size:.8rem;color:rgba(255,255,255,.5);letter-spacing:1px;text-transform:uppercase;margin-bottom:8px;}
.form-input{
width:100%;padding:14px 18px;border-radius:12px;
background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.12);
color:#fff;font-family:‘DM Sans’,sans-serif;font-size:.95rem;
outline:none;transition:border-color .25s;
}
.form-input:focus{border-color:var(–gold);}
.form-input::placeholder{color:rgba(255,255,255,.3);}
select.form-input option{background:#1A2840;}
.form-submit{
width:100%;padding:16px;border-radius:12px;border:none;cursor:pointer;
background:linear-gradient(135deg,var(–gold),var(–amber));
color:var(–ink);font-family:‘Syne’,sans-serif;font-size:1rem;font-weight:800;
letter-spacing:.5px;transition:transform .2s,box-shadow .2s;
margin-top:8px;
}
.form-submit:hover{transform:translateY(-2px);box-shadow:0 10px 32px rgba(245,166,35,.45);}
.trust-row{
display:flex;gap:16px;margin-top:16px;flex-wrap:wrap;
}
.trust-item{
display:flex;align-items:center;gap:6px;
font-size:.75rem;color:rgba(255,255,255,.4);
}
.trust-item::before{content:‘✓’;color:var(–gold);font-weight:700;}

/* ─── FOOTER ─── */
footer{
background:#080E1A;
border-top:1px solid var(–border);
padding:64px;
}
.footer-top{
display:grid;grid-template-columns:2.5fr 1fr 1fr 1fr;
gap:56px;margin-bottom:56px;
}
.f-brand{}
.f-logo-row{display:flex;align-items:center;gap:12px;margin-bottom:18px;}
.f-logo-icon{
width:40px;height:40px;border-radius:10px;
background:linear-gradient(135deg,var(–gold),var(–amber));
display:flex;align-items:center;justify-content:center;font-size:1.3rem;
}
.f-logo-name{font-family:‘Syne’,sans-serif;font-size:1.1rem;font-weight:800;}
.f-logo-name small{display:block;font-size:.6rem;color:var(–gold);letter-spacing:2px;}
.f-desc{color:rgba(255,255,255,.4);font-size:.88rem;line-height:1.7;margin-bottom:24px;}
.f-cert{display:flex;gap:10px;flex-wrap:wrap;}
.cert-pill{
background:rgba(255,255,255,.05);border:1px solid rgba(255,255,255,.1);
padding:4px 12px;border-radius:20px;font-size:.72rem;color:rgba(255,255,255,.5);
}
.f-col h4{font-family:‘Syne’,sans-serif;font-size:.85rem;font-weight:700;color:var(–gold);letter-spacing:1.5px;text-transform:uppercase;margin-bottom:20px;}
.f-col ul{list-style:none;}
.f-col ul li{margin-bottom:10px;}
.f-col ul li a{color:rgba(255,255,255,.4);text-decoration:none;font-size:.88rem;transition:color .2s;}
.f-col ul li a:hover{color:#fff;}
.footer-bottom{
padding-top:32px;border-top:1px solid var(–border);
display:flex;justify-content:space-between;align-items:center;
flex-wrap:wrap;gap:12px;
}
.footer-bottom span{color:rgba(255,255,255,.28);font-size:.8rem;}
.f-socials{display:flex;gap:12px;}
.f-social{
width:36px;height:36px;border-radius:50%;
background:rgba(255,255,255,.06);border:1px solid var(–border);
display:flex;align-items:center;justify-content:center;
font-size:1rem;text-decoration:none;
transition:background .2s,border-color .2s;
}
.f-social:hover{background:rgba(245,166,35,.15);border-color:rgba(245,166,35,.4);}

/* ─── SCROLL REVEAL ─── */
.reveal{opacity:0;transform:translateY(28px);transition:opacity .7s,transform .7s;}
.reveal.up{opacity:1;transform:none;}

/* ─── RESPONSIVE ─── */
@media(max-width:1024px){
#hero{grid-template-columns:1fr;}
.hero-right{display:none;}
nav ul{display:none;}
section{padding:80px 28px;}
.services-grid,.products-layout,.adv-grid,.cta-inner,.test-grid,.footer-top{grid-template-columns:1fr;}
.process-track{grid-template-columns:1fr 1fr;gap:32px;}
.process-track::before{display:none;}
#about{grid-template-columns:1fr 1fr;}
.gallery-masonry{grid-template-columns:1fr 1fr;}
.gal-item.wide{grid-column:span 1;}
nav{padding:16px 24px;}
.hero-left{padding:130px 28px 70px;}
}
</style>

</head>
<body>

<!-- CURSOR -->

<div class="cursor" id="cursor"></div>
<div class="cursor-ring" id="cursorRing"></div>

<!-- NAV -->

<nav id="navbar">
  <div class="logo-wrap">
    <div class="logo-icon">⚡</div>
    <div class="logo-text">
      The Bhadu Solar Energy
      <small>Rajasthan, India</small>
    </div>
  </div>
  <ul>
    <li><a href="#services">Services</a></li>
    <li><a href="#products">Products</a></li>
    <li><a href="#gallery">Projects</a></li>
    <li><a href="#advantage">Why Us</a></li>
    <li><a href="#cta" class="nav-btn">Free Quote</a></li>
  </ul>
</nav>

<!-- ══════════ HERO ══════════ -->

<section id="hero">
  <!-- LEFT -->
  <div class="hero-left">
    <div class="hero-eyebrow">🌅 Rajasthan's Trusted Solar Partner Since 2012</div>
    <h1>
      Harness<br>
      <span class="line-gold">Rajasthan's</span><br>
      Infinite Sun
    </h1>
    <p class="hero-desc">
      The Bhadu Solar Energy brings cutting-edge solar technology to every corner of Rajasthan — from desert farms in Barmer to rooftops in Jaipur. Zero bills. Zero compromise.
    </p>
    <div class="hero-actions">
      <a href="#cta" class="btn-glow">Get Free Survey →</a>
      <a href="#products" class="btn-ghost">Our Products</a>
    </div>
    <div class="hero-stats">
      <div class="hs"><div class="hs-num" data-target="9200">0</div><div class="hs-lbl">Installations Done</div></div>
      <div class="hs"><div class="hs-num" data-target="25" data-suffix=" MW">0</div><div class="hs-lbl">Capacity Installed</div></div>
      <div class="hs"><div class="hs-num" data-target="325" data-suffix="+">0</div><div class="hs-lbl">Sunny Days / Year</div></div>
      <div class="hs"><div class="hs-num" data-target="15" data-suffix=" Yr">0</div><div class="hs-lbl">Warranty</div></div>
    </div>
  </div>

  <!-- RIGHT (real image) -->

  <div class="hero-right">
    <div class="hero-img-main"></div>
    <div class="hero-img-overlay"></div>

```
<div class="live-badge">
  <span class="live-dot"></span> Live Generation: 18.4 kW
</div>

<!-- floating stat cards -->
<div class="float-card">
  <div class="fc-label">Today's Output</div>
  <div class="fc-value">142 kWh</div>
  <div class="fc-sub">Sitapura Plant, Jaipur</div>
</div>
<div class="float-card">
  <div class="fc-label">CO₂ Saved</div>
  <div class="fc-value">4,820 T</div>
  <div class="fc-sub">This year across Rajasthan</div>
</div>
<div class="float-card">
  <div class="fc-label">Savings Generated</div>
  <div class="fc-value">₹280 Cr</div>
  <div class="fc-sub">For our customers</div>
</div>
```

  </div>

  <div class="scroll-hint">
    <div class="scroll-arrow"></div>
    Scroll
  </div>
</section>

<!-- ══════════ ABOUT STRIP ══════════ -->

<div id="about">
  <div class="about-item reveal">
    <div class="ai-num">12+</div>
    <div class="ai-title">Years of Experience</div>
    <div class="ai-desc">Serving Rajasthan since 2012 with a team of 200+ certified solar engineers.</div>
  </div>
  <div class="about-item reveal">
    <div class="ai-num">50</div>
    <div class="ai-title">Districts Covered</div>
    <div class="ai-desc">Service centers in Jaipur, Jodhpur, Udaipur, Kota, Bikaner, Barmer & more.</div>
  </div>
  <div class="about-item reveal">
    <div class="ai-num">MNRE</div>
    <div class="ai-title">Approved Partner</div>
    <div class="ai-desc">Empanelled with RRECL, MNRE and all 3 DISCOMs — JVVNL, AVVNL, JDVVNL.</div>
  </div>
  <div class="about-item reveal">
    <div class="ai-num">4.9★</div>
    <div class="ai-title">Customer Rating</div>
    <div class="ai-desc">Based on 3,400+ verified reviews from across Rajasthan.</div>
  </div>
</div>

<!-- ══════════ SERVICES ══════════ -->

<section id="services">
  <div class="tag">What We Do</div>
  <h2 class="sec-title">Complete Solar Solutions<br>for Every Rajasthani</h2>
  <p class="sec-sub">Whether you're a farmer, a home owner or a factory owner — The Bhadu Solar Energy has a solution built for you.</p>

  <div class="services-grid">
    <div class="svc-card reveal">
      <div class="svc-img" style="background-image:url('https://images.unsplash.com/photo-1558449028-b53a39d100fc?w=800&q=80&auto=format&fit=crop')"></div>
      <div class="svc-overlay"></div>
      <div class="svc-badge">Most Popular</div>
      <div class="svc-content">
        <span class="svc-icon">🏠</span>
        <div class="svc-name">Residential Rooftop</div>
        <div class="svc-desc">1kW–20kW systems for homes. Net metering support. Up to ₹78,000 RRECL subsidy. Payback in 3–4 years.</div>
      </div>
    </div>
    <div class="svc-card reveal">
      <div class="svc-img" style="background-image:url('https://images.unsplash.com/photo-1521618755572-156ae0cdd74d?w=800&q=80&auto=format&fit=crop')"></div>
      <div class="svc-overlay"></div>
      <div class="svc-content">
        <span class="svc-icon">🏭</span>
        <div class="svc-name">Industrial & Commercial</div>
        <div class="svc-desc">50kW–10MW EPC turnkey projects. Complete design, supply, install and O&M for factories, malls and hospitals.</div>
      </div>
    </div>
    <div class="svc-card reveal">
      <div class="svc-img" style="background-image:url('https://images.unsplash.com/photo-1497440001374-f26997328c1b?w=800&q=80&auto=format&fit=crop')"></div>
      <div class="svc-overlay"></div>
      <div class="svc-badge">PM-KUSUM</div>
      <div class="svc-content">
        <span class="svc-icon">🌾</span>
        <div class="svc-name">Agri Solar Pumps</div>
        <div class="svc-desc">Solar pumping systems under PM-KUSUM with 60% government subsidy. Zero diesel cost for irrigation.</div>
      </div>
    </div>
  </div>
</section>

<!-- ══════════ PRODUCTS ══════════ -->

<section id="products">
  <div class="tag">Our Products</div>
  <h2 class="sec-title">Panels Engineered<br>for Desert Conditions</h2>
  <p class="sec-sub">Tested up to 75°C ambient — our panels perform at peak efficiency even when Rajasthan temperatures cross 50°C.</p>

  <div class="products-layout">
    <!-- showcase image -->
    <div class="product-showcase reveal">
      <div class="product-showcase-img" id="showcaseImg"></div>
      <div class="product-showcase-grad"></div>
      <div class="showcase-info" id="showcaseInfo">
        <div class="showcase-tag">Best Seller</div>
        <div class="showcase-name">Bhadu Max Pro 545W</div>
        <div class="showcase-sub">Monocrystalline PERC Half-Cut | 21.5% Efficiency | BIS Certified | IP68</div>
        <div class="eff-bar"><div class="eff-fill" style="width:86%"></div></div>
        <div class="eff-label"><span>Efficiency</span><span>21.5%</span></div>
      </div>
    </div>

```
<!-- product list -->
<div class="product-list">
  <div class="prd active reveal" onclick="selectProduct(this,0)">
    <div class="prd-thumb" style="background-image:url('https://images.unsplash.com/photo-1609947017136-9daf32a5ab32?w=200&q=80&auto=format&fit=crop')"></div>
    <div class="prd-info">
      <div class="prd-name">Bhadu Max Pro 545W</div>
      <div class="prd-spec">Mono PERC Half-Cut | 25-yr warranty | BIS Certified</div>
      <span class="prd-watt">545W</span>
    </div>
    <div class="prd-price">₹14,500</div>
  </div>
  <div class="prd reveal" onclick="selectProduct(this,1)">
    <div class="prd-thumb" style="background-image:url('https://images.unsplash.com/photo-1624397640148-949b1732bb0a?w=200&q=80&auto=format&fit=crop')"></div>
    <div class="prd-info">
      <div class="prd-name">Bhadu Home 440W</div>
      <div class="prd-spec">Polycrystalline | Best value residential | IEC Certified</div>
      <span class="prd-watt">440W</span>
    </div>
    <div class="prd-price">₹10,200</div>
  </div>
  <div class="prd reveal" onclick="selectProduct(this,2)">
    <div class="prd-thumb" style="background-image:url('https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?w=200&q=80&auto=format&fit=crop')"></div>
    <div class="prd-info">
      <div class="prd-name">Bhadu Agri Bifacial 600W</div>
      <div class="prd-spec">Bifacial Mono | Sandstorm rated | 30-yr warranty</div>
      <span class="prd-watt">600W</span>
    </div>
    <div class="prd-price">₹18,000</div>
  </div>
  <div class="prd reveal" onclick="selectProduct(this,3)">
    <div class="prd-thumb" style="background-image:url('https://images.unsplash.com/photo-1473341304170-971dccb5ac1e?w=200&q=80&auto=format&fit=crop')"></div>
    <div class="prd-info">
      <div class="prd-name">Bhadu Lithium BESS 10kWh</div>
      <div class="prd-spec">LiFePO4 Battery Storage | 6000+ cycles | Smart BMS</div>
      <span class="prd-watt">Storage</span>
    </div>
    <div class="prd-price">₹2,20,000</div>
  </div>
</div>
```

  </div>
</section>

<!-- ══════════ GALLERY ══════════ -->

<section id="gallery">
  <div class="gallery-header">
    <div class="tag">Our Work</div>
    <h2 class="sec-title">Real Projects Across<br>Rajasthan</h2>
  </div>
  <div class="gallery-masonry">
    <div class="gal-item tall reveal">
      <img src="https://images.unsplash.com/photo-1509391366360-2e959784a276?w=600&q=80&auto=format&fit=crop" alt="Solar farm Rajasthan" loading="lazy">
      <div class="gal-caption">500kW Ground Mount — Jaisalmer</div>
    </div>
    <div class="gal-item reveal">
      <img src="https://images.unsplash.com/photo-1611365892117-00ac5ef43c90?w=600&q=80&auto=format&fit=crop" alt="Solar panels" loading="lazy">
      <div class="gal-caption">Rooftop 20kW — Jodhpur</div>
    </div>
    <div class="gal-item reveal">
      <img src="https://images.unsplash.com/photo-1466611653911-95081537e5b7?w=600&q=80&auto=format&fit=crop" alt="Solar field sunset" loading="lazy">
      <div class="gal-caption">2MW Agri Solar — Barmer</div>
    </div>
    <div class="gal-item tall reveal">
      <img src="https://images.unsplash.com/photo-1558618666-fcd25c85cd64?w=600&q=80&auto=format&fit=crop" alt="Industrial solar" loading="lazy">
      <div class="gal-caption">150kW Industrial — Bhilwara</div>
    </div>
    <div class="gal-item wide reveal">
      <img src="https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?w=900&q=80&auto=format&fit=crop" alt="Solar installation" loading="lazy">
      <div class="gal-caption">PM-KUSUM Solar Pump — Nagaur</div>
    </div>
    <div class="gal-item reveal">
      <img src="https://images.unsplash.com/photo-1497440001374-f26997328c1b?w=600&q=80&auto=format&fit=crop" alt="Solar panels aerial" loading="lazy">
      <div class="gal-caption">Hospital 80kW — Udaipur</div>
    </div>
    <div class="gal-item reveal">
      <img src="https://images.unsplash.com/photo-1624397640148-949b1732bb0a?w=600&q=80&auto=format&fit=crop" alt="Close up panels" loading="lazy">
      <div class="gal-caption">Residential 10kW — Jaipur</div>
    </div>
  </div>
</section>

<!-- ══════════ ADVANTAGE ══════════ -->

<section id="advantage">
  <div class="adv-grid">
    <div class="adv-img-wrap reveal">
      <img src="https://images.unsplash.com/photo-1521618755572-156ae0cdd74d?w=900&q=80&auto=format&fit=crop" alt="Solar farm Rajasthan" loading="lazy">
      <div class="sun-badge">
        <div class="sun-big">6.2</div>
        <div class="sun-lbl">kWh/m²/day<br>Peak Irradiance</div>
      </div>
    </div>
    <div>
      <div class="tag">Why Rajasthan + Why Bhadu</div>
      <h2 class="sec-title">India's Solar Capital<br>Needs India's Best</h2>
      <div class="adv-points">
        <div class="adv-pt reveal">
          <div class="adv-icon">☀️</div>
          <div class="adv-txt">
            <h3>Highest Solar Irradiance in India</h3>
            <p>Rajasthan receives 6.2 kWh/m²/day — 20% more than the national average — meaning every panel generates more power here than anywhere else in India.</p>
          </div>
        </div>
        <div class="adv-pt reveal">
          <div class="adv-icon">🏛️</div>
          <div class="adv-txt">
            <h3>₹78,000 RRECL Subsidy — We Handle It All</h3>
            <p>As RRECL-empanelled installers, we file every subsidy application, DISCOM approval and net-meter form on your behalf. Zero paperwork for you.</p>
          </div>
        </div>
        <div class="adv-pt reveal">
          <div class="adv-icon">📱</div>
          <div class="adv-txt">
            <h3>Real-Time App Monitoring</h3>
            <p>Track live generation, savings and CO₂ avoided from the Bhadu Solar app. Get alerts if performance dips below threshold.</p>
          </div>
        </div>
        <div class="adv-pt reveal">
          <div class="adv-icon">🛡️</div>
          <div class="adv-txt">
            <h3>25-Year Performance Guarantee</h3>
            <p>We guarantee ≥80% power output at 25 years. Backed by insurance and backed by Bhadu — the name Rajasthan trusts.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ══════════ PROCESS ══════════ -->

<section id="process">
  <div style="text-align:center;margin-bottom:0">
    <div class="tag">How It Works</div>
    <h2 class="sec-title">Solar in 5 Simple Steps</h2>
    <p class="sec-sub" style="margin:0 auto">From first call to first unit generated — The Bhadu Solar manages everything.</p>
  </div>
  <div class="process-track">
    <div class="proc reveal">
      <div class="proc-circle">📞<div class="proc-n">1</div></div>
      <div class="proc-title">Free Consultation</div>
      <div class="proc-desc">Call or WhatsApp us. Our expert analyzes your electricity bill and suggests system size.</div>
    </div>
    <div class="proc reveal">
      <div class="proc-circle">🔍<div class="proc-n">2</div></div>
      <div class="proc-title">Site Survey</div>
      <div class="proc-desc">Our engineer visits your site and designs the optimal solar layout for maximum output.</div>
    </div>
    <div class="proc reveal">
      <div class="proc-circle">📋<div class="proc-n">3</div></div>
      <div class="proc-title">Subsidy Filing</div>
      <div class="proc-desc">We submit all RRECL, DISCOM and government subsidy paperwork. Zero hassle for you.</div>
    </div>
    <div class="proc reveal">
      <div class="proc-circle">🔧<div class="proc-n">4</div></div>
      <div class="proc-title">Installation</div>
      <div class="proc-desc">Certified engineers install the system in 1–3 days with clean, professional workmanship.</div>
    </div>
    <div class="proc reveal">
      <div class="proc-circle">⚡<div class="proc-n">5</div></div>
      <div class="proc-title">Go Solar!</div>
      <div class="proc-desc">Net meter activated. Open your Bhadu app and watch your electricity bills disappear.</div>
    </div>
  </div>
</section>

<!-- ══════════ TESTIMONIALS ══════════ -->

<section id="testimonials">
  <div class="tag">Customer Stories</div>
  <h2 class="sec-title">4.9★ Rated Across<br>Rajasthan</h2>
  <div class="test-grid">
    <div class="test-card reveal">
      <div class="test-stars">★★★★★</div>
      <p class="test-text">"Bhadu Solar ne hamare 5kW ka system lagaya — ab bijli ka bill ₹8,000 se ₹0 ho gaya. Pura paise 3.5 saal mein vasool. Team bahut professional thi."</p>
      <div class="test-author">
        <div class="avi-initials">RK</div>
        <div>
          <div class="aut-name">Ramesh Kumar Sharma</div>
          <div class="aut-loc">📍 Mansarovar, Jaipur</div>
        </div>
      </div>
    </div>
    <div class="test-card reveal">
      <div class="test-stars">★★★★★</div>
      <p class="test-text">"PM-KUSUM scheme ke through solar pump lagwaya. 60% subsidy mili, Bhadu Solar ne sab kuch handle kiya. Khet mein ab free paani. Barmer ke sabhi kisaanon ke liye recommend karunga."</p>
      <div class="test-author">
        <div class="avi-initials">BS</div>
        <div>
          <div class="aut-name">Bhawar Singh Rajput</div>
          <div class="aut-loc">📍 Barmer, Rajasthan</div>
        </div>
      </div>
    </div>
    <div class="test-card reveal">
      <div class="test-stars">★★★★★</div>
      <p class="test-text">"Our 200kW factory installation in Bhilwara was completed on schedule. ROI achieved in 3.5 years. The monitoring app is brilliant — I can see real-time data from anywhere."</p>
      <div class="test-author">
        <div class="avi-initials">PJ</div>
        <div>
          <div class="aut-name">Priya Jain</div>
          <div class="aut-loc">📍 Bhilwara Industrial Area</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ══════════ CTA ══════════ -->

<section id="cta">
  <div class="cta-bg"></div>
  <div class="cta-inner">
    <div class="cta-left">
      <div class="tag">Limited Offer — March 2025</div>
      <h2 class="cta-title">Get <span>₹5,000 Off</span><br>+ Free Installation<br>This Month</h2>
      <p class="cta-sub">Join 9,200+ happy customers across Rajasthan. Our solar advisors respond within 30 minutes.</p>
      <div class="offer-box">
        <div class="offer-icon">🎁</div>
        <div class="offer-txt">
          <strong>Special March Offer</strong>
          <span>₹5,000 discount + Free site survey + Free net meter application worth ₹3,500</span>
        </div>
      </div>
      <div style="display:flex;gap:28px;flex-wrap:wrap">
        <div><div style="font-family:'Syne',sans-serif;font-size:1.8rem;font-weight:800;color:var(--gold)">₹0</div><div style="font-size:.78rem;color:rgba(255,255,255,.45);text-transform:uppercase;letter-spacing:1px">Site Survey Cost</div></div>
        <div><div style="font-family:'Syne',sans-serif;font-size:1.8rem;font-weight:800;color:var(--gold)">30 Min</div><div style="font-size:.78rem;color:rgba(255,255,255,.45);text-transform:uppercase;letter-spacing:1px">Response Time</div></div>
        <div><div style="font-family:'Syne',sans-serif;font-size:1.8rem;font-weight:800;color:var(--gold)">24/7</div><div style="font-size:.78rem;color:rgba(255,255,255,.45);text-transform:uppercase;letter-spacing:1px">Support</div></div>
      </div>
    </div>
    <div class="cta-right">
      <div class="form-title">Get Your Free Quote</div>
      <div class="form-group">
        <label>Full Name</label>
        <input class="form-input" type="text" placeholder="Ramesh Kumar Sharma">
      </div>
      <div class="form-group">
        <label>Mobile Number</label>
        <input class="form-input" type="tel" placeholder="+91 98765 43210">
      </div>
      <div class="form-group">
        <label>City / District</label>
        <select class="form-input">
          <option value="">Select your city</option>
          <option>Jaipur</option><option>Jodhpur</option><option>Udaipur</option>
          <option>Kota</option><option>Bikaner</option><option>Jaisalmer</option>
          <option>Barmer</option><option>Ajmer</option><option>Alwar</option>
          <option>Other Rajasthan District</option>
        </select>
      </div>
      <div class="form-group">
        <label>I Need Solar For</label>
        <select class="form-input">
          <option>My Home (Residential)</option>
          <option>My Farm (Agri / PM-KUSUM)</option>
          <option>My Factory / Shop (Commercial)</option>
          <option>Industrial / Large Project</option>
        </select>
      </div>
      <button class="form-submit" onclick="alert('धन्यवाद! The Bhadu Solar की टीम 30 मिनट में संपर्क करेगी। 🌞')">
        ⚡ Get Free Quote Now
      </button>
      <div class="trust-row">
        <div class="trust-item">RRECL Empanelled</div>
        <div class="trust-item">MNRE Approved</div>
        <div class="trust-item">BIS Certified</div>
        <div class="trust-item">No Spam</div>
      </div>
    </div>
  </div>
</section>

<!-- ══════════ FOOTER ══════════ -->

<footer>
  <div class="footer-top">
    <div class="f-brand">
      <div class="f-logo-row">
        <div class="f-logo-icon">⚡</div>
        <div class="f-logo-name">The Bhadu Solar Energy<small>Rajasthan, India</small></div>
      </div>
      <p class="f-desc">Rajasthan's most trusted solar energy company. Delivering clean, affordable solar power to homes, farms and industries across all 50 districts since 2012.</p>
      <div class="f-cert">
        <span class="cert-pill">🇮🇳 Made in India</span>
        <span class="cert-pill">RRECL Empanelled</span>
        <span class="cert-pill">MNRE Approved</span>
        <span class="cert-pill">BIS Certified</span>
        <span class="cert-pill">ISO 9001:2015</span>
      </div>
    </div>
    <div class="f-col">
      <h4>Services</h4>
      <ul>
        <li><a href="#">Residential Solar</a></li>
        <li><a href="#">Commercial Solar</a></li>
        <li><a href="#">Industrial EPC</a></li>
        <li><a href="#">Agri PM-KUSUM</a></li>
        <li><a href="#">Battery Storage</a></li>
        <li><a href="#">O&M Services</a></li>
      </ul>
    </div>
    <div class="f-col">
      <h4>Cities</h4>
      <ul>
        <li><a href="#">Jaipur</a></li>
        <li><a href="#">Jodhpur</a></li>
        <li><a href="#">Udaipur</a></li>
        <li><a href="#">Kota</a></li>
        <li><a href="#">Bikaner</a></li>
        <li><a href="#">Jaisalmer & Barmer</a></li>
      </ul>
    </div>
    <div class="f-col">
      <h4>Contact</h4>
      <ul>
        <li><a href="tel:18001234567">📞 1800-123-BHADU (Free)</a></li>
        <li><a href="#">💬 WhatsApp: +91 98XXX XXXXX</a></li>
        <li><a href="#">✉️ info@bhadusolar.in</a></li>
        <li><a href="#">📍 Plot 42, RIICO, Sitapura<br>Jaipur — 302022</a></li>
      </ul>
    </div>
  </div>
  <div class="footer-bottom">
    <span>© 2025 The Bhadu Solar Energy Pvt. Ltd. | CIN: U40100RJ2012PTC XXXXXX | All rights reserved.</span>
    <div class="f-socials">
      <a class="f-social" href="#">📘</a>
      <a class="f-social" href="#">📷</a>
      <a class="f-social" href="#">▶️</a>
      <a class="f-social" href="#">💬</a>
    </div>
  </div>
</footer>

<script>
// ── Custom Cursor ──
const cur = document.getElementById('cursor');
const ring = document.getElementById('cursorRing');
let mx=0,my=0,rx=0,ry=0;
document.addEventListener('mousemove',e=>{
  mx=e.clientX; my=e.clientY;
  cur.style.left=mx+'px'; cur.style.top=my+'px';
});
(function animRing(){
  rx+=(mx-rx)*.12; ry+=(my-ry)*.12;
  ring.style.left=rx+'px'; ring.style.top=ry+'px';
  requestAnimationFrame(animRing);
})();
document.querySelectorAll('a,button,.prd,.svc-card,.gal-item').forEach(el=>{
  el.addEventListener('mouseenter',()=>{ring.style.transform='translate(-50%,-50%) scale(1.8)';ring.style.borderColor='rgba(245,166,35,0.8)';});
  el.addEventListener('mouseleave',()=>{ring.style.transform='translate(-50%,-50%) scale(1)';ring.style.borderColor='rgba(245,166,35,0.5)';});
});

// ── Navbar scroll ──
window.addEventListener('scroll',()=>{
  document.getElementById('navbar').classList.toggle('scrolled',window.scrollY>60);
});

// ── Scroll reveal ──
const revealObs = new IntersectionObserver(entries=>{
  entries.forEach(e=>{ if(e.isIntersecting) e.target.classList.add('up'); });
},{threshold:0.12});
document.querySelectorAll('.reveal').forEach(el=>revealObs.observe(el));

// ── Counter animation ──
const countObs = new IntersectionObserver(entries=>{
  entries.forEach(e=>{
    if(!e.isIntersecting) return;
    const el = e.target;
    const target = +el.dataset.target;
    const suffix = el.dataset.suffix || '';
    let curr = 0;
    const step = target / 80;
    const iv = setInterval(()=>{
      curr = Math.min(curr + step, target);
      el.textContent = (Number.isInteger(target) ? Math.floor(curr) : curr.toFixed(1)) + suffix;
      if(curr >= target) clearInterval(iv);
    }, 20);
    countObs.unobserve(el);
  });
},{threshold:0.5});
document.querySelectorAll('[data-target]').forEach(el=>countObs.observe(el));

// ── Product selector ──
const products = [
  {
    name:'Bhadu Max Pro 545W',
    sub:'Monocrystalline PERC Half-Cut | 21.5% Efficiency | BIS Certified | IP68 | 25-yr warranty',
    eff:86,
    img:'https://images.unsplash.com/photo-1609947017136-9daf32a5ab32?w=900&q=85&auto=format&fit=crop',
    badge:'Best Seller'
  },
  {
    name:'Bhadu Home 440W',
    sub:'Polycrystalline | Best value for residential | IEC Certified | 20-yr warranty',
    eff:72,
    img:'https://images.unsplash.com/photo-1624397640148-949b1732bb0a?w=900&q=85&auto=format&fit=crop',
    badge:'Best Value'
  },
  {
    name:'Bhadu Agri Bifacial 600W',
    sub:'Bifacial Monocrystalline | Sandstorm rated | 30-yr warranty | For agri & utility',
    eff:93,
    img:'https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?w=900&q=85&auto=format&fit=crop',
    badge:'Top Efficiency'
  },
  {
    name:'Bhadu Lithium BESS 10kWh',
    sub:'LiFePO4 Battery | 6000+ cycles | Smart BMS | 24/7 backup power | 10-yr warranty',
    eff:98,
    img:'https://images.unsplash.com/photo-1473341304170-971dccb5ac1e?w=900&q=85&auto=format&fit=crop',
    badge:'New Product'
  }
];

function selectProduct(el, idx){
  document.querySelectorAll('.prd').forEach(p=>p.classList.remove('active'));
  el.classList.add('active');
  const p = products[idx];
  document.getElementById('showcaseImg').style.backgroundImage = `url('${p.img}')`;
  document.getElementById('showcaseInfo').innerHTML = `
    <div class="showcase-tag">${p.badge}</div>
    <div class="showcase-name">${p.name}</div>
    <div class="showcase-sub">${p.sub}</div>
    <div class="eff-bar"><div class="eff-fill" style="width:${p.eff}%;animation:fillBar 1s ease both"></div></div>
    <div class="eff-label"><span>Efficiency Score</span><span>${p.eff}%</span></div>
  `;
}
// init showcase
selectProduct(document.querySelector('.prd.active'), 0);
</script>

</body>
</html>
