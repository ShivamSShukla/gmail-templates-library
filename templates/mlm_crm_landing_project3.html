<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>MLM-CRM Dashboard</title>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<style>
*{box-sizing:border-box;margin:0;padding:0}
:root{
  --bg:#ffffff;--text:#0a122a;--muted:#6b7280;--brand:#2563eb;--brand-2:#1e40af;--card:#f3f4f6;--stroke:#e5e7eb;--accent:#10b981;--warn:#f59e0b;--danger:#ef4444;--shadow:0 10px 30px rgba(2,6,23,.08)
}
:root.dark{
  --bg:#0b1220;--text:#e5e7eb;--muted:#9aa3b2;--brand:#60a5fa;--brand-2:#3b82f6;--card:#0f172a;--stroke:#1f2937;--accent:#34d399;--warn:#fbbf24;--danger:#f87171;--shadow:0 14px 34px rgba(0,0,0,.35)
}
html,body{height:100%}
body{font-family:system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Arial,Helvetica,sans-serif;background:var(--bg);color:var(--text);display:flex;min-height:100vh}
a{color:inherit;text-decoration:none}
.app{display:flex;width:100%}
.sidebar{width:280px;min-width:260px;background:linear-gradient(180deg,#ffffff 0%,#eef2ff 100%);border-right:1px solid var(--stroke);padding:24px;position:sticky;top:0;height:100vh}
:root.dark .sidebar{background:linear-gradient(180deg,#0b1220 0%,#0d1528 100%)}
.brand{display:flex;align-items:center;gap:12px;font-weight:800;font-size:20px;margin-bottom:24px;color:var(--brand-2)}
.brand .dot{width:12px;height:12px;border-radius:50%;background:var(--brand)}
.search{display:flex;align-items:center;gap:8px;background:var(--card);border:1px solid var(--stroke);padding:10px 12px;border-radius:12px;margin-bottom:18px}
.search input{border:none;outline:none;background:transparent;flex:1;color:var(--text)}
.nav{display:flex;flex-direction:column;gap:8px;margin-top:8px}
.nav button{width:100%;text-align:left;border:1px solid var(--stroke);background:var(--bg);padding:12px 14px;border-radius:12px;font-weight:600;color:var(--text);transition:.2s;display:flex;align-items:center;gap:10px}
.nav button.active{background:var(--brand);border-color:transparent;color:#fff}
.nav button:hover{transform:translateY(-2px)}
.tag{margin-left:auto;font-size:12px;background:var(--card);padding:2px 8px;border-radius:999px;border:1px solid var(--stroke)}
.main{flex:1;display:flex;flex-direction:column;min-width:0}
.topbar{display:flex;align-items:center;gap:12px;justify-content:space-between;padding:18px 22px;border-bottom:1px solid var(--stroke);position:sticky;top:0;background:var(--bg);z-index:20}
.hgroup{display:flex;flex-direction:column}
.hgroup h1{font-size:22px}
.hgroup p{color:var(--muted);font-size:13px}
.actions{display:flex;align-items:center;gap:10px}
.btn{border:1px solid var(--stroke);background:var(--bg);padding:10px 14px;border-radius:12px;font-weight:600;cursor:pointer}
.btn.brand{background:var(--brand);border-color:transparent;color:#fff}
.toggle{position:relative;width:48px;height:28px;border-radius:999px;background:var(--card);border:1px solid var(--stroke);cursor:pointer}
.toggle i{position:absolute;top:3px;left:3px;width:22px;height:22px;border-radius:50%;background:var(--brand);transition:.2s}
:root.dark .toggle i{left:23px;background:#111827}
.content{padding:22px;display:grid;grid-template-columns:1fr;gap:18px}
.cards{display:grid;grid-template-columns:repeat(12,1fr);gap:18px}
.card{grid-column:span 12;background:var(--bg);border:1px solid var(--stroke);border-radius:16px;box-shadow:var(--shadow)}
.card .inner{padding:18px}
.kpis{display:grid;grid-template-columns:repeat(12,1fr);gap:14px}
.kpi{grid-column:span 12;background:var(--card);border:1px solid var(--stroke);border-radius:14px;padding:16px}
.kpi h4{font-size:13px;color:var(--muted)}
.kpi .v{font-size:24px;font-weight:800;margin-top:6px}
@media(min-width:900px){
  .kpi{grid-column:span 3}
  .card.span6{grid-column:span 6}
}
.table{width:100%;border-collapse:collapse}
.table th,.table td{padding:12px 10px;border-bottom:1px solid var(--stroke);font-size:14px;text-align:left}
.badge{display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:999px;font-size:12px;border:1px solid var(--stroke);background:var(--bg)}
.badge.ok{background:rgba(16,185,129,.12);border-color:rgba(16,185,129,.25);color:var(--accent)}
.badge.w{background:rgba(245,158,11,.12);border-color:rgba(245,158,11,.25);color:var(--warn)}
.badge.d{background:rgba(239,68,68,.12);border-color:rgba(239,68,68,.25);color:var(--danger)}
.tree{display:flex;gap:20px;overflow:auto;padding-bottom:8px}
.node{min-width:180px;background:var(--card);border:1px solid var(--stroke);border-radius:12px;padding:12px}
.node h5{font-size:14px}
.node p{font-size:12px;color:var(--muted)}
.row{display:flex;gap:12px;margin-top:12px}
.threedots{position:fixed;right:20px;top:80px;z-index:25}
.dots-btn{width:44px;height:44px;border-radius:50%;border:1px solid var(--stroke);background:var(--bg);box-shadow:var(--shadow);cursor:pointer;font-weight:900}
.panel{position:fixed;right:20px;top:136px;width:280px;max-height:70vh;overflow:auto;background:var(--bg);border:1px solid var(--stroke);border-radius:16px;box-shadow:var(--shadow);display:none}
.panel .inner{padding:16px;display:flex;flex-direction:column;gap:10px}
.panel .item{display:flex;align-items:center;justify-content:space-between;border:1px solid var(--stroke);border-radius:12px;padding:10px 12px;background:var(--card)}
.panel .item b{font-size:14px}
.panel .links{display:flex;flex-direction:column;gap:8px}
.panel .links a{border:1px solid var(--stroke);background:var(--bg);padding:10px 12px;border-radius:10px;font-weight:600}
.chat{position:fixed;right:20px;bottom:20px;z-index:26}
.chat button{border:none;background:var(--brand);color:#fff;padding:12px 16px;border-radius:999px;font-weight:700;box-shadow:var(--shadow);cursor:pointer}
.chatbox{position:fixed;right:20px;bottom:70px;width:320px;max-height:420px;border:1px solid var(--stroke);background:var(--bg);border-radius:16px;box-shadow:var(--shadow);display:none;overflow:hidden}
.chatbox header{padding:12px 14px;border-bottom:1px solid var(--stroke);display:flex;align-items:center;justify-content:space-between}
.chatlog{padding:12px;display:flex;flex-direction:column;gap:10px;max-height:300px;overflow:auto}
.msg{padding:10px 12px;border-radius:12px;max-width:82%}
.msg.bot{background:var(--card);border:1px solid var(--stroke)}
.msg.me{background:var(--brand);color:#fff;margin-left:auto}
.chatbox footer{display:flex;gap:8px;padding:12px;border-top:1px solid var(--stroke)}
.chatbox input{flex:1;border:1px solid var(--stroke);background:var(--bg);border-radius:10px;padding:10px 12px;color:var(--text);outline:none}
.chatbox .send{border:none;background:var(--brand-2);color:#fff;padding:10px 14px;border-radius:10px;font-weight:700;cursor:pointer}
.small{font-size:12px;color:var(--muted)}
.hr{height:1px;background:var(--stroke);margin:12px 0}
</style>
</head>
<body>
<div class="app">
  <aside class="sidebar">
    <div class="brand"><span class="dot"></span> MLM‑CRM</div>
    <div class="search"><span>🔎</span><input id="search" placeholder="Search leads or reps"></div>
    <nav class="nav">
      <button data-page="dashboard" class="active">🏠 Dashboard</button>
      <button data-page="network">🧬 MLM Network <span class="tag">view</span></button>
      <button data-page="leads">📇 Leads <span class="tag">12</span></button>
      <button data-page="reps">🧑‍💼 Sales Reps</button>
      <button data-page="reports">📊 Reports</button>
      <button data-page="settings">⚙️ Settings</button>
    </nav>
  </aside>

  <main class="main">
    <div class="topbar">
      <div class="hgroup">
        <h1 id="title">Dashboard</h1>
        <p id="subtitle">Overview of performance, leads, and network growth</p>
      </div>
      <div class="actions">
        <div class="toggle" id="mode"><i></i></div>
        <button class="btn" id="export">Export CSV</button>
        <button class="btn brand" id="newLead">+ New Lead</button>
      </div>
    </div>

    <div class="content" id="content">
      <div class="cards">
        <div class="card"><div class="inner">
          <div class="kpis">
            <div class="kpi"><h4>Total Downline</h4><div class="v" id="kpiDownline">1,248</div><div class="small">+3.1% this week</div></div>
            <div class="kpi"><h4>Active Leads</h4><div class="v" id="kpiLeads">312</div><div class="small">Automation on 74%</div></div>
            <div class="kpi"><h4>Conversion Rate</h4><div class="v" id="kpiConv">18.6%</div><div class="small">Qualified ↑</div></div>
            <div class="kpi"><h4>Payouts (Month)</h4><div class="v" id="kpiPayout">$42,910</div><div class="small">On schedule</div></div>
          </div>
        </div></div>

        <div class="card span6"><div class="inner">
          <h3>Lead Nurturing Timeline</h3>
          <div class="hr"></div>
          <table class="table" id="timeline">
            <thead><tr><th>Lead</th><th>Stage</th><th>Next Step</th><th>Status</th></tr></thead>
            <tbody></tbody>
          </table>
        </div></div>

        <div class="card span6"><div class="inner">
          <h3>Recent Activity</h3>
          <div class="hr"></div>
          <table class="table" id="activity">
            <thead><tr><th>Time</th><th>User</th><th>Action</th><th>Result</th></tr></thead>
            <tbody></tbody>
          </table>
        </div></div>
      </div>
    </div>
  </main>
</div>

<div class="threedots">
  <button class="dots-btn" id="dots">⋮</button>
  <div class="panel" id="panel">
    <div class="inner">
      <div class="item"><b>Quick Theme</b><span id="quickTheme" class="badge">Toggle</span></div>
      <div class="item"><b>New Lead</b><span id="quickLead" class="badge ok">Create</span></div>
      <div class="item"><b>Import CSV</b><span class="badge w">Coming</span></div>
      <div class="item"><b>Payout Rules</b><span class="badge">Open</span></div>
      <div class="links">
        <a data-page="dashboard">Go to Dashboard</a>
        <a data-page="network">Go to MLM Network</a>
        <a data-page="leads">Go to Leads</a>
        <a data-page="reps">Go to Sales Reps</a>
        <a data-page="reports">Go to Reports</a>
      </div>
    </div>
  </div>
</div>

<div class="chat">
  <button id="chatBtn">💬 Chat</button>
  <div class="chatbox" id="chatBox">
    <header><b>MLM Assistant</b><button class="btn" id="closeChat">Close</button></header>
    <div class="chatlog" id="chatLog">
      <div class="msg bot">Hi! Ask me about MLM networks, leads, nurturing, or roles.</div>
    </div>
    <footer>
      <input id="chatInput" placeholder="Type a question...">
      <button class="send" id="chatSend">Send</button>
    </footer>
  </div>
</div>

<script>
const $=s=>document.querySelector(s);const $$=s=>document.querySelectorAll(s);
function setPage(p){
  $$(".nav button").forEach(b=>b.classList.toggle("active",b.dataset.page===p));
  $("#title").textContent=p[0].toUpperCase()+p.slice(1);
  const sub={
    dashboard:"Overview of performance, leads, and network growth",
    network:"Explore downlines, levels, and commission flow",
    leads:"Manage prospects with automation and scoring",
    reps:"Track rep performance and assignments",
    reports:"KPIs, payouts, conversions, growth trends",
    settings:"Preferences, roles, and payout rules"
  };
  $("#subtitle").textContent=sub[p]||"";
  const c=$("#content");c.innerHTML="";
  if(p==="dashboard"){renderDashboard(c)} 
  else if(p==="network"){renderNetwork(c)}
  else if(p==="leads"){renderLeads(c)}
  else if(p==="reps"){renderReps(c)}
  else if(p==="reports"){renderReports(c)}
  else if(p==="settings"){renderSettings(c)}
}
$$(".nav button").forEach(b=>b.addEventListener("click",()=>setPage(b.dataset.page)));
$("#newLead").addEventListener("click",()=>promptNewLead());
$("#export").addEventListener("click",()=>exportCSV());
$("#dots").addEventListener("click",()=>togglePanel());
$("#quickTheme").addEventListener("click",()=>toggleMode());
$("#quickLead").addEventListener("click",()=>promptNewLead());
$$(".panel .links a").forEach(a=>a.addEventListener("click",e=>{e.preventDefault();togglePanel(false);setPage(a.dataset.page)}));
function togglePanel(force){const p=$("#panel");const show=force!==undefined?force:p.style.display!=="block";p.style.display=show?"block":"none"}
const mode=$("#mode");mode.addEventListener("click",toggleMode);
function toggleMode(){
  const d=document.documentElement;
  d.classList.toggle("dark");
  localStorage.setItem("mlm_mode",d.classList.contains("dark")?"dark":"light");
  const k="mlm_demo_data";const raw=localStorage.getItem(k);if(raw){localStorage.setItem(k,raw)}
}
(function(){const m=localStorage.getItem("mlm_mode");if(m==="dark")document.documentElement.classList.add("dark")})();
function cardWrap(title,body){
  const wrap=document.createElement("div");
  wrap.className="card";const inner=document.createElement("div");inner.className="inner";
  const h=document.createElement("h3");h.textContent=title;inner.appendChild(h);
  const hr=document.createElement("div");hr.className="hr";inner.appendChild(hr);
  inner.appendChild(body);wrap.appendChild(inner);return wrap
}
function renderDashboard(c){
  const kpi=document.createElement("div");kpi.className="cards";
  const top=document.createElement("div");top.className="card";const tIn=document.createElement("div");tIn.className="inner";
  const grid=document.createElement("div");grid.className="kpis";
  const items=[["Total Downline","1,248","+3.1% this week"],["Active Leads","312","Automation on 74%"],["Conversion Rate","18.6%","Qualified ↑"],["Payouts (Month)","$42,910","On schedule"]];
  items.forEach(x=>{const d=document.createElement("div");d.className="kpi";d.innerHTML=`<h4>${x[0]}</h4><div class="v">${x[1]}</div><div class="small">${x[2]}</div>`;grid.appendChild(d)});
  tIn.appendChild(grid);top.appendChild(tIn);c.appendChild(top);
  const left=mkTimeline();left.classList.add("span6");c.appendChild(left);
  const right=mkActivity();right.classList.add("span6");c.appendChild(right)
}
function mkTimeline(){
  const box=document.createElement("div");box.className="card";const inn=document.createElement("div");inn.className="inner";
  const h=document.createElement("h3");h.textContent="Lead Nurturing Timeline";const hr=document.createElement("div");hr.className="hr";
  const table=document.createElement("table");table.className="table";table.innerHTML=`<thead><tr><th>Lead</th><th>Stage</th><th>Next Step</th><th>Status</th></tr></thead><tbody></tbody>`;
  const data=[["Asha Patel","Qualified","Call 10:00","ok"],["Daniel Kim","Nurturing","Email Day 3","w"],["M. Alvarez","Proposal","Review terms","ok"],["Sara Noor","New","Assign rep","w"],["John Lee","Dormant","Re‑engage campaign","d"]];
  const tb=table.querySelector("tbody");
  data.forEach(r=>{const tr=document.createElement("tr");const badge=r[3]==="ok"?"ok":r[3]==="w"?"w":"d";tr.innerHTML=`<td>${r[0]}</td><td>${r[1]}</td><td>${r[2]}</td><td><span class="badge ${badge}">${r[3]==="ok"?"On track":r[3]==="w"?"Pending":"Stalled"}</span></td>`;tb.appendChild(tr)});
  inn.append(h,hr,table);box.appendChild(inn);return box
}
function mkActivity(){
  const box=document.createElement("div");box.className="card";const inn=document.createElement("div");inn.className="inner";
  const h=document.createElement("h3");h.textContent="Recent Activity";const hr=document.createElement("div");hr.className="hr";
  const table=document.createElement("table");table.className="table";table.innerHTML=`<thead><tr><th>Time</th><th>User</th><th>Action</th><th>Result</th></tr></thead><tbody></tbody>`;
  const data=[["09:10","S. Reed","Sent follow‑up","Opened"],["08:42","I. Chen","Added lead","Queued"],["Yesterday","Admin","Updated payout","Saved"],["Yesterday","A. Musa","Qualified lead","Converted"]];
  const tb=table.querySelector("tbody");data.forEach(r=>{const tr=document.createElement("tr");tr.innerHTML=`<td>${r[0]}</td><td>${r[1]}</td><td>${r[2]}</td><td>${r[3]}</td>`;tb.appendChild(tr)});
  inn.append(h,hr,table);box.appendChild(inn);return box
}
function renderNetwork(c){
  const wrap=document.createElement("div");wrap.className="cards";
  const intro=cardWrap("Network Snapshot",document.createElement("div"));
  intro.querySelector(".inner").insertAdjacentHTML("beforeend",`<div class="kpis"><div class="kpi"><h4>Levels</h4><div class="v">5</div></div><div class="kpi"><h4>Active Nodes</h4><div class="v">874</div></div><div class="kpi"><h4>Avg. Depth</h4><div class="v">3.2</div></div><div class="kpi"><h4>This Week</h4><div class="v">+48</div></div></div>`);
  wrap.appendChild(intro);
  const treeCard=document.createElement("div");treeCard.className="card";const inner=document.createElement("div");inner.className="inner";
  const tree=document.createElement("div");tree.className="tree";
  const root=node("You","Tier 0","$1,240");
  const row1=row([node("Team A","Tier 1","$520"),node("Team B","Tier 1","$410"),node("Team C","Tier 1","$310")]);
  const row2=row([node("A‑1","Tier 2","$210"),node("A‑2","Tier 2","$160"),node("B‑1","Tier 2","$180"),node("C‑1","Tier 2","$140")]);
  tree.append(root,row1,row2);
  inner.appendChild(tree);treeCard.appendChild(inner);wrap.appendChild(treeCard);
  c.appendChild(wrap)
  function node(name,tier,payout){const d=document.createElement("div");d.className="node";d.innerHTML=`<h5>${name}</h5><p>${tier}</p><div class="hr"></div><div class="small">Payout: ${payout}</div>`;return d}
  function row(children){const r=document.createElement("div");r.className="row";children.forEach(ch=>r.appendChild(ch));return r}
}
const seedLeads=[{name:"Asha Patel",email:"asha@example.com",phone:"+1‑555‑0142",stage:"Qualified",score:82,status:"On track"},{name:"Daniel Kim",email:"daniel@example.com",phone:"+1‑555‑0174",stage:"Nurturing",score:64,status:"Pending"},{name:"Mei Lin",email:"mei@example.com",phone:"+1‑555‑0109",stage:"Proposal",score:91,status:"On track"},{name:"John Lee",email:"john@example.com",phone:"+1‑555‑0133",stage:"New",score:38,status:"Pending"}];
function getLeads(){const k="mlm_demo_data";const raw=localStorage.getItem(k);if(raw){try{return JSON.parse(raw)}catch{return seedLeads}}localStorage.setItem(k,JSON.stringify(seedLeads));return seedLeads}
function setLeads(arr){localStorage.setItem("mlm_demo_data",JSON.stringify(arr))}
function renderLeads(c){
  const wrap=document.createElement("div");wrap.className="cards";
  const card=document.createElement("div");card.className="card";const inner=document.createElement("div");inner.className="inner";
  const head=document.createElement("div");head.style.display="flex";head.style.justifyContent="space-between";head.style.alignItems="center";
  const h=document.createElement("h3");h.textContent="Leads";const tools=document.createElement("div");
  const f=document.createElement("input");f.placeholder="Filter by name or stage";f.style.border="1px solid var(--stroke)";f.style.background="var(--bg)";f.style.padding="10px 12px";f.style.borderRadius="10px";f.style.minWidth="240px";
  tools.appendChild(f);head.append(h,tools);
  const table=document.createElement("table");table.className="table";table.innerHTML=`<thead><tr><th>Name</th><th>Email</th><th>Phone</th><th>Stage</th><th>Score</th><th>Status</th></tr></thead><tbody></tbody>`;
  const tb=table.querySelector("tbody");
  const renderRows=(rows)=>{tb.innerHTML="";rows.forEach(r=>{const tr=document.createElement("tr");const badge=r.status==="On track"?"ok":r.status==="Pending"?"w":"d";tr.innerHTML=`<td>${r.name}</td><td>${r.email}</td><td>${r.phone}</td><td>${r.stage}</td><td>${r.score}</td><td><span class="badge ${badge}">${r.status}</span></td>`;tb.appendChild(tr)})};
  const data=getLeads();renderRows(data);
  f.addEventListener("input",()=>{const q=f.value.toLowerCase();renderRows(data.filter(d=>[d.name,d.stage].join("|").toLowerCase().includes(q)))});
  inner.append(head,document.createElement("div"),table);card.appendChild(inner);wrap.appendChild(card);
  const add=document.createElement("div");add.className="card";const aI=document.createElement("div");aI.className="inner";
  const form=document.createElement("form");form.style.display="grid";form.style.gridTemplateColumns="repeat(12,1fr)";form.style.gap="12px";
  form.innerHTML=`<input required placeholder="Name" style="grid-column:span 3;padding:12px;border:1px solid var(--stroke);background:var(--bg);border-radius:10px">
  <input required placeholder="Email" style="grid-column:span 3;padding:12px;border:1px solid var(--stroke);background:var(--bg);border-radius:10px">
  <input required placeholder="Phone" style="grid-column:span 3;padding:12px;border:1px solid var(--stroke);background:var(--bg);border-radius:10px">
  <select style="grid-column:span 2;padding:12px;border:1px solid var(--stroke);background:var(--bg);border-radius:10px">
    <option>New</option><option>Nurturing</option><option>Qualified</option><option>Proposal</option>
  </select>
  <input type="number" min="0" max="100" value="50" style="grid-column:span 1;padding:12px;border:1px solid var(--stroke);background:var(--bg);border-radius:10px">
  <button class="btn brand" style="grid-column:span 12">Add Lead</button>`;
  form.addEventListener("submit",e=>{
    e.preventDefault();
    const v=[...form.querySelectorAll("input,select")].map(x=>x.value);
    const row={name:v[0],email:v[1],phone:v[2],stage:v[3],score:parseInt(v[4],10)||0,status:v[3]==="Qualified"||v[3]==="Proposal"?"On track":"Pending"};
    const cur=getLeads();cur.unshift(row);setLeads(cur);setPage("leads")
  });
  aI.appendChild(form);add.appendChild(aI);wrap.appendChild(add);
  c.appendChild(wrap)
}
function renderReps(c){
  const wrap=document.createElement("div");wrap.className="cards";
  const card=document.createElement("div");card.className="card";const inn=document.createElement("div");inn.className="inner";
  const table=document.createElement("table");table.className="table";
  table.innerHTML=`<thead><tr><th>Rep</th><th>Email</th><th>Leads</th><th>Conversion</th><th>Status</th></tr></thead><tbody></tbody>`;
  const rows=[["Samuel Reed","samuel@crm.io",64,"21%","Active"],["Imani Chen","imani@crm.io",52,"18%","Active"],["Ahmed Musa","ahmed@crm.io",31,"24%","Active"],["Lina Ortiz","lina@crm.io",22,"15%","On leave"]];
  const tb=table.querySelector("tbody");rows.forEach(r=>{const tr=document.createElement("tr");tr.innerHTML=`<td>${r[0]}</td><td>${r[1]}</td><td>${r[2]}</td><td>${r[3]}</td><td>${r[4]}</td>`;tb.appendChild(tr)});
  inn.appendChild(table);card.appendChild(inn);wrap.appendChild(card);c.appendChild(wrap)
}
function renderReports(c){
  const wrap=document.createElement("div");wrap.className="cards";
  const left=cardWrap("Monthly Snapshot",document.createElement("div"));
  left.querySelector(".inner").insertAdjacentHTML("beforeend",`<div class="kpis"><div class="kpi"><h4>New Leads</h4><div class="v">188</div></div><div class="kpi"><h4>Qualified</h4><div class="v">96</div></div><div class="kpi"><h4>Closed Won</h4><div class="v">31</div></div><div class="kpi"><h4>Payouts</h4><div class="v">$128,440</div></div></div>`);
  const right=cardWrap("Notes",document.createElement("div"));
  right.querySelector(".inner").insertAdjacentHTML("beforeend",`<div class="small">Automation series A/B shows higher open rate on Day 2; consider moving call task to Day 3 for cold segments.</div>`);
  wrap.append(left,right);c.appendChild(wrap)
}
function renderSettings(c){
  const card=document.createElement("div");card.className="card";const inn=document.createElement("div");inn.className="inner";
  const box=document.createElement("div");box.style.display="grid";box.style.gridTemplateColumns="repeat(12,1fr)";box.style.gap="12px";
  box.innerHTML=`<label style="grid-column:span 6">Default Mode<select id="prefMode" style="width:100%;padding:10px;border:1px solid var(--stroke);background:var(--bg);border-radius:10px"><option>Light</option><option>Dark</option></select></label>
  <label style="grid-column:span 6">Timezone<select style="width:100%;padding:10px;border:1px solid var(--stroke);background:var(--bg);border-radius:10px"><option>UTC</option><option selected>Africa/Addis_Ababa</option><option>Asia/Kolkata</option></select></label>
  <button id="savePref" class="btn brand" style="grid-column:span 12">Save Preferences</button>`;
  inn.appendChild(box);card.appendChild(inn);c.appendChild(card);
  const pref=$("#prefMode");pref.value=document.documentElement.classList.contains("dark")?"Dark":"Light";
  $("#savePref").addEventListener("click",()=>{if(pref.value==="Dark"){document.documentElement.classList.add("dark")}else{document.documentElement.classList.remove("dark")}localStorage.setItem("mlm_mode",pref.value==="Dark"?"dark":"light")})
}
function promptNewLead(){
  const name=prompt("Lead name");if(!name)return;
  const email=prompt("Email");if(!email)return;
  const phone=prompt("Phone");if(!phone)return;
  const stage=prompt("Stage (New, Nurturing, Qualified, Proposal)")||"New";
  const score=Math.max(0,Math.min(100,parseInt(prompt("Score 0-100")||"50",10)));
  const row={name,email,phone,stage,score,status:stage==="Qualified"||stage==="Proposal"?"On track":"Pending"};
  const cur=getLeads();cur.unshift(row);setLeads(cur);setPage("leads")
}
function exportCSV(){
  const rows=[["name","email","phone","stage","score","status"],...getLeads().map(r=>[r.name,r.email,r.phone,r.stage,r.score,r.status])];
  const csv=rows.map(r=>r.map(x=>`"${String(x).replace(/"/g,'""')}"`).join(",")).join("\n");
  const blob=new Blob([csv],{type:"text/csv"});const url=URL.createObjectURL(blob);
  const a=document.createElement("a");a.href=url;a.download="leads.csv";document.body.appendChild(a);a.click();a.remove();URL.revokeObjectURL(url)
}
const chatBtn=$("#chatBtn");const chatBox=$("#chatBox");const chatLog=$("#chatLog");const chatInput=$("#chatInput");const chatSend=$("#chatSend");const closeChat=$("#closeChat");
chatBtn.addEventListener("click",()=>chatBox.style.display=chatBox.style.display==="block"?"none":"block");
closeChat.addEventListener("click",()=>chatBox.style.display="none");
chatSend.addEventListener("click",sendChat);chatInput.addEventListener("keydown",e=>{if(e.key==="Enter"){sendChat()}});
function sendChat(){
  const q=chatInput.value.trim();if(!q)return;
  addMsg(q,"me");chatInput.value="";setTimeout(()=>{addMsg(reply(q),"bot");chatLog.scrollTop=chatLog.scrollHeight},300)
}
function addMsg(t,role){const m=document.createElement("div");m.className="msg "+role;m.textContent=t;chatLog.appendChild(m);chatLog.scrollTop=chatLog.scrollHeight}
function reply(q){
  const s=q.toLowerCase();
  if(s.includes("mlm")&&s.includes("track"))return "Use the MLM Network page to view levels, downlines, and payouts. You can expand nodes and monitor growth by tier.";
  if(s.includes("lead")&&s.includes("nurtur"))return "Leads move through New → Nurturing → Qualified → Proposal. Automation sends timed emails and sets call tasks.";
  if(s.includes("role")||s.includes("rep"))return "Roles include Sales Rep, Manager, and Admin. Access is limited by role; conversions are credited to assigned reps.";
  if(s.includes("commission")||s.includes("payout"))return "Payouts roll up by tier monthly. Reports show totals, and Settings lets you adjust percentages.";
  if(s.includes("dark")||s.includes("theme"))return "Toggle the theme using the switch in the top-right or the three‑dots quick panel.";
  return "I can help with MLM network, leads, roles, payouts, and theme. Ask me about any of these."
}
setPage("dashboard");
</script>
</body>
</html>
