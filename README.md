
<style>
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@700;800&family=Plus+Jakarta+Sans:ital,wght@0,400;0,500;0,600;1,400&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
.pg{font-family:'Plus Jakarta Sans',sans-serif;background:#fff;color:#1a1a2e}

.hero{background:#f0f4ff;padding:44px 24px 36px;text-align:center;position:relative;overflow:hidden;border-bottom:3px solid #e8edff}
.confetti-dot{position:absolute;border-radius:50%;animation:float-up var(--d,4s) ease-in-out infinite var(--dl,0s);opacity:0.6}
@keyframes float-up{0%,100%{transform:translateY(0) rotate(0deg);opacity:0.6}50%{transform:translateY(-20px) rotate(180deg);opacity:1}}
.hero-tag{display:inline-block;background:#6c63ff;color:#fff;font-size:11px;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;padding:5px 16px;border-radius:20px;margin-bottom:18px}
.hero-name{font-family:'Syne',sans-serif;font-size:46px;font-weight:800;color:#1a1a2e;line-height:1.05;margin-bottom:8px}
.hero-name span{color:#6c63ff}
.typed-row{height:34px;display:flex;align-items:center;justify-content:center;margin-bottom:20px}
#typed{font-family:'Syne',sans-serif;font-size:17px;font-weight:700;color:#ff6b6b}
#cur{display:inline-block;width:2px;height:18px;background:#ff6b6b;margin-left:2px;vertical-align:middle;animation:blink 0.7s step-end infinite}
@keyframes blink{0%,100%{opacity:1}50%{opacity:0}}
.hero-pills{display:flex;justify-content:center;gap:8px;flex-wrap:wrap;margin-bottom:22px}
.hpill{padding:6px 16px;border-radius:20px;font-size:12px;font-weight:700;border:2px solid}
.hp-pink{background:#fff0f3;border-color:#ff6b6b;color:#c0392b}
.hp-violet{background:#f0edff;border-color:#6c63ff;color:#4a3fa8}
.hp-mint{background:#e8fff4;border-color:#00d68f;color:#00875a}
.cta-row{display:flex;justify-content:center;gap:10px;flex-wrap:wrap}
.cta{padding:10px 22px;border-radius:10px;font-size:13px;font-weight:700;border:2px solid;cursor:pointer;transition:all 0.18s;text-decoration:none;display:inline-block}
.cta-li{background:#6c63ff;border-color:#6c63ff;color:#fff}
.cta-li:hover{background:#5a51e0;border-color:#5a51e0}
.cta-em{background:#fff;border-color:#ff6b6b;color:#ff6b6b}
.cta-em:hover{background:#ff6b6b;color:#fff}

.bio-section{padding:32px 24px 24px;text-align:center;background:#fff}
.sec-title{font-family:'Syne',sans-serif;font-size:26px;font-weight:800;color:#1a1a2e;margin-bottom:12px}
.sec-title span{color:#6c63ff}
.bio-text{font-size:14px;color:#555;line-height:1.9;max-width:580px;margin:0 auto 18px}
.stat-row{display:flex;justify-content:center;gap:12px;flex-wrap:wrap;margin-top:6px}
.stat-bubble{background:#f0edff;border:2px solid #d0c8ff;border-radius:16px;padding:14px 22px;text-align:center;min-width:110px}
.stat-num{font-family:'Syne',sans-serif;font-size:26px;font-weight:800;color:#6c63ff}
.stat-lbl{font-size:11px;color:#888;font-weight:600;margin-top:2px;text-transform:uppercase;letter-spacing:0.5px}

.charts-section{padding:24px 20px 28px;background:#fafbff}
.chart-row{display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-top:16px}
.chart-box{background:#fff;border:2px solid #e8edff;border-radius:14px;padding:16px}
.chart-label{font-size:12px;font-weight:700;color:#1a1a2e;margin-bottom:12px;display:flex;align-items:center;gap:6px}
.chart-label .dot{width:10px;height:10px;border-radius:50%;flex-shrink:0}
.cl-v{background:#6c63ff}.cl-p{background:#ff6b6b}.cl-g{background:#00d68f}.cl-o{background:#ffb347}

.skill-bar-wrap{display:flex;align-items:center;gap:8px;margin-bottom:8px}
.skill-name{font-size:11px;color:#555;font-weight:600;width:80px;flex-shrink:0}
.skill-track{flex:1;height:10px;background:#f0edff;border-radius:8px;overflow:hidden}
.skill-fill{height:100%;border-radius:8px;animation:grow 1.2s ease both}
@keyframes grow{from{width:0}to{width:var(--w)}}
.sf-v{background:#6c63ff}.sf-p{background:#ff6b6b}.sf-g{background:#00d68f}.sf-o{background:#ffb347}.sf-b{background:#00b4d8}
.skill-pct{font-size:10px;font-weight:700;color:#888;width:30px;text-align:right;flex-shrink:0}

.lang-ring-wrap{display:flex;align-items:center;gap:16px}
.lang-legend{flex:1}
.lang-item{display:flex;align-items:center;gap:6px;margin-bottom:7px}
.lang-dot{width:10px;height:10px;border-radius:2px;flex-shrink:0}
.lang-name{font-size:11px;color:#555;font-weight:600;flex:1}
.lang-pct{font-size:11px;font-weight:700}

.proj-section{padding:4px 20px 28px;background:#fff}
.proj-card{background:#fff;border:2px solid #e8edff;border-radius:16px;padding:20px;margin-bottom:14px;position:relative;overflow:hidden;transition:border-color 0.2s,transform 0.2s}
.proj-card:hover{border-color:#b8b0ff;transform:translateY(-2px)}
.proj-accent{position:absolute;left:0;top:0;bottom:0;width:5px;border-radius:16px 0 0 16px}
.pa-v{background:#6c63ff}.pa-p{background:#ff6b6b}.pa-g{background:#00d68f}.pa-o{background:#ffb347}
.proj-inner{padding-left:14px}
.proj-emoji{font-size:26px;margin-bottom:8px;display:block}
.proj-name{font-family:'Syne',sans-serif;font-size:16px;font-weight:800;color:#1a1a2e;margin-bottom:3px}
.proj-sub{font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;margin-bottom:10px}
.ps-v{color:#6c63ff}.ps-p{color:#ff6b6b}.ps-g{color:#00875a}.ps-o{color:#e67e22}
.proj-desc{font-size:13px;color:#555;line-height:1.75;margin-bottom:12px}
.proj-desc strong{color:#1a1a2e;font-weight:700}
.proj-meta{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:8px}
.proj-tags{display:flex;flex-wrap:wrap;gap:5px}
.ptag{font-size:10px;font-weight:700;padding:3px 9px;border-radius:6px;border:1.5px solid}
.t-v{color:#4a3fa8;background:#f0edff;border-color:#c8c0ff}
.t-p{color:#c0392b;background:#fff0f3;border-color:#ffc0c7}
.t-g{color:#00875a;background:#e8fff4;border-color:#b0f0d0}
.t-o{color:#c27a00;background:#fff8e0;border-color:#ffe080}
.t-b{color:#006b8a;background:#e0f7ff;border-color:#a0e0f8}
.proj-link{font-size:11px;font-weight:700;color:#6c63ff;border:1.5px solid #c8c0ff;background:#f0edff;padding:5px 14px;border-radius:8px;cursor:pointer;transition:all 0.18s}
.proj-link:hover{background:#6c63ff;color:#fff;border-color:#6c63ff}

.stack-section{padding:4px 20px 28px;background:#fafbff}
.stack-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:10px;margin-top:14px}
.stack-card{background:#fff;border:2px solid #e8edff;border-radius:12px;padding:14px}
.stack-icon{font-size:20px;margin-bottom:6px}
.stack-title{font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:#888;margin-bottom:8px}
.stack-list{display:flex;flex-direction:column;gap:4px}
.stack-item{font-size:12px;font-weight:600;color:#333;display:flex;align-items:center;gap:5px}
.stack-item::before{content:'';width:6px;height:6px;border-radius:50%;flex-shrink:0}
.si-v::before{background:#6c63ff}
.si-p::before{background:#ff6b6b}
.si-g::before{background:#00d68f}
.si-o::before{background:#ffb347}
.si-b::before{background:#00b4d8}

.connect-section{padding:20px 24px 28px;background:#f0edff;text-align:center}
.connect-row{display:flex;justify-content:center;gap:12px;flex-wrap:wrap;margin-top:16px}
.cc{background:#fff;border:2px solid #d0c8ff;border-radius:14px;padding:16px 20px;min-width:140px;text-align:center;transition:all 0.18s}
.cc:hover{border-color:#6c63ff;transform:translateY(-2px)}
.cc-icon{font-size:22px;margin-bottom:6px}
.cc-label{font-size:10px;font-weight:700;letter-spacing:0.8px;text-transform:uppercase;color:#888;margin-bottom:3px}
.cc-val{font-size:11px;font-weight:600;color:#6c63ff}

.footer{text-align:center;padding:22px 20px 30px;background:#1a1a2e;color:#fff}
.footer-q{font-family:'Syne',sans-serif;font-size:20px;font-weight:800;background:linear-gradient(90deg,#ff6b6b,#6c63ff,#00d68f,#ffb347,#ff6b6b);background-size:200%;-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;animation:shift 4s linear infinite}
@keyframes shift{0%{background-position:0}100%{background-position:200%}}
.footer-sub{font-size:12px;color:#555;margin-top:6px}
</style>

<div class="pg">

<!-- HERO -->
<div class="hero">
  <div id="confetti"></div>
  <div style="position:relative;z-index:1">
    <div class="hero-tag">// open to collabs</div>
    <div class="hero-name">Aahona <span>Mukhopadhyay</span></div>
    <div class="typed-row"><span id="typed"></span><span id="cur"></span></div>
    <div class="hero-pills">
      <span class="hpill hp-pink">🚀 AI Builder</span>
      <span class="hpill hp-violet">🧠 Full Stack Dev</span>
      <span class="hpill hp-mint">🇮🇳 India</span>
    </div>
    <div class="cta-row">
      <a href="https://www.linkedin.com/in/aahona-mukhopadhyay-451075293/" class="cta cta-li">💼 LinkedIn</a>
      <a href="mailto:aahona1609@gmail.com" class="cta cta-em">✉️ Email me</a>
    </div>
  </div>
</div>

<!-- BIO + STATS -->
<div class="bio-section">
  <div class="sec-title">Hey, I'm <span>Aahona</span> ✨</div>
  <p class="bio-text">I build things that actually solve problems — not just look good in a portfolio. Right now I'm deep into AI systems, full-stack apps, and making tech work for real people. I believe in shipping fast, learning in public, and never building brainrot.</p>
  <div class="stat-row">
    <div class="stat-bubble"><div class="stat-num">4+</div><div class="stat-lbl">Projects</div></div>
    <div class="stat-bubble"><div class="stat-num">4</div><div class="stat-lbl">Languages</div></div>
    <div class="stat-bubble"><div class="stat-num">10+</div><div class="stat-lbl">Repos</div></div>
    <div class="stat-bubble" style="background:#fff0f3;border-color:#ffc0c7"><div class="stat-num" style="color:#ff6b6b">∞</div><div class="stat-lbl">Learning</div></div>
  </div>
</div>

<!-- CHARTS -->
<div class="charts-section">
  <div style="text-align:center"><div class="sec-title">📊 By the <span>Numbers</span></div></div>
  <div class="chart-row">

    <!-- Skill bars -->
    <div class="chart-box">
      <div class="chart-label"><span class="dot cl-v"></span>Tech skill levels</div>
      <div class="skill-bar-wrap"><span class="skill-name">React / JS</span><div class="skill-track"><div class="skill-fill sf-v" style="--w:88%"></div></div><span class="skill-pct">88%</span></div>
      <div class="skill-bar-wrap"><span class="skill-name">Python / AI</span><div class="skill-track"><div class="skill-fill sf-p" style="--w:82%;animation-delay:0.1s"></div></div><span class="skill-pct">82%</span></div>
      <div class="skill-bar-wrap"><span class="skill-name">Node.js</span><div class="skill-track"><div class="skill-fill sf-g" style="--w:78%;animation-delay:0.2s"></div></div><span class="skill-pct">78%</span></div>
      <div class="skill-bar-wrap"><span class="skill-name">C++</span><div class="skill-track"><div class="skill-fill sf-o" style="--w:70%;animation-delay:0.3s"></div></div><span class="skill-pct">70%</span></div>
      <div class="skill-bar-wrap"><span class="skill-name">Java</span><div class="skill-track"><div class="skill-fill sf-b" style="--w:65%;animation-delay:0.4s"></div></div><span class="skill-pct">65%</span></div>
    </div>

    <!-- Language donut via canvas -->
    <div class="chart-box">
      <div class="chart-label"><span class="dot cl-p"></span>Languages across repos</div>
      <div style="display:flex;align-items:center;gap:14px">
        <div style="position:relative;width:110px;height:110px;flex-shrink:0">
          <canvas id="donut" role="img" aria-label="Language distribution: JavaScript 35%, Python 28%, C++ 20%, Java 17%">JS 35%, Python 28%, C++ 20%, Java 17%</canvas>
        </div>
        <div class="lang-legend">
          <div class="lang-item"><div class="lang-dot" style="background:#6c63ff"></div><span class="lang-name">JavaScript</span><span class="lang-pct" style="color:#6c63ff">35%</span></div>
          <div class="lang-item"><div class="lang-dot" style="background:#ff6b6b"></div><span class="lang-name">Python</span><span class="lang-pct" style="color:#ff6b6b">28%</span></div>
          <div class="lang-item"><div class="lang-dot" style="background:#00d68f"></div><span class="lang-name">C++</span><span class="lang-pct" style="color:#00d68f">20%</span></div>
          <div class="lang-item"><div class="lang-dot" style="background:#ffb347"></div><span class="lang-name">Java</span><span class="lang-pct" style="color:#ffb347">17%</span></div>
        </div>
      </div>
    </div>

    <!-- Project impact bar chart -->
    <div class="chart-box" style="grid-column:1/-1">
      <div class="chart-label"><span class="dot cl-g"></span>Project focus areas</div>
      <div style="position:relative;height:140px">
        <canvas id="bar" role="img" aria-label="Project focus: AI/ML 40, Full Stack 30, Security 20, Fintech 10">AI/ML 40, Full Stack 30, Security 20, Fintech 10</canvas>
      </div>
    </div>

  </div>
</div>

<!-- PROJECTS -->
<div class="proj-section">
  <div style="text-align:center;padding:8px 0 20px"><div class="sec-title">🚀 What I've <span>Built</span></div></div>

  <div class="proj-card">
    <div class="proj-accent pa-v"></div>
    <div class="proj-inner">
      <span class="proj-emoji">🧠</span>
      <div class="proj-name">Local RAG</div>
      <div class="proj-sub ps-v">Private AI · Document Chat · Memory Vault</div>
      <p class="proj-desc">Chat with your PDFs, Word files and spreadsheets — fully private, zero cloud. Uses <strong>AI vision</strong> to read charts and tables, has a <strong>memory vault</strong> that remembers your preferences across sessions, and supports screenshot paste for multimodal queries.</p>
      <div class="proj-meta">
        <div class="proj-tags"><span class="ptag t-v">Python</span><span class="ptag t-v">Flask</span><span class="ptag t-b">Elasticsearch</span><span class="ptag t-v">Gemini Flash</span><span class="ptag t-o">SQLite</span></div>
        <button class="proj-link" onclick="openLink('https://github.com/aahona-16/Local-RAG')">↗ View Repo</button>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-accent pa-p"></div>
    <div class="proj-inner">
      <span class="proj-emoji">🤖</span>
      <div class="proj-name">AI Clinic Receptionist</div>
      <div class="proj-sub ps-p">Healthcare · 24/7 AI · 60–80% Workload Reduction</div>
      <p class="proj-desc">An AI-powered receptionist that handles patient queries around the clock and automates appointment scheduling. Understands patient intent, books appointments intelligently, and responds in real-time — <strong>built for real clinic deployment.</strong></p>
      <div class="proj-meta">
        <div class="proj-tags"><span class="ptag t-o">React</span><span class="ptag t-g">Node.js</span><span class="ptag t-v">OpenAI GPT</span><span class="ptag t-b">Firebase</span></div>
        <button class="proj-link" onclick="openLink('https://github.com/aahona-16/ai-clinic-receptionist')">↗ View Repo</button>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-accent pa-o"></div>
    <div class="proj-inner">
      <span class="proj-emoji">🔍</span>
      <div class="proj-name">Deep Packet Analyzer</div>
      <div class="proj-sub ps-o">Network Security · Real-Time DPI · C++</div>
      <p class="proj-desc">A multi-threaded C++ network inspection engine that analyzes live traffic, classifies apps using <strong>TLS SNI</strong> and HTTP headers, and applies blocking rules instantly. Parses PCAP at high speed and writes filtered output for security analysis.</p>
      <div class="proj-meta">
        <div class="proj-tags"><span class="ptag t-b">C++</span><span class="ptag t-o">Multi-threaded</span><span class="ptag t-g">PCAP</span><span class="ptag t-p">TLS SNI</span></div>
        <button class="proj-link" onclick="openLink('https://github.com/aahona-16/Packet_analyzer')">↗ View Repo</button>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-accent pa-g"></div>
    <div class="proj-inner">
      <span class="proj-emoji">💳</span>
      <div class="proj-name">UPI Without Internet</div>
      <div class="proj-sub ps-g">Offline Mesh Payments · RSA+AES-GCM · Idempotent</div>
      <p class="proj-desc">Payments hop device-to-device over Bluetooth until one gets signal and settles with the backend. Uses <strong>RSA-OAEP + AES-256-GCM encryption</strong> so no middleman can read the payment — and an <strong>atomic idempotency layer</strong> ensures it settles exactly once, even with 3 bridges uploading simultaneously.</p>
      <div class="proj-meta">
        <div class="proj-tags"><span class="ptag t-o">Java</span><span class="ptag t-g">Spring Boot</span><span class="ptag t-p">RSA+AES-GCM</span><span class="ptag t-b">H2 DB</span></div>
        <button class="proj-link" onclick="openLink('https://github.com/aahona-16/UPI_Without_Internet')">↗ View Repo</button>
      </div>
    </div>
  </div>
</div>

<!-- STACK -->
<div class="stack-section">
  <div style="text-align:center;padding:8px 0 4px"><div class="sec-title">🛠️ Tech <span>Stack</span></div></div>
  <div class="stack-grid">
    <div class="stack-card">
      <div class="stack-icon">⚡</div>
      <div class="stack-title">Languages</div>
      <div class="stack-list">
        <span class="stack-item si-v">JavaScript</span>
        <span class="stack-item si-p">Python</span>
        <span class="stack-item si-b">C++</span>
        <span class="stack-item si-o">Java</span>
      </div>
    </div>
    <div class="stack-card">
      <div class="stack-icon">🎨</div>
      <div class="stack-title">Frontend</div>
      <div class="stack-list">
        <span class="stack-item si-v">React</span>
        <span class="stack-item si-v">Next.js</span>
        <span class="stack-item si-p">React Native</span>
        <span class="stack-item si-o">HTML / CSS</span>
      </div>
    </div>
    <div class="stack-card">
      <div class="stack-icon">🔧</div>
      <div class="stack-title">Backend</div>
      <div class="stack-list">
        <span class="stack-item si-g">Node.js</span>
        <span class="stack-item si-g">Flask</span>
        <span class="stack-item si-g">Spring Boot</span>
        <span class="stack-item si-g">Express</span>
      </div>
    </div>
    <div class="stack-card">
      <div class="stack-icon">🤖</div>
      <div class="stack-title">AI / ML</div>
      <div class="stack-list">
        <span class="stack-item si-v">OpenAI GPT</span>
        <span class="stack-item si-v">Gemini</span>
        <span class="stack-item si-p">Scikit-learn</span>
        <span class="stack-item si-p">XGBoost</span>
      </div>
    </div>
    <div class="stack-card">
      <div class="stack-icon">🗄️</div>
      <div class="stack-title">Databases</div>
      <div class="stack-list">
        <span class="stack-item si-b">PostgreSQL</span>
        <span class="stack-item si-o">Firebase</span>
        <span class="stack-item si-b">Elasticsearch</span>
        <span class="stack-item si-b">SQLite</span>
      </div>
    </div>
  </div>
</div>

<!-- CONNECT -->
<div class="connect-section">
  <div class="sec-title">📬 Let's <span>Connect</span></div>
  <p style="font-size:13px;color:#666;margin-top:4px">Always down to talk AI, startups, or just cool ideas 🚀</p>
  <div class="connect-row">
    <div class="cc"><div class="cc-icon">💼</div><div class="cc-label">LinkedIn</div><div class="cc-val">aahona-mukhopadhyay</div></div>
    <div class="cc"><div class="cc-icon">✉️</div><div class="cc-label">Email</div><div class="cc-val">aahona1609@gmail.com</div></div>
    <div class="cc"><div class="cc-icon">🐙</div><div class="cc-label">GitHub</div><div class="cc-val">@aahona-16</div></div>
  </div>
</div>

<!-- FOOTER -->
<div class="footer">
  <div class="footer-q">" Code. Build. Learn. Repeat. "</div>
  <div class="footer-sub" style="color:#888">— always building, always learning</div>
</div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
<script>
const lines=['🚀 Turning ideas into real apps','🤖 Exploring AI & Scalable Systems','💡 Building useful tech, not brainrot','📚 Always learning, always shipping'];
let li=0,ci=0,del=false;
const el=document.getElementById('typed');
function tick(){const cur=lines[li];if(!del){el.textContent=cur.slice(0,++ci);if(ci===cur.length){del=true;setTimeout(tick,1800);return;}}else{el.textContent=cur.slice(0,--ci);if(ci===0){del=false;li=(li+1)%lines.length;setTimeout(tick,400);return;}}setTimeout(tick,del?35:65);}
tick();

const c=document.getElementById('confetti');
const cols=['#ff6b6b','#6c63ff','#00d68f','#ffb347','#00b4d8','#ff9ff3'];
for(let i=0;i<22;i++){const d=document.createElement('div');const s=6+Math.random()*8;d.className='confetti-dot';d.style.cssText=`width:${s}px;height:${s}px;left:${Math.random()*100}%;top:${20+Math.random()*70}%;background:${cols[i%cols.length]};--d:${3+Math.random()*4}s;--dl:-${Math.random()*4}s`;c.appendChild(d);}

new Chart(document.getElementById('donut'),{type:'doughnut',data:{labels:['JavaScript','Python','C++','Java'],datasets:[{data:[35,28,20,17],backgroundColor:['#6c63ff','#ff6b6b','#00d68f','#ffb347'],borderWidth:2,borderColor:'#fff'}]},options:{responsive:true,maintainAspectRatio:false,cutout:'68%',plugins:{legend:{display:false},tooltip:{callbacks:{label:c=>`${c.label}: ${c.parsed}%`}}}}});

new Chart(document.getElementById('bar'),{type:'bar',data:{labels:['AI / ML','Full Stack','Network Security','Fintech'],datasets:[{data:[40,30,20,10],backgroundColor:['#6c63ff','#ff6b6b','#00d68f','#ffb347'],borderRadius:8,borderSkipped:false}]},options:{responsive:true,maintainAspectRatio:false,plugins:{legend:{display:false}},scales:{x:{grid:{display:false},ticks:{color:'#888',font:{size:11,weight:'bold'}}},y:{grid:{color:'#f0edff'},ticks:{color:'#aaa',font:{size:10}},beginAtZero:true,max:50}}}});
</script>
