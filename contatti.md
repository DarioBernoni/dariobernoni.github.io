:root{
  --bg:#f7f7f8;
  --surface:#ffffff;
  --text:#111827;
  --muted:#6b7280;
  --line:#e5e7eb;
  --primary:#0f172a;
  --shadow:0 10px 25px rgba(15,23,42,.08);
}
*{box-sizing:border-box}
html,body{margin:0;padding:0}
body{font-family:Inter,ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Helvetica,Arial,sans-serif;background:var(--bg);color:var(--text);line-height:1.65}
.container{width:min(1120px,calc(100% - 32px));margin-inline:auto}
.site-header{position:sticky;top:0;z-index:10;background:rgba(255,255,255,.9);backdrop-filter:saturate(180%) blur(8px);border-bottom:1px solid var(--line)}
.nav{display:flex;align-items:center;justify-content:space-between;min-height:72px;gap:16px}
.brand{color:var(--primary);text-decoration:none;font-weight:800;letter-spacing:-.02em;font-size:1.15rem}
.site-nav{display:flex;gap:18px;align-items:center}
.site-nav a{color:var(--primary);text-decoration:none;font-weight:600}
.nav-toggle{display:none;border:1px solid var(--line);background:#fff;border-radius:10px;padding:8px 10px;font-size:1rem}
.content{padding:32px 0 72px}
.hero{display:grid;grid-template-columns:1.05fr .95fr;gap:32px;align-items:center;margin:12px 0 40px}
.eyebrow{margin:0 0 8px;color:var(--muted);text-transform:uppercase;letter-spacing:.14em;font-size:.78rem;font-weight:700}
.hero h1{margin:0;font-size:clamp(2.2rem,4vw,4.25rem);line-height:1.02;letter-spacing:-.03em}
.lead{margin-top:16px;color:#374151;font-size:1.08rem;max-width:60ch}
.hero-actions{display:flex;gap:12px;flex-wrap:wrap;margin-top:24px}
.button{display:inline-flex;align-items:center;justify-content:center;border-radius:999px;padding:12px 18px;font-weight:700;text-decoration:none;transition:transform .12s ease}
.button.primary{background:var(--primary);color:#fff;box-shadow:var(--shadow)}
.button.ghost{background:#fff;color:var(--primary);border:1px solid var(--line)}
.hero-image img{width:100%;aspect-ratio:4/5;object-fit:cover;border-radius:28px;border:1px solid var(--line);box-shadow:var(--shadow);background:#ddd}
.section{margin-top:40px}
.section-head{display:flex;align-items:end;justify-content:space-between;gap:16px;margin-bottom:18px}
.section h2{margin:0;font-size:1.55rem;letter-spacing:-.02em}
.section-head a{color:var(--primary);text-decoration:none;font-weight:700}
.post-list{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:18px}
.post-card{background:var(--surface);border:1px solid var(--line);border-radius:20px;overflow:hidden;box-shadow:0 1px 2px rgba(0,0,0,.03);transition:transform .12s ease, box-shadow .12s ease}
.post-card:hover{transform:translateY(-2px);box-shadow:var(--shadow)}
.post-card-body{padding:18px 18px 20px}
.post-category{margin:0 0 6px;color:var(--muted);font-size:.9rem;font-weight:700;text-transform:uppercase;letter-spacing:.06em}
.post-card h3{margin:0 0 10px;font-size:1.18rem;line-height:1.25}
.post-card h3 a{color:var(--text);text-decoration:none}
.post-card h3 a:hover{text-decoration:underline}
.post-date{margin:0;color:var(--muted);font-size:.92rem}
.chip-list{display:flex;flex-wrap:wrap;gap:10px}
.chip{background:#fff;border:1px solid var(--line);border-radius:999px;padding:8px 12px;font-size:.92rem;color:#374151}
.post h1{margin-bottom:6px;font-size:2rem;letter-spacing:-.02em}
.post-meta{color:var(--muted);margin-top:0;margin-bottom:24px}
.site-footer{border-top:1px solid var(--line);color:var(--muted);padding:28px 0 40px;text-align:center}
@media (max-width:900px){.hero{grid-template-columns:1fr}.hero-image{order:-1}.hero-image img{aspect-ratio:16/9}.post-list{grid-template-columns:1fr}}
@media (max-width:720px){.nav-toggle{display:inline-flex;align-items:center;justify-content:center}.site-nav{display:none;position:absolute;top:72px;left:16px;right:16px;background:#fff;border:1px solid var(--line);border-radius:16px;padding:12px;box-shadow:var(--shadow);flex-direction:column;align-items:flex-start;gap:8px}.site-nav.open{display:flex}.site-nav a{width:100%;padding:10px 12px;border-radius:10px}.site-nav a:hover{background:#f3f4f6}.section-head{align-items:start;flex-direction:column}}
