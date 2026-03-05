:root{
  --bg:#0b0c10;
  --card:#121420;
  --text:#e8e8ea;
  --muted:#b7b7c0;
  --line:#25283a;
  --accent:#7c5cff;
}

*{box-sizing:border-box}
html,body{margin:0;padding:0;font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial; background:var(--bg); color:var(--text);}
a{color:inherit}
.container{width:min(1100px, 92vw); margin:0 auto;}
.section{padding:42px 0}
h1,h2,h3{margin:0 0 12px 0; letter-spacing:-0.02em}
h2{font-size:22px}
.cn{color:var(--muted); font-size:0.9em; margin-left:6px}
.note{color:var(--muted); font-size:14px; margin-top:12px}

.hero{
  position:relative;
  padding:84px 0 54px;
  background:
    radial-gradient(1000px 400px at 20% 10%, rgba(124,92,255,.35), transparent 60%),
    radial-gradient(800px 420px at 80% 0%, rgba(255,92,174,.25), transparent 60%),
    linear-gradient(180deg, rgba(255,255,255,.06), transparent 60%);
  border-bottom:1px solid var(--line);
}
.hero__overlay{position:absolute; inset:0; background:linear-gradient(180deg, rgba(0,0,0,.35), rgba(0,0,0,.85));}
.hero__content{position:relative}
.kicker{display:flex; gap:10px; align-items:center; margin-bottom:10px}
.badge{font-size:12px; padding:6px 10px; border:1px solid var(--line); border-radius:999px; background:rgba(255,255,255,.03)}
.title{font-size:44px; line-height:1.05; margin-bottom:10px}
.subtitle{color:var(--muted); font-size:16px; margin:0 0 20px 0; max-width:70ch}
.meta{display:flex; gap:14px; flex-wrap:wrap; margin-bottom:22px}
.meta__item{padding:10px 12px; border:1px solid var(--line); border-radius:14px; background:rgba(255,255,255,.03); color:var(--muted)}
.meta__item strong{color:var(--text)}
.btn{display:inline-block; padding:12px 16px; border-radius:14px; background:var(--accent); text-decoration:none; font-weight:600}

.card{
  border:1px solid var(--line);
  background:rgba(255,255,255,.03);
  border-radius:18px;
  padding:16px;
  box-shadow: 0 14px 40px rgba(0,0,0,.25);
}

.section__head{display:flex; align-items:flex-end; justify-content:space-between; gap:20px; margin-bottom:14px}
.section__desc{margin:0; color:var(--muted); max-width:60ch}

.grid{
  display:grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap:14px;
}
@media (max-width: 860px){
  .title{font-size:34px}
  .grid{grid-template-columns:1fr}
}

.film{display:grid; grid-template-columns: 160px 1fr; gap:14px; align-items:stretch}
.film__poster{
  position:relative;
  border-radius:14px;
  overflow:hidden;
  border:1px solid var(--line);
  background:linear-gradient(135deg, rgba(124,92,255,.22), rgba(255,92,174,.10));
  min-height:210px;
}
.film__poster img{width:100%; height:100%; object-fit:cover; display:block}
.poster__placeholder{
  position:absolute; inset:0;
  display:flex; align-items:center; justify-content:center;
  color:rgba(255,255,255,.75);
  font-weight:700;
  letter-spacing:.06em;
}
.film__facts{list-style:none; padding:0; margin:8px 0 10px 0; color:var(--muted); font-size:14px}
.film__facts li{margin:4px 0}
.synopsis{margin:0; color:var(--text); line-height:1.55}

.footer{padding:28px 0; border-top:1px solid var(--line); color:var(--muted); font-size:14px}
