<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<title>SLLC Online Course — Imagine1Day</title>
<meta name="description" content="School-Based Literacy and Language Club implementation course for Ethiopian primary schools (Grades 1–8).">
<meta name="theme-color" content="#0d6b50" media="(prefers-color-scheme: light)">
<meta name="theme-color" content="#0e1612" media="(prefers-color-scheme: dark)">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Atkinson+Hyperlegible:wght@400;700&family=Bricolage+Grotesque:opsz,wght@12..96,600;12..96,800&display=swap">
<style>
:root{color-scheme:light;box-sizing:border-box;
  --bg:#f5f7f4; --surface:#ffffff; --surface2:#eaf0ec; --ink:#14201b; --muted:#53635b; --line:#d3ddd6;
  --accent:#0d6b50; --accent-ink:#ffffff; --sun:#f0b323; --sun-ink:#3a2a00; --good:#13795b; --bad:#b3261e; --good-bg:#e1f3ec; --bad-bg:#fbe6e4;
  --head:"Bricolage Grotesque","Atkinson Hyperlegible",system-ui,-apple-system,"Segoe UI",sans-serif;
  --body:"Atkinson Hyperlegible",system-ui,-apple-system,"Segoe UI",sans-serif;
}
@media (prefers-color-scheme: dark){:root:not([data-theme="light"]){
  --bg:#0e1612; --surface:#16211b; --surface2:#1e2c25; --ink:#e8f0eb; --muted:#9db0a5; --line:#2c3d34;
  --accent:#3fbf93; --accent-ink:#06231a; --sun:#f0b323; --sun-ink:#3a2a00; --good:#4fd1a1; --bad:#ff8a80; --good-bg:#12372b; --bad-bg:#40201d; color-scheme:dark}}
:root[data-theme="dark"]{
  --bg:#0e1612; --surface:#16211b; --surface2:#1e2c25; --ink:#e8f0eb; --muted:#9db0a5; --line:#2c3d34;
  --accent:#3fbf93; --accent-ink:#06231a; --sun:#f0b323; --sun-ink:#3a2a00; --good:#4fd1a1; --bad:#ff8a80; --good-bg:#12372b; --bad-bg:#40201d; color-scheme:dark}
html{scroll-padding-top:calc(env(safe-area-inset-top,0px) + 72px)}
*,*::before,*::after{box-sizing:border-box}
img{max-width:100%}
[hidden]:not([hidden=until-found i]){display:none!important}
body{background:var(--bg);color:var(--ink);font:16px/1.6 var(--body);margin:0;padding-block:env(safe-area-inset-top,0px) calc(56px + env(safe-area-inset-bottom,0px));padding-left:max(16px,env(safe-area-inset-left,0px));padding-right:max(16px,env(safe-area-inset-right,0px))}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);background:var(--surface);z-index:30}
h1,h2,h3{font-family:var(--head);line-height:1.15;text-wrap:balance;margin:0}
h1{font-size:clamp(1.9rem,4.8vw,3rem);font-weight:800;letter-spacing:-.02em}
h2{font-size:1.55rem;font-weight:800;letter-spacing:-.01em}
h3{font-size:1.15rem;font-weight:600}
p{margin:0}
a{color:var(--accent)}
[tabindex="-1"]:focus{outline:none}
.skip{position:absolute;left:-999px;top:env(safe-area-inset-top,0px);z-index:100;background:var(--accent);color:var(--accent-ink);padding:10px 16px;text-decoration:none;font-weight:700;border-radius:0 0 10px 0}
.skip:focus{left:0}
.wrap{max-width:1120px;margin:0 auto}
header.top{position:sticky;top:env(safe-area-inset-top,0px);z-index:20;background:var(--surface);border-bottom:1px solid var(--line);margin-inline:calc(-1*max(16px,env(safe-area-inset-left,0px)));padding-inline:max(16px,env(safe-area-inset-left,0px))}
.bar{max-width:1120px;margin:0 auto;display:flex;align-items:center;gap:14px;flex-wrap:wrap;padding:10px 0}
.brand{font-family:var(--head);font-weight:800;font-size:1.08rem;margin-right:auto;display:flex;align-items:center;gap:10px;text-decoration:none;color:var(--ink)}
.mark{width:32px;height:32px;border-radius:8px;background:var(--accent);color:var(--accent-ink);display:grid;place-items:center;font-size:.95rem;font-weight:800}
nav{display:flex;gap:4px;flex-wrap:wrap}
nav a{padding:8px 12px;border-radius:8px;text-decoration:none;color:var(--muted);font-weight:700;font-size:.94rem}
nav a[aria-current="page"]{background:var(--surface2);color:var(--ink)}
nav a:hover{color:var(--ink)}
:focus-visible{outline:3px solid var(--sun);outline-offset:2px}
button,.btn{font:inherit;font-weight:700;border-radius:10px;border:1px solid var(--line);background:var(--surface);color:var(--ink);padding:10px 16px;cursor:pointer;text-decoration:none;display:inline-flex;align-items:center;gap:8px;min-height:44px}
button:hover,.btn:hover{border-color:var(--accent)}
.primary{background:var(--accent);color:var(--accent-ink);border-color:var(--accent)}
.primary:hover{filter:brightness(1.08)}
.sun{background:var(--sun);color:var(--sun-ink);border-color:var(--sun)}
button[disabled]{opacity:.5;cursor:not-allowed}
.theme-btn{min-height:40px;min-width:40px;padding:0 10px;font-size:1.1rem;line-height:1;border-radius:10px}
input[type=text],input[type=email],input[type=password],input[type=url]{font:inherit;width:100%;padding:11px 12px;border-radius:10px;border:1px solid var(--line);background:var(--bg);color:var(--ink);min-height:44px}
label{display:block;font-weight:700;margin-bottom:4px;font-size:.95rem}
.field{display:grid;gap:4px;margin-bottom:14px}
.hint{color:var(--muted);font-size:.9rem}
.card{background:var(--surface);border:1px solid var(--line);border-radius:14px;padding:22px}
.row{display:flex;gap:12px;flex-wrap:wrap;align-items:center}
.grid2{display:grid;grid-template-columns:1fr 1fr;gap:20px}
.stack{display:grid;gap:16px}
.pill{display:inline-flex;align-items:center;gap:6px;font-size:.8rem;font-weight:700;padding:3px 10px;border-radius:99px;background:var(--surface2);color:var(--muted);letter-spacing:.02em}
.pill.ok{background:var(--good-bg);color:var(--good)}
.pill.sunp{background:var(--sun);color:var(--sun-ink)}
.msg{padding:12px 14px;border-radius:10px;font-weight:700}
.msg.bad{background:var(--bad-bg);color:var(--bad)}
.msg.good{background:var(--good-bg);color:var(--good)}
.msg.info{background:var(--surface2);color:var(--ink);font-weight:400}
.hero{padding:38px 0 24px;display:grid;gap:16px;max-width:780px}
.hero p.lead{font-size:1.12rem;color:var(--muted)}
.steps{counter-reset:s;display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin:8px 0 28px;padding:0;list-style:none}
.steps li{counter-increment:s;background:var(--surface);border:1px solid var(--line);border-radius:14px;padding:16px 18px}
.steps li::before{content:counter(s);display:grid;place-items:center;width:28px;height:28px;border-radius:50%;background:var(--sun);color:var(--sun-ink);font-weight:800;margin-bottom:8px}
.steps b{display:block;font-family:var(--head);margin-bottom:4px}
.copybox{background:var(--bg);border:1px dashed var(--line);border-radius:10px;padding:12px;font-family:ui-monospace,Menlo,Consolas,monospace;font-size:.85rem;white-space:pre-wrap;word-break:break-all;user-select:all}
.copyrow{display:flex;gap:8px;align-items:center;flex-wrap:wrap}
.course{display:grid;grid-template-columns:295px minmax(0,1fr);gap:24px;padding-top:24px;align-items:start}
.rail{position:sticky;top:calc(env(safe-area-inset-top,0px) + 74px);display:grid;gap:4px;max-height:calc(100vh - 104px);overflow:auto}
.rail button{justify-content:flex-start;text-align:left;border:1px solid transparent;background:none;font-weight:400;padding:9px 10px;border-radius:10px;width:100%;line-height:1.3}
.rail button[aria-current="true"]{background:var(--surface2);border-color:var(--line);font-weight:700}
.rail .n{flex:0 0 26px;height:26px;border-radius:50%;display:grid;place-items:center;font-size:.8rem;font-weight:700;background:var(--surface2);color:var(--muted)}
.rail .done .n{background:var(--good);color:var(--accent-ink)}
.menu{display:none}
.progress{height:8px;border-radius:99px;background:var(--surface2);overflow:hidden}
.progress i{display:block;height:100%;background:var(--accent);transition:width .25s ease}
.lesson{display:grid;gap:22px;min-width:0}
.lesson section{display:grid;gap:10px}
.lesson ul{margin:0;padding-left:1.2rem;display:grid;gap:6px}
.tablewrap{overflow-x:auto;border:1px solid var(--line);border-radius:10px}
table{border-collapse:collapse;width:100%;min-width:520px;font-size:.95rem}
th,td{text-align:left;padding:10px 12px;border-bottom:1px solid var(--line);vertical-align:top}
th{background:var(--surface2);font-family:var(--head)}
tr:last-child td{border-bottom:0}
.q{border:1px solid var(--line);border-radius:12px;padding:16px;display:grid;gap:10px;background:var(--surface);min-width:0}
.q legend{font-weight:700;padding:0 4px}
fieldset{border:0;margin:0;padding:0;min-width:0}
.opt{display:flex;gap:10px;align-items:flex-start;padding:10px 12px;border:1px solid var(--line);border-radius:10px;cursor:pointer;font-weight:400;margin:0}
.opt input{margin-top:5px;accent-color:var(--accent)}
.opt.right{border-color:var(--good);background:var(--good-bg)}
.opt.wrong{border-color:var(--bad);background:var(--bad-bg)}
.why{font-size:.92rem;color:var(--muted)}
.cert{background:#fffdf5;color:#1d2b24;border:1px solid var(--line);border-radius:10px;overflow:hidden}
.cert svg{display:block;width:100%;height:auto}
.stat{display:flex;gap:28px;flex-wrap:wrap}
.stat div b{display:block;font-family:var(--head);font-size:1.8rem;color:var(--accent)}
.res{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:12px;padding:0;margin:0;list-style:none}
.res a{display:grid;gap:4px;height:100%;padding:14px;border:1px solid var(--line);border-radius:12px;background:var(--surface);text-decoration:none;color:var(--ink)}
.res a:hover{border-color:var(--accent)}
.res b{font-family:var(--head);font-weight:600;line-height:1.25}
.res span.d{color:var(--muted);font-size:.9rem}
.k{justify-self:start;font-size:.75rem;font-weight:700;letter-spacing:.04em;text-transform:uppercase;padding:2px 8px;border-radius:6px;background:var(--surface2);color:var(--muted)}
.k.video{background:var(--bad-bg);color:var(--bad)}
.k.audio{background:var(--sun);color:var(--sun-ink)}
.k.tool{background:var(--good-bg);color:var(--good)}
footer{max-width:1120px;margin:40px auto 0;color:var(--muted);font-size:.88rem;border-top:1px solid var(--line);padding-top:16px}
@media (max-width:860px){
  .course{grid-template-columns:1fr}
  .rail{display:none}
  .menu{display:block}
  .grid2,.steps{grid-template-columns:1fr}
  .menu summary{cursor:pointer;font-weight:700;padding:12px 14px;background:var(--surface);border:1px solid var(--line);border-radius:10px}
  .menu .rail{display:grid;position:static;max-height:none;margin-top:8px}
}
textarea,select{font:inherit;width:100%;padding:11px 12px;border-radius:10px;border:1px solid var(--line);background:var(--bg);color:var(--ink)}
textarea{min-height:120px;resize:vertical}
select{min-height:44px}
.vis{background:var(--surface);border:1px solid var(--line);border-radius:14px;padding:16px;display:grid;gap:10px}
.vis .cap{font-family:var(--head);font-weight:600}
.flow{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:8px;list-style:none;padding:0;margin:0}
.flow li{background:var(--surface2);border:1px solid var(--line);border-radius:12px;padding:10px 12px;font-size:.92rem;line-height:1.35}
.flow li b{display:grid;place-items:center;width:26px;height:26px;border-radius:50%;background:var(--accent);color:var(--accent-ink);font-size:.82rem;margin-bottom:6px}
.hub{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:8px}
.hub .c{grid-column:1/-1;text-align:center;background:var(--accent);color:var(--accent-ink);border-radius:12px;padding:12px;font-family:var(--head);font-weight:800}
.hub .i{background:var(--surface2);border:1px solid var(--line);border-radius:12px;padding:10px 12px;text-align:center;font-size:.92rem}
.cols{display:grid;grid-template-columns:repeat(auto-fit,minmax(190px,1fr));gap:10px}
.cols>div{border:1px solid var(--line);border-radius:12px;background:var(--surface2);padding:12px}
.cols h4{margin:0 0 6px;font-family:var(--head)}
.cols ul{margin:0;padding-left:1.1rem;font-size:.92rem;display:grid;gap:3px}
.res.vid a{border-left:4px solid var(--bad)}
.k.video::before{content:"\25B6\00a0"}
.prac{border:2px solid var(--sun);border-radius:14px;padding:20px;background:var(--surface);display:grid;gap:12px}
.pdot{display:inline-block;width:8px;height:8px;border-radius:50%;background:var(--sun);margin-left:auto;flex:0 0 auto}
@media (prefers-reduced-motion:reduce){*{transition:none!important;animation:none!important}}
@media print{
  header.top,nav,.skip,footer,.no-print{display:none!important}
  body{background:#fff;color:#000;padding:0}
  .wrap{max-width:none}
  .cert{border:0;border-radius:0}
}
</style>
</head>
<body>
<a class="skip" href="#app">Skip to main content</a>
<header class="top"><div class="bar">
  <a class="brand" href="#home"><span class="mark" aria-hidden="true">Aa</span>SLLC Online Course</a>
  <nav id="nav" aria-label="Main"></nav>
  <button type="button" id="theme-toggle" class="theme-btn" aria-label="Toggle colour theme" aria-pressed="false" title="Toggle colour theme">☾</button>
</div></header>
<main class="wrap" id="app" tabindex="-1"></main>
<footer id="foot"></footer>

<script>
/* ======= SETTINGS the course owner can change ======= */
const CFG = {
  org: "Imagine1Day International Organizations",
  course: "School-Based Literacy and Language Club (SLLC)",
  sub: "Reading & Writing Club implementation course for Ethiopian primary schools (Grades 1–8)",
  ownerEmail: "mohammedscho2023@gmail.com",
  social: { name: "SLLC Practitioners Community", url: "" },
  passModule: 3,          // correct answers needed (out of 4) to complete a module
  examSize: 30,
  passPct: 70,
  practiceMin: 10,        // practice tasks (out of 14) needed for the certificate
  practiceMinChars: 40,   // minimum length of a written practice answer
  salt: "imagine1day-sllc-2026-x7Qm",
  pageUrl: "https://claude.ai/artifact/H7AYWxnnBFwjDHb8yznzLo",
  instructorHash: "3b7af1bb3e422b7d1c9fd21c9d5e10d8a21d1bdc30f9f4fc92d2902a6a773c3c"
};

/* SHA-256 using TextEncoder for UTF-8 handling */
function sha256(s){
  const K=[0x428a2f98,0x71374491,0xb5c0fbcf,0xe9b5dba5,0x3956c25b,0x59f111f1,0x923f82a4,0xab1c5ed5,0xd807aa98,0x12835b01,0x243185be,0x550c7dc3,0x72be5d74,0x80deb1fe,0x9bdc06a7,0xc19bf174,0xe49b69c1,0xefbe4786,0x0fc19dc6,0x240ca1cc,0x2de92c6f,0x4a7484aa,0x5cb0a9dc,0x76f988da,0x983e5152,0xa831c66d,0xb00327c8,0xbf597fc7,0xc6e00bf3,0xd5a79147,0x06ca6351,0x14292967,0x27b70a85,0x2e1b2138,0x4d2c6dfc,0x53380d13,0x650a7354,0x766a0abb,0x81c2c92e,0x92722c85,0xa2bfe8a1,0xa81a664b,0xc24b8b70,0xc76c51a3,0xd192e819,0xd6990624,0xf40e3585,0x106aa070,0x19a4c116,0x1e376c08,0x2748774c,0x34b0bcb5,0x391c0cb3,0x4ed8aa4a,0x5b9cca4f,0x682e6ff3,0x748f82ee,0x78a5636f,0x84c87814,0x8cc70208,0x90befffa,0xa4506ceb,0xbef9a3f7,0xc67178f2];
  const b = Array.from(new TextEncoder().encode(s));
  const l = b.length * 8;
  b.push(0x80);
  while (b.length % 64 !== 56) b.push(0);
  for (let i = 7; i >= 0; i--) b.push(i > 3 ? 0 : (l >>> (i * 8)) & 255);
  let h = [0x6a09e667,0xbb67ae85,0x3c6ef372,0xa54ff53a,0x510e527f,0x9b05688c,0x1f83d9ab,0x5be0cd19];
  const R = (x, n) => (x >>> n) | (x << (32 - n));
  for (let o = 0; o < b.length; o += 64) {
    const w = new Array(64);
    for (let i = 0; i < 16; i++) w[i] = (b[o + 4*i] << 24) | (b[o + 4*i + 1] << 16) | (b[o + 4*i + 2] << 8) | b[o + 4*i + 3];
    for (let i = 16; i < 64; i++) {
      const s0 = R(w[i-15],7) ^ R(w[i-15],18) ^ (w[i-15] >>> 3);
      const s1 = R(w[i-2],17) ^ R(w[i-2],19) ^ (w[i-2] >>> 10);
      w[i] = (w[i-16] + s0 + w[i-7] + s1) | 0;
    }
    let [a,c,d,e,f,g,hh,j] = h;
    for (let i = 0; i < 64; i++) {
      const S1 = R(f,6) ^ R(f,11) ^ R(f,25), ch = (f & g) ^ (~f & hh), t1 = (j + S1 + ch + K[i] + w[i]) | 0;
      const S0 = R(a,2) ^ R(a,13) ^ R(a,22), mj = (a & c) ^ (a & d) ^ (c & d), t2 = (S0 + mj) | 0;
      j = hh; hh = g; g = f; f = (e + t1) | 0; e = d; d = c; c = a; a = (t1 + t2) | 0;
    }
    h = [h[0]+a,h[1]+c,h[2]+d,h[3]+e,h[4]+f,h[5]+g,h[6]+hh,h[7]+j].map(x => x | 0);
  }
  return h.map(x => (x >>> 0).toString(16).padStart(8,'0')).join('');
}

/* ======= Safe Storage ======= */
const memStore = new Map();
function saveState(key, val) {
  const raw = JSON.stringify(val);
  memStore.set(key, raw);
  try { localStorage.setItem("sllc_" + key, raw); } catch (_) {}
}
function loadState(key, fallback) {
  let raw = memStore.get(key);
  if (raw == null) {
    try { raw = localStorage.getItem("sllc_" + key); } catch (_) {}
  }
  if (!raw) return fallback;
  try { return JSON.parse(raw); } catch (_) { return fallback; }
}

/* ======= Curriculum Data (8 Modules, 14 Practice Tasks, 32 Exam Questions) ======= */
const MODULES = [
  {
    id: 1, title: "Understanding School-Based Literacy Improvement", mins: 35,
    intro: "School-based literacy improvement is a planned, continuous effort led by the school itself (directors, teachers, volunteers, parents and students) so that all children learn to read and write well, especially in the early grades and in their mother tongue.",
    visual: {
      cap: "School-Based Literacy Improvement Cycle",
      type: "flow",
      items: [
        "Identify local literacy gaps (e.g., Grade 2 word decoding)",
        "Set measurable school targets (e.g., 80% at 40+ WCPM)",
        "Mobilise lessons, clubs, corners, buddies & families",
        "Monitor with quick checks & adapt instruction"
      ]
    },
    sections: [
      { h: "The core idea", l: [
        "The school identifies its own literacy challenges, for example many Grade 2 students cannot read simple words.",
        "It sets clear goals, for example 80% of Grade 2 students reading at least 40 words correct per minute by June.",
        "It plans and carries out actions: TaRL, better teaching, extra practice time, reading clubs, reading corners, volunteer support and parent engagement.",
        "It checks progress regularly and adjusts the plan using evidence such as simple assessments, observation and student work."
      ]},
      { h: "Seven key components", l: [
        "Strong classroom instruction in reading and writing",
        "Extra practice time through clubs and activities",
        "Access to supplementary reading materials",
        "Support for struggling learners",
        "Inclusion, gender equity and language considerations",
        "Parent and community engagement",
        "Monitoring, review and continuous improvement"
      ]},
      { h: "Five types of school-based literacy activity", table: {
        head: ["Type", "Examples"],
        rows: [
          ["Classroom reading and writing lessons", "Letter/Fidel sounds, blending, guided reading, TaRL classrooms"],
          ["Co-curricular literacy clubs", "Reading and Writing Club, 1–2 times a week, about 90 minutes"],
          ["Reading corners and spaces", "Classroom shelves, reading room, community book banks"],
          ["Volunteer, peer and family support", "Reading buddies, parents listening to children read"],
          ["School-wide events", "Fluency competitions, storytelling contests, literacy weeks"]
        ]
      }},
      { h: "The five key reading skills", table: {
        head: ["Skill", "What it means", "Example"],
        rows: [
          ["Phonemic awareness", "Hearing and manipulating individual sounds in spoken words (oral, no letters)", "Segmenting a spoken word into onset and rime or individual sounds"],
          ["Phonics", "Linking letters (graphemes) to sounds (phonemes)", "Connecting Fidel characters or Latin letter blends to sounds"],
          ["Fluency", "Reading accurately, smoothly and with expression", "Choral, paired and repeated reading"],
          ["Vocabulary", "Words a learner knows and uses", "Teaching harvest with a sentence and discussion"],
          ["Comprehension", "Understanding, interpreting and thinking about text", "Why did Sara carry an umbrella?"]
        ]
      }},
      { h: "Eight principles of effective literacy development", l: [
        "Start with the mother tongue",
        "Teach the five key reading skills explicitly",
        "Integrate reading, writing, speaking and listening",
        "Provide lots of practice with appropriate texts: decodable, levelled, culturally relevant, narrative and informational",
        "Differentiate support for struggling learners",
        "Ensure inclusion and gender equity",
        "Create a print-rich, supportive environment",
        "Monitor progress and use data to improve"
      ]}
    ],
    practice: [
      { id: "p1", prompt: "Describe one realistic mother-tongue literacy gap in Grades 1–4 at your school (or a school you support), state a concrete target for the term, and name two school-led actions." },
      { id: "p2", prompt: "Give one classroom or club activity example for each of the five reading skills (phonemic awareness, phonics, fluency, vocabulary, comprehension)." }
    ],
    quiz: [
      { q: "What makes literacy improvement “school-based”?", o: ["Decisions come only from the regional education bureau","Decisions are made at school level, led by teachers and school leaders with support from supervisors, PTSA and communities","Only textbooks supplied by the woreda are used","Only volunteers from outside the school lead it"], a: 1, why: "The approach is school-based because decisions are made at school level and rooted in the school's daily reality." },
      { q: "Which skill is an oral language skill that does not involve printed letters?", o: ["Phonics","Fluency","Phonemic awareness","Writing"], a: 2, why: "Phonemic awareness is hearing, identifying and manipulating sounds in spoken words." },
      { q: "Why should instruction begin in the mother tongue?", o: ["Children learn to read and write best in a language they understand, and this supports later learning of other languages","It is cheaper for schools","English should never be taught","It removes the need for assessment"], a: 0, why: "Strong mother-tongue literacy supports later learning of additional languages such as English." },
      { q: "Texts for practice should be…", o: ["Only very long and difficult","Decodable, levelled, interesting and culturally relevant","Only informational","Only chosen by volunteers without checking level"], a: 1, why: "Texts should match sounds taught, match reading ability, interest children and include both narrative and informational types." }
    ]
  },
  {
    id: 2, title: "The School-Based Literacy and Language Club (SLLC)", mins: 30,
    intro: "The SLLC is a student-centred extracurricular platform within a school that improves literacy, language, communication and reading skills through organised and enjoyable activities beyond regular lessons.",
    visual: {
      cap: "Integrated SLLC Platform",
      type: "hub",
      center: "School-Based Literacy & Language Club (SLLC)",
      items: ["Guided Reading Circles","Creative & Functional Writing","Oral Storytelling & Poetry","Structured Debate & Public Speaking","Drama & Role-Play","Peer Literacy Support"]
    },
    sections: [
      { h: "Purpose", l: [
        "Improve reading, writing, speaking and listening",
        "Build a culture of reading and lifelong learning",
        "Strengthen the language of instruction and other languages taught",
        "Develop communication, collaboration, leadership and critical thinking",
        "Support struggling readers and writers with inclusive participation",
        "Offer storytelling, debates, public speaking, reading circles, drama, poetry and creative writing"
      ]},
      { h: "Why one integrated club?", l: [
        "Literacy skills are interconnected: reading, writing, speaking and listening reinforce each other.",
        "Efficient use of limited resources, facilitators and meeting time.",
        "Inclusive participation: varied activities appeal to different strengths.",
        "Stronger learning, communication, reading culture, academic achievement and leadership skills.",
        "Less duplication and administrative workload, and a sustainable framework."
      ]},
      { h: "General objective", p: "To enhance students' literacy and language competencies through participatory, enjoyable and inclusive activities that promote reading, writing, speaking, listening and critical thinking." },
      { h: "Eleven guiding principles", l: [
        "Learner-centred participation","Inclusiveness and equity","Voluntary and enjoyable learning","Holistic literacy development",
        "Respect for diversity","Collaboration and teamwork","Creativity and innovation","Leadership and responsibility",
        "Continuous learning and improvement","Community and stakeholder engagement","Child protection and a safe learning environment"
      ]}
    ],
    practice: [
      { id: "p3", prompt: "Explain how merging separate reading, debate, or drama clubs into one integrated SLLC reduces teacher workload and strengthens student literacy in a primary school." },
      { id: "p4", prompt: "Outline a sample 90-minute SLLC session structure for Grades 5–8 that blends reading, writing, and oral language." }
    ],
    quiz: [
      { q: "What is the main advantage of one integrated literacy club over separate clubs?", o: ["It needs no facilitators","It combines reading, writing, speaking and listening under one coordinated platform, saving resources and reducing duplication","It only serves the best readers","It replaces classroom lessons"], a: 1, why: "Integration recognises that literacy skills are interconnected and maximises limited resources." },
      { q: "Which principle says participation should be based on students' interest?", o: ["Voluntary and enjoyable learning","Continuous improvement","Holistic development","Community engagement"], a: 0, why: "Participation should come from interest and enthusiasm, with interactive, enjoyable activities." },
      { q: "Who are the primary actors in planning, implementing and evaluating club activities?", o: ["Only teachers","Only the school director","Students","Only parents"], a: 2, why: "Learner-centred participation makes students the primary actors." },
      { q: "The SLLC should give equal opportunities regardless of…", o: ["Only gender","Gender, language background, disability, socioeconomic status or academic performance","Only academic performance","Nothing; places are limited to top learners"], a: 1, why: "Inclusiveness and equity cover all these dimensions, with special attention to marginalised and struggling learners." }
    ]
  },
  {
    id: 3, title: "Club Leadership and Management", mins: 35,
    intro: "A clear committee structure, defined roles, annual and weekly plans and regular review meetings keep the club accountable and running smoothly.",
    sections: [
      { h: "Committee roles", table: {
        head: ["Position", "Key responsibilities"],
        rows: [
          ["Chairperson / President", "Overall leadership, chairs meetings, represents the club, ensures plans are implemented"],
          ["Vice Chairperson", "Supports the Chairperson, acts when the Chairperson is absent, monitors progress"],
          ["Secretary", "Agendas, minutes, records, correspondence and membership register"],
          ["Treasurer", "Financial records, budgets and reports, transparency"],
          ["Program / Activity Coordinator", "Activity schedules, event plans, monitors and reports outcomes"],
          ["Membership Coordinator", "Recruits and orients members, keeps records, promotes retention"],
          ["Communications Officer", "Shares information, publicises activities and achievements"]
        ]
      }},
      { h: "Best practices for committees", l: [
        "Define terms of office and election procedures",
        "Hold regular committee meetings and document decisions and actions",
        "Ensure transparency in financial and operational matters",
        "Promote gender balance, inclusion and active member participation"
      ]},
      { h: "Annual planning steps", l: [
        "Review the previous year's performance","Identify priorities, opportunities and challenges","Set annual goals and objectives",
        "Develop activities and timelines","Assign responsibilities","Prepare a budget and resource plan",
        "Obtain committee approval","Communicate the plan to members"
      ]},
      { h: "Weekly timetable and review meetings", l: [
        "Weekly timetable: identify the week's activities, allocate dates, times and venues, assign people, confirm resources, share with members.",
        "Review meetings come in four types: weekly, monthly, quarterly and annual review and planning.",
        "Standard agenda: welcome, previous minutes and actions, progress updates, challenges, financial update, decisions and actions, planning ahead, closing.",
        "Outputs: minutes, updated action plan, progress reports, recommendations and agreed next steps."
      ]}
    ],
    practice: [
      { id: "p5", prompt: "Draft a brief student-committee election and gender-balance plan for an SLLC serving Grades 1–8, naming at least four committee roles and their teacher mentor link." },
      { id: "p6", prompt: "Write a one-week SLLC timetable (day, time, venue, activity, lead, materials) and list what you will check at the weekly review meeting." }
    ],
    quiz: [
      { q: "Who records and distributes meeting minutes and keeps the membership register?", o: ["Treasurer","Secretary","Communications Officer","Vice Chairperson"], a: 1, why: "The Secretary prepares agendas, records minutes and maintains records and the membership register." },
      { q: "Which is the FIRST step in annual planning?", o: ["Prepare the budget","Review the previous year's performance","Assign responsibilities","Obtain committee approval"], a: 1, why: "Planning begins by reviewing last year's performance." },
      { q: "Which is NOT one of the four types of review meeting?", o: ["Weekly","Monthly","Quarterly","Daily"], a: 3, why: "The manual lists weekly, monthly, quarterly and annual review meetings." },
      { q: "Who manages budgets and financial reports?", o: ["Treasurer","Membership Coordinator","Program Coordinator","Chairperson only"], a: 0, why: "The Treasurer maintains financial records and prepares budgets and reports." }
    ]
  },
  {
    id: 4, title: "Student Participation and Inclusion", mins: 35,
    intro: "All learners should have equal opportunities to benefit. Clubs identify and support vulnerable students, promote gender equity, include children with disabilities and create safe, accessible spaces.",
    sections: [
      { h: "Students who may need additional support", l: [
        "Students with disabilities or learning difficulties",
        "Girls facing social or cultural barriers",
        "Children from economically disadvantaged households",
        "Orphans and vulnerable children",
        "Students with frequent absenteeism",
        "Students with emotional or psychosocial challenges or language and communication difficulties"
      ]},
      { h: "Identifying and supporting", l: [
        "Identify through classroom observation, attendance monitoring, talks with students and parents, teacher referrals, peer feedback and community assessments.",
        "Support through mentoring, tutoring, referral to specialised services, learning materials, psychosocial activities and regular follow-up.",
        "Maintain confidentiality and dignity, avoid labelling or stigma, and involve parents and caregivers."
      ]},
      { h: "Gender equity", l: [
        "Encourage girls and boys to participate equally and balance club committees.",
        "Use inclusive language, remove participation barriers and give leadership opportunities to all.",
        "Indicators: balanced membership, equal participation, fair leadership distribution, reduced absenteeism and dropout."
      ]},
      { h: "Disability inclusion and safe environments", l: [
        "Adapt activities, use accessible communication, arrange seating and spaces, encourage peer support and give extra time when needed.",
        "Focus on abilities rather than limitations and consult students and caregivers.",
        "Safe environment: respectful relationships, clear rules, protection from bullying and discrimination.",
        "Accessible environment: safe physical access, adequate lighting and seating, clear instructions and flexible participation."
      ]},
      { h: "Safety and accessibility checklist", table: {
        head: ["Area", "Checklist item"],
        rows: [
          ["Physical environment", "Learning space is clean and safe"],
          ["Accessibility", "Students can enter and move around comfortably"],
          ["Participation", "All students have opportunities to contribute"],
          ["Communication", "Information is clear and understandable"],
          ["Protection", "Procedures exist for reporting concerns"],
          ["Inclusion", "Activities are adapted for different needs"]
        ]
      }}
    ],
    practice: [
      { id: "p7", prompt: "Identify three practical barriers that prevent girls or children with disabilities from joining an after-school SLLC, and state how your club will remove each barrier confidentially." },
      { id: "p8", prompt: "Design an adapted storytelling or reading-circle activity so a student with low vision or speech/hearing difficulty participates actively rather than passively." }
    ],
    quiz: [
      { q: "Which is a best practice when supporting vulnerable students?", o: ["Announce their needs to the whole group","Maintain confidentiality and dignity and avoid labelling","Exclude them from leadership","Move them to separate clubs"], a: 1, why: "Confidentiality, dignity and avoiding stigma are core practices." },
      { q: "Which is an indicator of gender equity?", o: ["Only boys hold leadership roles","Balanced club membership by gender and fair distribution of leadership","Girls attend on separate days","No attendance records are kept"], a: 1, why: "Balanced membership, equal participation and fair leadership are indicators." },
      { q: "Inclusion of children with disabilities means…", o: ["They watch from the side","They participate fully, actively and meaningfully, with barriers removed","They only join once a year","Parents lead their sessions"], a: 1, why: "Inclusion is full, active and meaningful participation." },
      { q: "Which method helps identify students needing support?", o: ["Attendance monitoring and teacher referrals","Guessing from appearance","Ranking by family income publicly","Waiting for complaints"], a: 0, why: "Observation, attendance monitoring, referrals and talks with parents are the listed methods." }
    ]
  },
  {
    id: 5, title: "Volunteers and the Reading Buddy Programme", mins: 40,
    intro: "Volunteers strengthen learning support. Good recruitment, selection, supervision and recognition make the programme safe, effective and lasting.",
    sections: [
      { h: "Recruitment", l: [
        "Sources: senior students and peer leaders, parents and caregivers, community members, retired teachers and professionals, youth groups, alumni and former club members.",
        "Process: identify needs and roles, write role descriptions, advertise, do outreach, receive applications, screen and select, then orient and train.",
        "Keep records of applications and placements and ensure transparency and equal opportunity."
      ]},
      { h: "Selection criteria", l: [
        "Commitment to children and education, communication skills, reliability, positive attitude, respect for diversity, teamwork and adequate literacy skills.",
        "Process: review applications, interview where needed, verify references, assess suitability for working with children, decide transparently and notify with orientation.",
        "Principles: fairness, non-discrimination, child safeguarding and transparency."
      ]},
      { h: "Reading Buddy pairing and routines", l: [
        "Pair older/stronger readers or trained volunteers with early-grade or struggling readers in small groups or 1-on-1 pairs.",
        "Use short 20–30 minute predictable routines: warm-up sound/word check, paired/echo reading, comprehension question, praise log.",
        "Rotate pairs periodically and keep buddy sessions visible in open school spaces with clear safeguarding rules."
      ]},
      { h: "Supervision, retention and recognition", l: [
        "Provide brief pre-service orientation on child safeguarding, praise-based feedback and simple reading routines.",
        "Supervise lightly via club coordinators and focal teachers; recognise volunteers through certificates, community appreciation events and peer spotlights."
      ]}
    ],
    practice: [
      { id: "p9", prompt: "Write a 25-minute Reading Buddy routine for a Grade 6 buddy working with a Grade 2 learner who struggles with blending, including child-safeguarding ground rules." },
      { id: "p10", prompt: "List your recruitment sources for SLLC volunteers in your community and describe one low-cost way to retain and recognise them over a school year." }
    ],
    quiz: [
      { q: "Why should volunteer selection include suitability checks for working with children?", o: ["To reduce club attendance","To uphold child protection and ensure a safe learning environment","To favour only former teachers","To avoid training volunteers"], a: 1, why: "Safeguarding and child protection are core principles in volunteer recruitment and selection." },
      { q: "Which is a strong feature of an effective Reading Buddy session?", o: ["Unstructured 2-hour lectures","Short, predictable routines with paired reading, encouragement and safeguarding oversight","Grading buddies on punishment","Pairing struggling learners with unbriefed strangers"], a: 1, why: "Predictable routines, supportive practice and safeguarding keep buddy pairs effective and safe." },
      { q: "Who can serve as SLLC volunteers?", o: ["Only university graduates","Senior students, parents, retired teachers, youth groups and community members","Only external NGO staff","Only school directors"], a: 1, why: "Broad local recruitment taps senior students, parents, alumni, youth and community members." },
      { q: "What helps sustain volunteer motivation over time?", o: ["Ignoring their attendance","Clear orientation, supportive supervision and public recognition","Changing roles every 5 minutes","Withholding feedback"], a: 1, why: "Orientation, light supervision and recognition support retention." }
    ]
  },
  {
    id: 6, title: "Reading Corners, Materials and Print-Rich Spaces", mins: 30,
    intro: "Children need accessible, varied, culturally familiar texts close at hand—inside classrooms, reading corners and community book banks.",
    sections: [
      { h: "Building low-cost print-rich spaces", l: [
        "Create classroom reading corners using shelves, sacks, cardboard crates or hanging pockets.",
        "Display student writing: stories, poems, riddles, local proverbs and illustrated posters.",
        "Label classroom objects and zones in the mother tongue and language of instruction."
      ]},
      { h: "Selecting and levelling texts", l: [
        "Balance decodable texts (for early phonics/Fidel practice), levelled readers, narrative stories and informational texts.",
        "Include local folktales, community livelihoods, health, environment and girls' leadership stories.",
        "Sort books by difficulty level with simple colour or number tags so learners pick texts they can succeed with."
      ]},
      { h: "Book care, lending and community book banks", l: [
        "Teach simple book-handling habits (clean hands, no folding corners, bookmark use) and repair torn pages with paper/tape.",
        "Use simple classroom lending logs and partner with PTSA/kebele libraries to build community book banks."
      ]}
    ],
    practice: [
      { id: "p11", prompt: "Describe how you would set up or upgrade a classroom reading corner with locally available materials, including how books are levelled and borrowed." }
    ],
    quiz: [
      { q: "Why should reading corners include both decodable and levelled/informational texts?", o: ["To decorate walls","So beginning decoders and fluent readers both have texts matched to their skill and interests","To replace textbooks","So only teachers read them"], a: 1, why: "Matched texts build confidence across reading stages and genres." },
      { q: "What is a practical way to make a reading corner sustainable in resource-constrained schools?", o: ["Locking all books in the director's office","Using local containers/shelves, student-created texts, simple book repair and PTSA/community book banks","Waiting for imported books only","Banning book borrowing"], a: 1, why: "Local materials, student authorship and community book banks sustain access." },
      { q: "What makes a classroom environment print-rich?", o: ["Bare walls","Student writing, word walls, labels, reading corners and accessible storybooks","Only exam timetables","Silent rooms with no books"], a: 1, why: "Print-rich spaces surround learners with meaningful, readable print." },
      { q: "How should young learners choose books from a reading corner?", o: ["Randomly without guidance","Using clear level markers and teacher/peer guidance so texts are appropriately challenging","Only the thickest book","By waiting for annual distribution"], a: 1, why: "Simple level markers help learners select readable, engaging books." }
    ]
  },
  {
    id: 7, title: "Linking SLLC with Classroom Instruction and TaRL", mins: 35,
    intro: "The SLLC thrives when club facilitators, classroom teachers and Teaching at the Right Level (TaRL) groups reinforce the same foundational skills.",
    sections: [
      { h: "Bridging classroom and club", l: [
        "Share weekly letter/sound, vocabulary or writing focuses between Grade 1–4 teachers and SLLC facilitators.",
        "Use club games, word cards, syllable/Fidel hunts and story retelling to reinforce classroom lessons without copying boring drills."
      ]},
      { h: "Supporting TaRL (Teaching at the Right Level) groups", l: [
        "Group learners by actual reading level (e.g., beginner, letter/Fidel, word, paragraph, story) rather than age alone.",
        "Use short, joyful, level-matched activities in SLLC to help lower-level readers move up levels."
      ]},
      { h: "Writing across the club", l: [
        "Pair reading with short functional and creative writing: sentence building, dialogue journals, school news sheets, riddles and letters."
      ]}
    ],
    practice: [
      { id: "p12", prompt: "Explain how an SLLC coordinator and Grade 1–3 teachers can align weekly literacy priorities and support learners currently at letter/word level in TaRL." }
    ],
    quiz: [
      { q: "How does SLLC best complement classroom and TaRL instruction?", o: ["By teaching completely unrelated topics","By reinforcing core sounds, vocabulary and comprehension through active, level-appropriate club activities","By testing students every 10 minutes","By separating Grades 1 and 8 permanently"], a: 1, why: "Alignment reinforces foundational skills while keeping club sessions active and engaging." },
      { q: "In TaRL-aligned practice, how are learners grouped for targeted support?", o: ["By height","By current reading competency level","By alphabetical order","By uniform colour"], a: 1, why: "TaRL groups learners by actual reading level so instruction meets them where they are." },
      { q: "How should writing be integrated into SLLC?", o: ["Only copying long paragraphs from the board","Through short, purposeful activities like word/sentence games, story retelling, riddles and club newsletters","Skipping writing completely","Only grading spelling with red ink"], a: 1, why: "Purposeful, low-stress writing builds confidence and links to reading." },
      { q: "Who should coordinate between classroom lessons and SLLC?", o: ["Only external evaluators","Club focal teachers, student committee leads and classroom teachers","Only security guards","No coordination is needed"], a: 1, why: "Focal teachers, classroom teachers and student leads keep learning connected." }
    ]
  },
  {
    id: 8, title: "Monitoring, Family Engagement and Sustainability", mins: 35,
    intro: "Simple tracking, family partnerships, PTSA/kebele support and school-wide literacy showcases keep the SLLC alive beyond project cycles.",
    sections: [
      { h: "Simple monitoring and evidence", l: [
        "Track membership and attendance disaggregated by sex, grade and disability/inclusion status.",
        "Collect qualitative evidence: sample student writings, reading buddy logs, observation notes and quarterly reflections."
      ]},
      { h: "Engaging parents, PTSA and community", l: [
        "Invite parents to storytelling days, home reading habits and book-bank contributions.",
        "Brief PTSA and woreda/cluster supervisors during review meetings so SLLC is part of the School Improvement Plan (SIP)."
      ]},
      { h: "School-wide literacy events and sustainability", l: [
        "Host termly reading festivals, poetry/storytelling showcases and peer book exhibitions.",
        "Embed SLLC into annual school plans, train incoming student leaders early and hand over clear records."
      ]}
    ],
    practice: [
      { id: "p13", prompt: "Design a simple one-page monthly SLLC tracking summary (attendance/inclusion, key activities, student highlights, challenge, next step) for the school director and PTSA." },
      { id: "p14", prompt: "List three concrete actions to embed SLLC into your school's annual School Improvement Plan (SIP) so it continues after external support ends." }
    ],
    quiz: [
      { q: "Why should SLLC attendance and participation data be disaggregated?", o: ["To publish names publicly","To check equity across gender, grades and inclusion needs and fix gaps early","To penalise absent students","To replace classroom attendance"], a: 1, why: "Disaggregated tracking reveals who is participating and who needs outreach." },
      { q: "What strengthens long-term sustainability of the SLLC?", o: ["Relying on a single temporary visitor","Integrating SLLC into the School Improvement Plan (SIP), training student leaders and engaging PTSA/parents","Keeping all plans secret","Stopping meetings during exams"], a: 1, why: "SIP integration, leadership handover and family/PTSA ownership sustain the club." },
      { q: "How can families support SLLC goals at home?", o: ["By forbidding home conversation","By listening to children read, sharing oral stories/proverbs and encouraging book care","By doing all writing assignments for children","By buying expensive imported software"], a: 1, why: "Oral storytelling, listening to children read and caring for books require little money and high impact." },
      { q: "What is the main purpose of a school-wide literacy showcase?", o: ["To humiliate struggling readers","To celebrate learner progress, motivate peers and demonstrate value to parents and leaders","To replace regular classes for a month","To sell club materials"], a: 1, why: "Showcases build pride, peer motivation and community support." }
    ]
  }
];

const RESOURCES = [
  { title: "SLLC Implementation Manual (Grades 1–8)", kind: "tool", desc: "Core guide on club governance, committee roles, inclusive participation and session routines.", url: "#course" },
  { title: "Five Key Reading Skills Quick Reference", kind: "tool", desc: "Classroom and club reference table for phonemic awareness, phonics, fluency, vocabulary and comprehension.", url: "#course" },
  { title: "Reading Buddy 25-Minute Session Guide", kind: "audio", desc: "Structured pairing, safeguarding and praise-based routine for peer and community volunteers.", url: "#course" },
  { title: "Low-Cost Reading Corner & Book Bank Setup", kind: "video", desc: "Practical ideas for shelves, student-authored texts, level tags and PTSA book banks.", url: "#course" },
  { title: "SLLC Monitoring & SIP Integration Template", kind: "tool", desc: "Simple monthly tracking and School Improvement Plan alignment checklist.", url: "#course" }
];

/* ======= Application State ======= */
const state = {
  route: "home",
  moduleId: 1,
  theme: loadState("theme", "system"),
  profile: loadState("profile", { name: "", school: "", woreda: "", role: "Teacher / Club Focal Person" }),
  doneModules: loadState("doneModules", []),
  quizAnswers: loadState("quizAnswers", {}),
  practiceAnswers: loadState("practiceAnswers", {}),
  exam: loadState("exam", null)
};

function persistAll() {
  saveState("theme", state.theme);
  saveState("profile", state.profile);
  saveState("doneModules", state.doneModules);
  saveState("quizAnswers", state.quizAnswers);
  saveState("practiceAnswers", state.practiceAnswers);
  saveState("exam", state.exam);
}

/* ======= Theme Handling ======= */
function applyTheme() {
  const root = document.documentElement;
  const btn = document.getElementById("theme-toggle");
  if (state.theme === "dark" || state.theme === "light") {
    root.setAttribute("data-theme", state.theme);
  } else {
    root.removeAttribute("data-theme");
  }
  const isDark = state.theme === "dark" || (state.theme === "system" && window.matchMedia("(prefers-color-scheme: dark)").matches);
  if (btn) {
    btn.textContent = isDark ? "☀" : "☾";
    btn.setAttribute("aria-pressed", String(isDark));
    btn.setAttribute("aria-label", isDark ? "Switch to light colour theme" : "Switch to dark colour theme");
  }
}

document.getElementById("theme-toggle").addEventListener("click", () => {
  const isDark = document.documentElement.getAttribute("data-theme") === "dark" ||
    (!document.documentElement.getAttribute("data-theme") && window.matchMedia("(prefers-color-scheme: dark)").matches);
  state.theme = isDark ? "light" : "dark";
  persistAll();
  applyTheme();
});

/* ======= Navigation & Footer ======= */
const ROUTES = [
  { id: "home", label: "Overview" },
  { id: "course", label: "Modules" },
  { id: "exam", label: "Final Exam" },
  { id: "certificate", label: "Certificate" },
  { id: "resources", label: "Resources" },
  { id: "instructor", label: "Verify" }
];

function renderNav() {
  const nav = document.getElementById("nav");
  nav.innerHTML = ROUTES.map(r =>
    `<a href="#${r.id}" ${state.route === r.id ? 'aria-current="page"' : ""}>${r.label}</a>`
  ).join("");
  const foot = document.getElementById("foot");
  foot.innerHTML = `<div class="row" style="justify-content:space-between">
    <div><strong>${esc(CFG.org)}</strong> — ${esc(CFG.course)}</div>
    <div>Contact: <a href="mailto:${esc(CFG.ownerEmail)}">${esc(CFG.ownerEmail)}</a></div>
  </div>`;
}

function esc(s) {
  return String(s ?? "").replace(/[&<>"']/g, c => ({ "&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;" }[c]));
}

function getAllPracticeTasks() {
  const list = [];
  MODULES.forEach(m => {
    (m.practice || []).forEach(p => list.push({ ...p, moduleId: m.id, moduleTitle: m.title }));
  });
  return list;
}

function getCompletedPracticeCount() {
  const tasks = getAllPracticeTasks();
  return tasks.filter(t => (state.practiceAnswers[t.id] || "").trim().length >= CFG.practiceMinChars).length;
}

function isEligibleForCertificate() {
  const allModulesDone = state.doneModules.length >= MODULES.length;
  const practiceOk = getCompletedPracticeCount() >= CFG.practiceMin;
  const examOk = state.exam && state.exam.passed === true;
  return { allModulesDone, practiceOk, examOk, eligible: allModulesDone && practiceOk && examOk };
}

/* ======= Visual Helpers ======= */
function renderVisual(vis) {
  if (!vis) return "";
  if (vis.type === "flow") {
    return `<div class="vis">
      <div class="cap">${esc(vis.cap)}</div>
      <ol class="flow">${vis.items.map((it, idx) => `<li><b>${idx + 1}</b>${esc(it)}</li>`).join("")}</ol>
    </div>`;
  }
  if (vis.type === "hub") {
    return `<div class="vis">
      <div class="cap">${esc(vis.cap)}</div>
      <div class="hub">
        <div class="c">${esc(vis.center)}</div>
        ${vis.items.map(it => `<div class="i">${esc(it)}</div>`).join("")}
      </div>
    </div>`;
  }
  return "";
}

/* ======= Views ======= */
function viewHome() {
  const pct = Math.round((state.doneModules.length / MODULES.length) * 100);
  const pracCount = getCompletedPracticeCount();
  const totalPrac = getAllPracticeTasks().length;
  const elig = isEligibleForCertificate();

  return `<section class="hero">
    <span class="pill ok">${esc(CFG.org)}</span>
    <h1>${esc(CFG.course)}</h1>
    <p class="lead">${esc(CFG.sub)}</p>
    <div class="row">
      <a class="btn primary" href="#course">Start / Continue Modules</a>
      <a class="btn" href="#exam">Take Final Exam</a>
      <a class="btn" href="#certificate">Certificate &amp; Progress</a>
    </div>
  </section>

  <ol class="steps">
    <li><b>Complete 8 Modules</b>Work through core literacy concepts, club governance, inclusion, Reading Buddies, TaRL links and sustainability, passing each module quiz (${CFG.passModule}/4).</li>
    <li><b>Submit Practice Tasks</b>Complete at least ${CFG.practiceMin} of ${totalPrac} school-grounded reflection tasks (${CFG.practiceMinChars}+ characters each).</li>
    <li><b>Pass Final Exam &amp; Certify</b>Score at least ${CFG.passPct}% on the ${CFG.examSize}-question exam to generate your verifiable certificate.</li>
  </ol>

  <div class="grid2">
    <div class="card stack">
      <h2>Your Course Readiness</h2>
      <div class="stat">
        <div><b>${state.doneModules.length}/${MODULES.length}</b><span class="hint">Modules completed</span></div>
        <div><b>${pracCount}/${totalPrac}</b><span class="hint">Practice tasks ready</span></div>
        <div><b>${state.exam ? state.exam.pct + "%" : "—"}</b><span class="hint">Final exam score</span></div>
      </div>
      <div class="progress" aria-label="Module progress"><i style="width:${pct}%"></i></div>
      <div>${elig.eligible
        ? '<span class="pill ok">Eligible for Certificate</span>'
        : '<span class="pill sunp">In Progress — complete modules, practice &amp; exam</span>'}</div>
    </div>

    <div class="card stack">
      <h2>Learner Profile</h2>
      <p class="hint">Saved locally on your device for your certificate header.</p>
      <div class="field">
        <label for="prof-name">Full Name</label>
        <input id="prof-name" type="text" value="${esc(state.profile.name)}" placeholder="e.g., Alemayehu Bekele">
      </div>
      <div class="field">
        <label for="prof-school">School &amp; Woreda / Zone</label>
        <input id="prof-school" type="text" value="${esc(state.profile.school)}" placeholder="e.g., Babile Primary School, East Hararghe">
      </div>
      <div class="field">
        <label for="prof-role">Role</label>
        <select id="prof-role">
          ${["Teacher / Club Focal Person","School Director / Vice Director","Cluster / Woreda Supervisor","Community / Volunteer Coordinator","NGO Education Officer"].map(r =>
            `<option value="${esc(r)}" ${state.profile.role === r ? "selected" : ""}>${esc(r)}</option>`
          ).join("")}
        </select>
      </div>
      <div class="row">
        <button type="button" class="primary" id="save-profile">Save Profile</button>
        <span id="prof-saved" class="hint" aria-live="polite"></span>
      </div>
    </div>
  </div>`;
}

function viewCourse() {
  const mod = MODULES.find(m => m.id === state.moduleId) || MODULES[0];
  state.moduleId = mod.id;
  const isDone = state.doneModules.includes(mod.id);
  const savedQuiz = state.quizAnswers[mod.id] || {};

  const railItems = MODULES.map(m => {
    const done = state.doneModules.includes(m.id);
    const current = m.id === mod.id;
    return `<button type="button" data-mod="${m.id}" class="${done ? "done" : ""}" aria-current="${current ? "true" : "false"}">
      <span class="n">${done ? "✓" : m.id}</span>
      <span>${esc(m.title)}</span>
    </button>`;
  }).join("");

  const sectionsHtml = mod.sections.map(sec => {
    let body = "";
    if (sec.p) body += `<p>${esc(sec.p)}</p>`;
    if (sec.l) body += `<ul>${sec.l.map(li => `<li>${esc(li)}</li>`).join("")}</ul>`;
    if (sec.table) {
      body += `<div class="tablewrap"><table><thead><tr>${sec.table.head.map(h => `<th>${esc(h)}</th>`).join("")}</tr></thead><tbody>
        ${sec.table.rows.map(row => `<tr>${row.map(cell => `<td>${esc(cell)}</td>`).join("")}</tr>`).join("")}
      </tbody></table></div>`;
    }
    return `<section><h3>${esc(sec.h)}</h3>${body}</section>`;
  }).join("");

  const practiceHtml = (mod.practice || []).map((p, idx) => {
    const val = state.practiceAnswers[p.id] || "";
    const len = val.trim().length;
    const ok = len >= CFG.practiceMinChars;
    return `<div class="prac">
      <div class="row" style="justify-content:space-between">
        <span class="pill sunp">Practice Task ${idx + 1} (Module ${mod.id})</span>
        <span class="pill ${ok ? "ok" : ""}">${len}/${CFG.practiceMinChars} min chars ${ok ? "✓" : ""}</span>
      </div>
      <p><strong>${esc(p.prompt)}</strong></p>
      <textarea data-prac="${esc(p.id)}" aria-label="Practice response for task ${idx + 1}" placeholder="Write your practical school response here (at least ${CFG.practiceMinChars} characters)...">${esc(val)}</textarea>
    </div>`;
  }).join("");

  const quizHtml = mod.quiz.map((q, qi) => {
    const chosen = savedQuiz[qi];
    return `<fieldset class="q">
      <legend>Question ${qi + 1}: ${esc(q.q)}</legend>
      ${q.o.map((opt, oi) => {
        let cls = "opt";
        if (typeof chosen === "number") {
          if (oi === q.a) cls += " right";
          else if (oi === chosen && chosen !== q.a) cls += " wrong";
        }
        return `<label class="${cls}">
          <input type="radio" name="q_${qi}" value="${oi}" ${chosen === oi ? "checked" : ""}>
          <span>${esc(opt)}</span>
        </label>`;
      }).join("")}
      ${typeof chosen === "number" ? `<p class="why"><strong>Explanation:</strong> ${esc(q.why)}</p>` : ""}
    </fieldset>`;
  }).join("");

  return `<div class="course">
    <details class="menu">
      <summary>Module ${mod.id} of ${MODULES.length}: ${esc(mod.title)}</summary>
      <div class="rail">${railItems}</div>
    </details>
    <aside class="rail" aria-label="Course modules">${railItems}</aside>

    <article class="lesson">
      <div class="card stack">
        <div class="row" style="justify-content:space-between">
          <span class="pill">Module ${mod.id} of ${MODULES.length} • ~${mod.mins} min</span>
          ${isDone ? '<span class="pill ok">Completed ✓</span>' : '<span class="pill">In Progress</span>'}
        </div>
        <h2>${esc(mod.title)}</h2>
        <p>${esc(mod.intro)}</p>
        ${renderVisual(mod.visual)}
      </div>

      <div class="card stack">${sectionsHtml}</div>

      <div class="stack">
        <h3>School-Based Practice Tasks</h3>
        ${practiceHtml}
      </div>

      <div class="card stack">
        <div class="row" style="justify-content:space-between">
          <h3>Module Check (Pass: ${CFG.passModule}/${mod.quiz.length})</h3>
          <button type="button" class="primary" id="grade-mod">Check Answers</button>
        </div>
        <div id="mod-quiz-wrap" class="stack">${quizHtml}</div>
        <div id="mod-quiz-msg"></div>
      </div>

      <div class="row" style="justify-content:space-between">
        <button type="button" id="prev-mod" ${mod.id <= 1 ? "disabled" : ""}>← Previous Module</button>
        ${mod.id < MODULES.length
          ? `<button type="button" class="primary" id="next-mod">Next Module →</button>`
          : `<a class="btn primary" href="#exam">Proceed to Final Exam →</a>`}
      </div>
    </article>
  </div>`;
}

function buildExamQuestions() {
  const pool = [];
  MODULES.forEach(m => {
    m.quiz.forEach((q, qi) => {
      pool.push({ id: `m${m.id}_q${qi}`, moduleTitle: m.title, ...q });
    });
  });
  return pool.slice(0, CFG.examSize);
}

function viewExam() {
  const questions = buildExamQuestions();
  const prev = state.exam;

  return `<div class="stack" style="padding-top:24px">
    <div class="card stack">
      <div class="row" style="justify-content:space-between">
        <span class="pill ok">${esc(CFG.course)}</span>
        <span class="pill">Pass threshold: ${CFG.passPct}% (${Math.ceil((CFG.examSize * CFG.passPct) / 100)}/${CFG.examSize})</span>
      </div>
      <h2>Final Implementation Exam</h2>
      <p class="hint">Answer all ${questions.length} questions below and submit to record your score for certification.</p>
      ${prev ? `<div class="msg ${prev.passed ? "good" : "bad"}">
        Last attempt: ${prev.score}/${prev.total} (${prev.pct}%) — ${prev.passed ? "Passed ✓" : "Not yet passed"}
      </div>` : ""}
    </div>

    <form id="exam-form" class="stack">
      ${questions.map((q, idx) => `<fieldset class="q">
        <legend>${idx + 1}. ${esc(q.q)} <span class="hint">(${esc(q.moduleTitle)})</span></legend>
        ${q.o.map((opt, oi) => `<label class="opt">
          <input type="radio" name="${q.id}" value="${oi}" required>
          <span>${esc(opt)}</span>
        </label>`).join("")}
      </fieldset>`).join("")}
      <div class="row">
        <button type="submit" class="primary">Submit Final Exam</button>
      </div>
      <div id="exam-result"></div>
    </form>
  </div>`;
}

function viewCertificate() {
  const elig = isEligibleForCertificate();
  const pracCount = getCompletedPracticeCount();
  const totalPrac = getAllPracticeTasks().length;
  const learnerName = state.profile.name.trim() || "SLLC Course Participant";
  const schoolName = state.profile.school.trim() || "Ethiopian Primary School (Grades 1–8)";
  const dateStr = state.exam?.date || new Date().toISOString().slice(0, 10);
  const examPct = state.exam ? `${state.exam.pct}%` : "Pending";
  const certCode = sha256(`${learnerName}|${schoolName}|${dateStr}|${examPct}|${CFG.salt}`).slice(0, 16).toUpperCase();

  return `<div class="stack" style="padding-top:24px">
    <div class="card stack">
      <h2>Certificate of Completion</h2>
      <div class="row">
        <span class="pill ${elig.allModulesDone ? "ok" : ""}">Modules: ${state.doneModules.length}/${MODULES.length}</span>
        <span class="pill ${elig.practiceOk ? "ok" : ""}">Practice: ${pracCount}/${totalPrac} (min ${CFG.practiceMin})</span>
        <span class="pill ${elig.examOk ? "ok" : ""}">Exam: ${state.exam ? state.exam.pct + "%" : "Not taken"} (min ${CFG.passPct}%)</span>
      </div>
      ${!elig.eligible ? `<div class="msg info">
        Complete all ${MODULES.length} modules, submit at least ${CFG.practiceMin} practice responses (${CFG.practiceMinChars}+ chars), and pass the final exam (${CFG.passPct}%+) to unlock full certification status. Preview is shown below.
      </div>` : `<div class="msg good">Congratulations — all certification requirements are met.</div>`}
      <div class="copyrow no-print">
        <button type="button" class="primary" onclick="window.print()">Print / Save PDF</button>
        <button type="button" id="copy-code">Copy Verification ID</button>
        <span class="copybox" id="cert-code-box">${certCode}</span>
      </div>
    </div>

    <div class="cert" role="img" aria-label="Certificate of Completion for ${esc(learnerName)}">
      <svg viewBox="0 0 1000 660" xmlns="http://www.w3.org/2000/svg">
        <rect x="18" y="18" width="964" height="624" rx="14" fill="#fffdf5" stroke="#0d6b50" stroke-width="6"/>
        <rect x="34" y="34" width="932" height="592" rx="8" fill="none" stroke="#f0b323" stroke-width="3"/>
        <text x="500" y="102" text-anchor="middle" font-family="sans-serif" font-size="18" font-weight="700" fill="#53635b" letter-spacing="3">${esc(CFG.org.toUpperCase())}</text>
        <text x="500" y="162" text-anchor="middle" font-family="serif" font-size="42" font-weight="bold" fill="#0d6b50">Certificate of Completion</text>
        <text x="500" y="212" text-anchor="middle" font-family="sans-serif" font-size="18" fill="#53635b">This certifies that</text>
        <text x="500" y="276" text-anchor="middle" font-family="serif" font-size="36" font-weight="bold" fill="#14201b">${esc(learnerName)}</text>
        <line x1="220" y1="294" x2="780" y2="294" stroke="#d3ddd6" stroke-width="2"/>
        <text x="500" y="330" text-anchor="middle" font-family="sans-serif" font-size="18" fill="#14201b">${esc(schoolName)}</text>
        <text x="500" y="382" text-anchor="middle" font-family="sans-serif" font-size="17" fill="#53635b">has completed the</text>
        <text x="500" y="422" text-anchor="middle" font-family="sans-serif" font-size="24" font-weight="bold" fill="#14201b">${esc(CFG.course)}</text>
        <text x="500" y="454" text-anchor="middle" font-family="sans-serif" font-size="16" fill="#53635b">${esc(CFG.sub)}</text>
        <text x="260" y="535" text-anchor="middle" font-family="sans-serif" font-size="15" fill="#14201b">Date: ${esc(dateStr)}</text>
        <text x="500" y="535" text-anchor="middle" font-family="sans-serif" font-size="15" fill="#14201b">Exam Score: ${esc(examPct)}</text>
        <text x="740" y="535" text-anchor="middle" font-family="sans-serif" font-size="15" fill="#14201b">Practice: ${pracCount}/${totalPrac}</text>
        <text x="500" y="588" text-anchor="middle" font-family="monospace" font-size="14" fill="#53635b">Verification ID: ${certCode}</text>
      </svg>
    </div>
  </div>`;
}

function viewResources() {
  return `<div class="stack" style="padding-top:24px">
    <div class="card stack">
      <h2>Implementation Resources &amp; Toolkits</h2>
      <p class="hint">Practical guides and templates supporting School-Based Literacy and Language Clubs in Ethiopian primary schools.</p>
    </div>
    <ul class="res">
      ${RESOURCES.map(r => `<li>
        <a href="${esc(r.url)}">
          <span class="k ${esc(r.kind)}">${esc(r.kind)}</span>
          <b>${esc(r.title)}</b>
          <span class="d">${esc(r.desc)}</span>
        </a>
      </li>`).join("")}
    </ul>
  </div>`;
}

function viewInstructor() {
  return `<div class="stack" style="padding-top:24px">
    <div class="card stack">
      <h2>Certificate &amp; Instructor Verification</h2>
      <p class="hint">Verify a learner's completion hash or check instructor passcode access.</p>
      <div class="grid2">
        <div class="stack">
          <h3>Verify Learner Certificate Hash</h3>
          <div class="field">
            <label for="v-name">Learner Full Name</label>
            <input id="v-name" type="text" placeholder="Full Name">
          </div>
          <div class="field">
            <label for="v-school">School &amp; Woreda / Zone</label>
            <input id="v-school" type="text" placeholder="School &amp; Woreda">
          </div>
          <div class="field">
            <label for="v-date">Date (YYYY-MM-DD)</label>
            <input id="v-date" type="text" placeholder="2026-11-14">
          </div>
          <div class="field">
            <label for="v-pct">Exam Score (e.g., 83%)</label>
            <input id="v-pct" type="text" placeholder="83%">
          </div>
          <div class="field">
            <label for="v-hash">Certificate Verification ID</label>
            <input id="v-hash" type="text" placeholder="16-character hex ID">
          </div>
          <button type="button" class="primary" id="run-verify">Verify Certificate</button>
          <div id="verify-out"></div>
        </div>

        <div class="stack">
          <h3>Instructor Passcode Check</h3>
          <p class="hint">Confirm instructor credentials configured in <code>CFG.instructorHash</code>.</p>
          <div class="field">
            <label for="inst-pass">Instructor Passcode</label>
            <input id="inst-pass" type="password" autocomplete="off">
          </div>
          <button type="button" id="check-inst">Validate Passcode</button>
          <div id="inst-out"></div>
        </div>
      </div>
    </div>
  </div>`;
}

/* ======= Main Render & Event Delegation ======= */
function renderApp() {
  renderNav();
  applyTheme();
  const app = document.getElementById("app");
  if (state.route === "course") app.innerHTML = viewCourse();
  else if (state.route === "exam") app.innerHTML = viewExam();
  else if (state.route === "certificate") app.innerHTML = viewCertificate();
  else if (state.route === "resources") app.innerHTML = viewResources();
  else if (state.route === "instructor") app.innerHTML = viewInstructor();
  else app.innerHTML = viewHome();
}

document.getElementById("app").addEventListener("click", (e) => {
  const modBtn = e.target.closest("[data-mod]");
  if (modBtn) {
    state.moduleId = Number(modBtn.dataset.mod);
    renderApp();
    return;
  }
  if (e.target.id === "prev-mod" && state.moduleId > 1) {
    state.moduleId -= 1;
    renderApp();
    return;
  }
  if (e.target.id === "next-mod" && state.moduleId < MODULES.length) {
    state.moduleId += 1;
    renderApp();
    return;
  }
  if (e.target.id === "save-profile") {
    state.profile = {
      name: document.getElementById("prof-name").value,
      school: document.getElementById("prof-school").value,
      role: document.getElementById("prof-role").value
    };
    persistAll();
    document.getElementById("prof-saved").textContent = "Saved ✓";
    return;
  }
  if (e.target.id === "grade-mod") {
    const mod = MODULES.find(m => m.id === state.moduleId);
    const answers = {};
    let correct = 0;
    mod.quiz.forEach((q, qi) => {
      const checked = document.querySelector(`input[name="q_${qi}"]:checked`);
      if (checked) {
        const val = Number(checked.value);
        answers[qi] = val;
        if (val === q.a) correct += 1;
      }
    });
    state.quizAnswers[mod.id] = answers;
    const passed = correct >= CFG.passModule;
    if (passed && !state.doneModules.includes(mod.id)) {
      state.doneModules.push(mod.id);
      state.doneModules.sort((a, b) => a - b);
    }
    persistAll();
    renderApp();
    const msgBox = document.getElementById("mod-quiz-msg");
    if (msgBox) {
      msgBox.innerHTML = `<div class="msg ${passed ? "good" : "bad"}">
        Score: ${correct}/${mod.quiz.length} — ${passed ? "Module completed! ✓" : `Need at least ${CFG.passModule}/${mod.quiz.length} to complete. Review explanations above and try again.`}
      </div>`;
    }
    return;
  }
  if (e.target.id === "copy-code") {
    const code = document.getElementById("cert-code-box")?.textContent?.trim() || "";
    if (navigator.clipboard && navigator.clipboard.writeText) {
      navigator.clipboard.writeText(code).catch(() => {});
    }
    e.target.textContent = "Copied ✓";
    return;
  }
  if (e.target.id === "run-verify") {
    const name = document.getElementById("v-name").value.trim();
    const school = document.getElementById("v-school").value.trim();
    const date = document.getElementById("v-date").value.trim();
    const pct = document.getElementById("v-pct").value.trim();
    const hash = document.getElementById("v-hash").value.trim().toUpperCase();
    const expected = sha256(`${name}|${school}|${date}|${pct}|${CFG.salt}`).slice(0, 16).toUpperCase();
    const match = Boolean(hash) && hash === expected;
    document.getElementById("verify-out").innerHTML = `<div class="msg ${match ? "good" : "bad"}">
      ${match ? "Valid certificate verification ID ✓" : "Verification ID does not match these fields."}
    </div>`;
    return;
  }
  if (e.target.id === "check-inst") {
    const pass = document.getElementById("inst-pass").value;
    const ok = sha256(pass) === CFG.instructorHash;
    document.getElementById("inst-out").innerHTML = `<div class="msg ${ok ? "good" : "bad"}">
      ${ok ? "Instructor passcode verified ✓" : "Passcode does not match configured hash."}
    </div>`;
  }
});

document.getElementById("app").addEventListener("input", (e) => {
  const pracId = e.target.dataset?.prac;
  if (pracId) {
    state.practiceAnswers[pracId] = e.target.value;
    persistAll();
  }
});

document.getElementById("app").addEventListener("submit", (e) => {
  if (e.target.id !== "exam-form") return;
  e.preventDefault();
  const questions = buildExamQuestions();
  let score = 0;
  questions.forEach(q => {
    const chosen = document.querySelector(`input[name="${q.id}"]:checked`);
    if (chosen && Number(chosen.value) === q.a) score += 1;
  });
  const pct = Math.round((score / questions.length) * 100);
  const passed = pct >= CFG.passPct;
  state.exam = { score, total: questions.length, pct, passed, date: new Date().toISOString().slice(0, 10) };
  persistAll();
  const out = document.getElementById("exam-result");
  out.innerHTML = `<div class="msg ${passed ? "good" : "bad"}">
    Exam Result: ${score}/${questions.length} (${pct}%) — ${passed ? 'Passed! Visit <a href="#certificate">Certificate</a> to view and print.' : `Need ${CFG.passPct}% to pass. Review modules and retry.`}
  </div>`;
});

function syncRouteFromHash() {
  const raw = (location.hash || "#home").replace(/^#/, "");
  state.route = ROUTES.some(r => r.id === raw) ? raw : "home";
  renderApp();
}

window.addEventListener("hashchange", syncRouteFromHash);
syncRouteFromHash();
</script>
</body>
</html>
