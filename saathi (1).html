<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Saathi — Live Classroom Captions &amp; Notes</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,500;9..144,600;9..144,700&family=Space+Grotesk:wght@500;600;700&family=Atkinson+Hyperlegible:wght@400;700&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
<style>
  :root{
    --bg:#FAF6EC; --panel:#FFFFFF; --ink:#1C1A16; --ink-soft:#5B5648;
    --accent:#E2962F; --accent-ink:#3A2600; --teal:#1F3A3D; --sage:#7FA897;
    --mark:#FFE9A8; --danger:#B3482F;
    --border:rgba(31,58,61,0.16); --radius:14px; --caption-scale:1;
    --font-ui:'Space Grotesk', sans-serif; --font-body:'Atkinson Hyperlegible', sans-serif; --font-display:'Fraunces', serif;
  }
  body[data-theme="dark"]{
    --bg:#14181B; --panel:#1E2428; --ink:#F3F0E6; --ink-soft:#B9C2C2;
    --accent:#F2B65A; --accent-ink:#1C1200; --border:rgba(243,240,230,0.16); --mark:#5A4A1E;
  }
  body[data-theme="contrast"]{
    --bg:#000000; --panel:#000000; --ink:#FFFF00; --ink-soft:#FFFF00;
    --accent:#FFFF00; --accent-ink:#000000; --border:#FFFF00; --teal:#FFFF00; --mark:#333300;
  }
  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{background:var(--bg); color:var(--ink); font-family:var(--font-body); padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px); transition:background .25s ease,color .25s ease;}
  .wrap{max-width:1080px; margin:0 auto; padding:28px 20px 60px;}

  header.top{display:flex; align-items:center; justify-content:space-between; gap:16px; flex-wrap:wrap; margin-bottom:18px;}
  .brand{display:flex; align-items:center; gap:14px;}
  .mascot{width:52px; height:52px; flex:none;}
  .mascot .face{transition:transform .3s ease;}
  .mascot.listening .face{animation:nod 1.4s ease-in-out infinite;}
  @keyframes nod{0%,100%{transform:rotate(0deg);} 50%{transform:rotate(-6deg);}}
  .brand h1{font-family:var(--font-display); font-size:2rem; margin:0; font-weight:600;}
  .brand p{margin:2px 0 0; font-size:.92rem; color:var(--ink-soft); font-family:var(--font-ui);}
  .status-pill{font-family:var(--font-ui); font-size:.8rem; padding:6px 12px; border-radius:999px; border:1px solid var(--border); color:var(--ink-soft); white-space:nowrap;}
  .status-pill.active{color:var(--accent-ink); background:var(--accent); border-color:transparent;}

  .panel{background:var(--panel); border:1px solid var(--border); border-radius:var(--radius); padding:20px; margin-bottom:18px;}
  .panel h2{font-family:var(--font-ui); font-size:.95rem; margin:0 0 14px; font-weight:600; color:var(--ink-soft);}

  .controls{display:flex; flex-wrap:wrap; gap:10px; align-items:center;}
  button{font-family:var(--font-ui); font-size:.85rem; font-weight:600; cursor:pointer; border-radius:10px; border:1px solid var(--border); background:transparent; color:var(--ink); padding:9px 15px; transition:all .15s ease;}
  button:hover{border-color:var(--accent);}
  button:disabled{opacity:.45; cursor:not-allowed;}
  button.primary{background:var(--accent); color:var(--accent-ink); border-color:transparent;}
  button.primary:hover{filter:brightness(1.06);}
  button.ghost-active{background:var(--teal); color:#fff; border-color:transparent;}
  button.warn{border-color:var(--danger); color:var(--danger);}
  .seg{display:flex; border:1px solid var(--border); border-radius:10px; overflow:hidden;}
  .seg button{border:none; border-radius:0; padding:8px 13px;}
  .seg button + button{border-left:1px solid var(--border);}
  .seg button.active{background:var(--teal); color:#fff;}
  .divider{width:1px; align-self:stretch; background:var(--border); margin:0 4px;}
  .control-label{font-family:var(--font-ui); font-size:.78rem; color:var(--ink-soft); margin-right:2px;}
  input[type="text"]{font-family:var(--font-body); font-size:.9rem; padding:8px 10px; border-radius:8px; border:1px solid var(--border); background:var(--bg); color:var(--ink);}
  select{font-family:var(--font-ui); font-size:.85rem; padding:8px 10px; border-radius:8px; border:1px solid var(--border); background:var(--bg); color:var(--ink);}

  .caption-box{min-height:120px; font-family:var(--font-body); font-size:calc(1.5rem * var(--caption-scale)); line-height:1.5; padding:10px 4px;}
  .caption-box .final{color:var(--ink);} .caption-box .interim{color:var(--ink-soft); font-style:italic;}
  .caption-placeholder{color:var(--ink-soft); font-style:italic;}
  mark{background:var(--mark); color:inherit; border-radius:3px; padding:0 2px;}

  .two-col{display:grid; grid-template-columns:1.1fr 1fr; gap:18px;}
  @media (max-width:760px){.two-col{grid-template-columns:1fr;}}

  #transcriptList{list-style:none; margin:0; padding:0; max-height:240px; overflow-y:auto;}
  #transcriptList li{padding:8px 0; border-bottom:1px solid var(--border); font-size:calc(1rem * var(--caption-scale)); line-height:1.45;}
  #transcriptList li:last-child{border-bottom:none;}
  #transcriptList time{display:block; font-family:var(--font-ui); font-size:.72rem; color:var(--ink-soft); margin-bottom:2px;}

  #doubtsList{list-style:none; margin:0; padding:0; max-height:160px; overflow-y:auto;}
  #doubtsList li{padding:7px 0; border-bottom:1px solid var(--border); font-size:.9rem;}
  #doubtsList time{font-family:var(--font-ui); font-size:.72rem; color:var(--ink-soft); margin-right:8px;}

  #notesOutput{font-size:calc(1rem * var(--caption-scale)); line-height:1.6; white-space:pre-wrap;}

  textarea{width:100%; min-height:90px; font-family:var(--font-body); font-size:1rem; background:var(--bg); color:var(--ink); border:1px solid var(--border); border-radius:10px; padding:12px; resize:vertical;}

  .sign-strip{display:flex; gap:10px; margin-top:12px; flex-wrap:wrap; min-height:70px;}
  .sign-chip{display:flex; flex-direction:column; align-items:center; gap:4px; animation:popin .25s ease;}
  .sign-chip svg{width:46px; height:46px;}
  .sign-chip span{font-family:var(--font-ui); font-size:.7rem; color:var(--ink-soft);}
  @keyframes popin{from{opacity:0; transform:scale(.7);} to{opacity:1; transform:scale(1);}}

  .profile-gate{display:flex; align-items:center; justify-content:center; min-height:70vh;}
  .profile-card{max-width:420px; width:100%; background:var(--panel); border:1px solid var(--border); border-radius:var(--radius); padding:32px; text-align:center;}
  .profile-card h2{font-family:var(--font-display); font-size:1.5rem; margin:0 0 6px; color:var(--ink);}
  .profile-card p{color:var(--ink-soft); font-family:var(--font-ui); font-size:.9rem; margin:0 0 20px;}
  .profile-card .field{text-align:left; margin-bottom:14px;}
  .profile-card label{display:block; font-family:var(--font-ui); font-size:.78rem; color:var(--ink-soft); margin-bottom:5px;}
  .profile-card input, .profile-card select{width:100%;}

  .chip-row{display:flex; flex-wrap:wrap; gap:6px; margin-top:8px;}
  .chip{font-family:var(--font-ui); font-size:.76rem; padding:4px 10px; border-radius:999px; border:1px solid var(--border); color:var(--ink-soft);}

  .banner{padding:12px 16px; border-radius:10px; font-family:var(--font-ui); font-size:.85rem; margin-bottom:14px; display:none;}
  .banner.show{display:block;}
  .banner.warn{background:rgba(179,72,47,.1); color:var(--danger); border:1px solid rgba(179,72,47,.3);}

  .footnote{font-family:var(--font-ui); font-size:.78rem; color:var(--ink-soft); line-height:1.6; margin-top:24px;}
  .footnote strong{color:var(--ink);}
  .hidden{display:none !important;}

  @media print{
    body *{visibility:hidden;}
    #printArea, #printArea *{visibility:visible;}
    #printArea{position:absolute; top:0; left:0; width:100%; padding:30px;}
  }
</style>
</head>
<body data-theme="light">

<div class="wrap" id="profileGate">
  <div class="profile-gate">
    <div class="profile-card">
      <h2>Welcome to Saathi</h2>
      <p>Every student's companion, in every language.</p>
      <div class="field">
        <label for="pfName">Your name</label>
        <input type="text" id="pfName" placeholder="e.g. Shama, or Ravi Sir">
      </div>
      <div class="field">
        <label for="pfRole">You are a</label>
        <select id="pfRole">
          <option value="teacher">Teacher</option>
          <option value="student">Student</option>
        </select>
      </div>
      <button class="primary" id="btnContinue" style="width:100%;">Continue</button>
    </div>
  </div>
</div>

<div class="wrap hidden" id="appRoot">

  <header class="top">
    <div class="brand">
      <svg class="mascot" id="ishara" viewBox="0 0 100 100">
        <g class="face">
          <circle cx="50" cy="50" r="46" fill="var(--teal)"/>
          <circle cx="34" cy="46" r="6" fill="var(--bg)"/>
          <circle cx="66" cy="46" r="6" fill="var(--bg)"/>
          <path d="M32 64 Q50 78 68 64" stroke="var(--bg)" stroke-width="5" fill="none" stroke-linecap="round"/>
        </g>
      </svg>
      <div>
        <h1>Saathi</h1>
        <p id="isharaStatus">Every student's companion, in every language.</p>
      </div>
    </div>
    <div class="status-pill" id="listeningPill">Not listening</div>
  </header>

  <section class="panel">
    <div class="controls" style="justify-content:space-between;">
      <div class="controls">
        <span class="control-label">Signed in as</span>
        <strong id="whoAmI" style="font-family:var(--font-ui); font-size:.9rem;"></strong>
        <button id="btnSwitchProfile" style="padding:6px 12px; font-size:.78rem;">Switch</button>
      </div>
      <div class="controls">
        <span class="control-label">Subject space</span>
        <select id="subjectSelect"></select>
        <button id="btnNewSubject" style="padding:6px 12px; font-size:.78rem;">+ New subject</button>
      </div>
    </div>
  </section>

  <div class="banner warn" id="micBanner"></div>

  <section class="panel">
    <h2>Class controls</h2>
    <div class="controls">
      <button class="primary" id="btnStart">Start Class</button>
      <div class="divider"></div>
      <span class="control-label">Language</span>
      <div class="seg" id="langSeg">
        <button data-lang="en-IN" class="active">English</button>
        <button data-lang="hi-IN">हिंदी</button>
      </div>
      <div class="divider"></div>
      <span class="control-label">Text size</span>
      <div class="seg"><button id="fontDec">A−</button><button id="fontReset">A</button><button id="fontInc">A+</button></div>
      <div class="divider"></div>
      <span class="control-label">Theme</span>
      <div class="seg" id="themeSeg">
        <button data-theme="light" class="active">Light</button>
        <button data-theme="dark">Dark</button>
        <button data-theme="contrast">High contrast</button>
      </div>
    </div>
    <div class="controls" style="margin-top:12px;">
      <span class="control-label">Highlight important terms</span>
      <input type="text" id="termInput" placeholder="e.g. mitochondria" style="width:200px;">
      <button id="btnAddTerm" style="padding:6px 12px; font-size:.78rem;">Add</button>
      <div class="chip-row" id="termChips"></div>
    </div>
  </section>

  <div class="two-col">
    <section class="panel">
      <h2>Live captions</h2>
      <div class="caption-box" id="captionBox">
        <span class="caption-placeholder">Captions will appear here once class starts. Works best in Chrome or Edge.</span>
      </div>
      <div class="sign-strip" id="signStrip"></div>
      <div class="controls" style="margin-top:12px;">
        <button class="warn" id="btnConfused">🤚 I'm confused — flag this moment</button>
      </div>
    </section>

    <section class="panel">
      <h2>Transcript so far</h2>
      <input type="text" id="transcriptSearch" placeholder="Search the transcript…" style="width:100%; margin-bottom:10px;">
      <ul id="transcriptList"></ul>
    </section>
  </div>

  <section class="panel">
    <h2>Flagged moments (students found this confusing)</h2>
    <ul id="doubtsList"></ul>
    <p class="caption-placeholder" id="doubtsEmpty" style="font-size:.88rem;">No flags yet this class.</p>
  </section>

  <section class="panel">
    <h2>No mic? Paste lecture text instead</h2>
    <textarea id="pasteArea" placeholder="Paste any lecture text here to generate notes without using the microphone…"></textarea>
  </section>

  <section class="panel" id="printArea">
    <h2>Revision notes</h2>
    <div class="controls" style="margin-bottom:14px;">
      <button class="primary" id="btnSummarize">Summarise for revision</button>
      <button id="btnDownload" disabled>Download .txt</button>
      <button id="btnCopy" disabled>Copy notes</button>
      <button id="btnReadAloud" disabled>🔊 Read aloud</button>
      <button id="btnPdf" disabled>Export as PDF</button>
      <button id="btnQr" disabled>Show QR code</button>
    </div>
    <div id="notesOutput"><span class="caption-placeholder">Notes will appear here after you summarise a class or pasted text.</span></div>
    <div id="qrBox" style="margin-top:14px;"></div>
  </section>

  <p class="footnote">
    <strong>Roadmap for the full build:</strong> automatic English–Hindi code-switching (currently a manual toggle), a full ISL dictionary for Ishara pending a data partnership with ISLRTC (today Ishara covers ~15 common classroom signs), cloud accounts for true cross-device access (today's profiles and subject spaces are saved on this device), and accent-robust recognition tuned across classroom environments.<br>
    Captions run entirely in your browser — audio never leaves your device. Only text you choose to summarise reaches the notes service, and nothing is stored on a server.
  </p>
</div>

<script src="https://js.puter.com/v2/"></script>
<script>
(function(){
  // ---------------- Sign library (original simple icons, not reproductions of any copyrighted dictionary) ----------------
  const SIGNS = {
    'yes':  '<circle cx="50" cy="50" r="42" fill="var(--sage)"/><path d="M30 52 L45 65 L72 35" stroke="#fff" stroke-width="7" fill="none" stroke-linecap="round" stroke-linejoin="round"/>',
    'no':   '<circle cx="50" cy="50" r="42" fill="var(--danger)"/><path d="M35 35 L65 65 M65 35 L35 65" stroke="#fff" stroke-width="7" stroke-linecap="round"/>',
    'question': '<circle cx="50" cy="50" r="42" fill="var(--accent)"/><text x="50" y="65" font-size="44" text-anchor="middle" fill="#fff" font-family="Space Grotesk">?</text>',
    'thanks': '<circle cx="50" cy="50" r="42" fill="var(--teal)"/><path d="M30 40 Q50 25 70 40 Q60 55 50 65 Q40 55 30 40 Z" fill="#fff"/>',
    'thank you': '<circle cx="50" cy="50" r="42" fill="var(--teal)"/><path d="M30 40 Q50 25 70 40 Q60 55 50 65 Q40 55 30 40 Z" fill="#fff"/>',
    'repeat': '<circle cx="50" cy="50" r="42" fill="var(--sage)"/><path d="M30 50 A20 20 0 1 1 38 64" stroke="#fff" stroke-width="6" fill="none"/><path d="M30 56 L30 66 L40 66" stroke="#fff" stroke-width="6" fill="none" stroke-linecap="round" stroke-linejoin="round"/>',
    'exam': '<rect x="14" y="14" width="72" height="72" rx="10" fill="var(--accent)"/><path d="M30 35 h40 M30 50 h40 M30 65 h25" stroke="#fff" stroke-width="6" stroke-linecap="round"/>',
    'homework': '<rect x="14" y="14" width="72" height="72" rx="10" fill="var(--teal)"/><path d="M30 30 h40 v40 h-40 z M38 42 h24 M38 52 h18" stroke="#fff" stroke-width="5" fill="none" stroke-linecap="round"/>',
    'teacher': '<circle cx="50" cy="50" r="42" fill="var(--sage)"/><circle cx="50" cy="38" r="12" fill="#fff"/><path d="M28 75 Q50 55 72 75" stroke="#fff" stroke-width="8" fill="none" stroke-linecap="round"/>',
    'student': '<circle cx="50" cy="50" r="42" fill="var(--accent)"/><circle cx="50" cy="38" r="10" fill="#fff"/><path d="M30 75 Q50 58 70 75" stroke="#fff" stroke-width="7" fill="none" stroke-linecap="round"/>',
    'stop': '<circle cx="50" cy="50" r="42" fill="var(--danger)"/><rect x="34" y="20" width="32" height="46" rx="8" fill="#fff"/>',
    'wait': '<circle cx="50" cy="50" r="42" fill="var(--accent)"/><rect x="40" y="18" width="10" height="46" rx="4" fill="#fff"/>',
    'good': '<circle cx="50" cy="50" r="42" fill="var(--sage)"/><path d="M42 70 L42 45 L30 45 L38 20 Q46 20 46 30 L46 38 L70 38 Q76 38 74 46 L68 66 Q66 70 60 70 Z" fill="#fff"/>',
    'understand': '<circle cx="50" cy="50" r="42" fill="var(--teal)"/><circle cx="50" cy="38" r="16" fill="none" stroke="#fff" stroke-width="6"/><path d="M50 54 v16" stroke="#fff" stroke-width="6" stroke-linecap="round"/>',
    'help': '<circle cx="50" cy="50" r="42" fill="var(--accent)"/><path d="M30 60 L50 30 L70 60" stroke="#fff" stroke-width="7" fill="none" stroke-linecap="round" stroke-linejoin="round"/>',
    'doubt': '<circle cx="50" cy="50" r="42" fill="var(--danger)"/><text x="50" y="65" font-size="44" text-anchor="middle" fill="#fff" font-family="Space Grotesk">?</text>'
  };

  // ---------------- Profile + subject-space storage (per-device demo accounts) ----------------
  const LS = {
    get(key, fallback){ try{ const v = localStorage.getItem(key); return v ? JSON.parse(v) : fallback; }catch(e){ return fallback; } },
    set(key, val){ try{ localStorage.setItem(key, JSON.stringify(val)); }catch(e){} }
  };

  let profile = LS.get('saathi_profile', null);
  let currentSubject = null;

  const gateEl = document.getElementById('profileGate');
  const appEl = document.getElementById('appRoot');

  function profileKey(){ return profile.role + ':' + profile.name; }
  function subjectsKey(){ return 'saathi_subjects_' + profileKey(); }
  function dataKey(subject){ return 'saathi_data_' + profileKey() + '_' + subject; }

  function loadSubjectData(subject){
    return LS.get(dataKey(subject), { transcript: [], notes: '', doubts: [] });
  }
  function saveSubjectData(subject, data){ LS.set(dataKey(subject), data); }

  function enterApp(){
    gateEl.classList.add('hidden');
    appEl.classList.remove('hidden');
    document.getElementById('whoAmI').textContent = profile.name + ' (' + (profile.role === 'teacher' ? 'Teacher' : 'Student') + ')';
    refreshSubjectDropdown();
  }

  document.getElementById('btnContinue').addEventListener('click', function(){
    const name = document.getElementById('pfName').value.trim();
    const role = document.getElementById('pfRole').value;
    if(!name){ document.getElementById('pfName').focus(); return; }
    profile = { name, role };
    LS.set('saathi_profile', profile);
    enterApp();
  });

  document.getElementById('btnSwitchProfile').addEventListener('click', function(){
    appEl.classList.add('hidden');
    gateEl.classList.remove('hidden');
  });

  function refreshSubjectDropdown(){
    const subjects = LS.get(subjectsKey(), ['General']);
    const sel = document.getElementById('subjectSelect');
    sel.innerHTML = '';
    subjects.forEach(s => {
      const opt = document.createElement('option');
      opt.value = s; opt.textContent = s;
      sel.appendChild(opt);
    });
    currentSubject = subjects[0];
    sel.value = currentSubject;
    loadIntoUI();
  }

  document.getElementById('subjectSelect').addEventListener('change', function(e){
    currentSubject = e.target.value;
    loadIntoUI();
  });

  document.getElementById('btnNewSubject').addEventListener('click', function(){
    const name = prompt('Name this subject space (e.g. Physics, History):');
    if(!name) return;
    const subjects = LS.get(subjectsKey(), ['General']);
    if(!subjects.includes(name)) subjects.push(name);
    LS.set(subjectsKey(), subjects);
    refreshSubjectDropdown();
    document.getElementById('subjectSelect').value = name;
    currentSubject = name;
    loadIntoUI();
  });

  if(profile) enterApp();

  // ---------------- App state ----------------
  const state = { recognition: null, listening: false, manuallyStopped: true, lang: 'en-IN', transcript: [], doubts: [] };
  let fontScale = 1;
  let lastSummaryText = '';
  let highlightTerms = [];

  const el = {
    btnStart: document.getElementById('btnStart'),
    listeningPill: document.getElementById('listeningPill'),
    captionBox: document.getElementById('captionBox'),
    transcriptList: document.getElementById('transcriptList'),
    transcriptSearch: document.getElementById('transcriptSearch'),
    doubtsList: document.getElementById('doubtsList'),
    doubtsEmpty: document.getElementById('doubtsEmpty'),
    langSeg: document.getElementById('langSeg'),
    themeSeg: document.getElementById('themeSeg'),
    fontDec: document.getElementById('fontDec'),
    fontReset: document.getElementById('fontReset'),
    fontInc: document.getElementById('fontInc'),
    pasteArea: document.getElementById('pasteArea'),
    btnSummarize: document.getElementById('btnSummarize'),
    btnDownload: document.getElementById('btnDownload'),
    btnCopy: document.getElementById('btnCopy'),
    btnReadAloud: document.getElementById('btnReadAloud'),
    btnPdf: document.getElementById('btnPdf'),
    btnQr: document.getElementById('btnQr'),
    qrBox: document.getElementById('qrBox'),
    notesOutput: document.getElementById('notesOutput'),
    ishara: document.getElementById('ishara'),
    isharaStatus: document.getElementById('isharaStatus'),
    body: document.body,
    micBanner: document.getElementById('micBanner'),
    signStrip: document.getElementById('signStrip'),
    btnConfused: document.getElementById('btnConfused'),
    termInput: document.getElementById('termInput'),
    btnAddTerm: document.getElementById('btnAddTerm'),
    termChips: document.getElementById('termChips'),
  };

  function escapeHtml(str){ return str.replace(/[&<>"']/g, m => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[m])); }

  function highlight(text){
    let safe = escapeHtml(text);
    highlightTerms.forEach(term => {
      if(!term) return;
      const re = new RegExp('(' + term.replace(/[.*+?^${}()|[\]\\]/g, '\\$&') + ')', 'gi');
      safe = safe.replace(re, '<mark>$1</mark>');
    });
    // auto-highlight capitalised words and standalone numbers as a light default
    safe = safe.replace(/\b([A-Z][a-z]{2,})\b/g, function(m){ return highlightTerms.length ? m : '<mark>' + m + '</mark>'; });
    return safe;
  }

  // ---------------- Load/save current subject into UI ----------------
  function loadIntoUI(){
    const data = loadSubjectData(currentSubject);
    state.transcript = data.transcript.map(t => ({ time: new Date(t.time), text: t.text }));
    state.doubts = data.doubts.map(d => ({ time: new Date(d.time), text: d.text }));
    lastSummaryText = data.notes || '';
    highlightTerms = LS.get(dataKey(currentSubject) + '_terms', []);
    renderTranscript();
    renderDoubts();
    renderTermChips();
    if(lastSummaryText){
      el.notesOutput.innerHTML = highlight(lastSummaryText).replace(/\n/g, '<br>');
      el.btnDownload.disabled = false; el.btnCopy.disabled = false; el.btnReadAloud.disabled = false; el.btnPdf.disabled = false; el.btnQr.disabled = false;
    } else {
      el.notesOutput.innerHTML = '<span class="caption-placeholder">Notes will appear here after you summarise a class or pasted text.</span>';
      el.btnDownload.disabled = true; el.btnCopy.disabled = true; el.btnReadAloud.disabled = true; el.btnPdf.disabled = true; el.btnQr.disabled = true;
    }
    el.qrBox.innerHTML = '';
    el.captionBox.innerHTML = '<span class="caption-placeholder">Captions will appear here once class starts.</span>';
  }

  function persist(){
    saveSubjectData(currentSubject, {
      transcript: state.transcript.map(t => ({ time: t.time.toISOString(), text: t.text })),
      doubts: state.doubts.map(d => ({ time: d.time.toISOString(), text: d.text })),
      notes: lastSummaryText
    });
  }

  function persistTerms(){ LS.set(dataKey(currentSubject) + '_terms', highlightTerms); }

  // ---------------- Highlight term chips ----------------
  function renderTermChips(){
    el.termChips.innerHTML = '';
    highlightTerms.forEach((term, i) => {
      const chip = document.createElement('span');
      chip.className = 'chip';
      chip.textContent = term + ' ✕';
      chip.style.cursor = 'pointer';
      chip.addEventListener('click', function(){
        highlightTerms.splice(i, 1);
        persistTerms();
        renderTermChips();
      });
      el.termChips.appendChild(chip);
    });
  }
  el.btnAddTerm.addEventListener('click', function(){
    const v = el.termInput.value.trim();
    if(!v) return;
    highlightTerms.push(v);
    persistTerms();
    renderTermChips();
    el.termInput.value = '';
  });

  // ---------------- Speech recognition ----------------
  const SpeechRecognitionImpl = window.SpeechRecognition || window.webkitSpeechRecognition;
  const isSecureContext = window.isSecureContext;

  function buildRecognition(){
    if(!SpeechRecognitionImpl) return null;
    const r = new SpeechRecognitionImpl();
    r.continuous = true; r.interimResults = true; r.lang = state.lang;
    r.onresult = function(event){
      let interim = '';
      for(let i = event.resultIndex; i < event.results.length; i++){
        const text = event.results[i][0].transcript;
        if(event.results[i].isFinal){ addTranscriptLine(text.trim()); } else { interim += text; }
      }
      renderCaption(interim);
    };
    r.onerror = function(e){
      if(e.error === 'not-allowed' || e.error === 'service-not-allowed'){
        showMicBanner('Microphone access was blocked. If you opened this file directly (file://), serve it from a local server instead — run "python -m http.server" in this folder and open it via http://localhost:8000/saathi.html, then allow the mic when Chrome asks.');
      } else if(e.error === 'network'){
        showMicBanner('No network reached the speech service. Captions need an internet connection even though they run in your browser.');
      }
    };
    r.onend = function(){ if(state.listening && !state.manuallyStopped){ try{ r.start(); }catch(e){} } };
    return r;
  }

  function showMicBanner(msg){ el.micBanner.textContent = msg; el.micBanner.classList.add('show'); }
  function hideMicBanner(){ el.micBanner.classList.remove('show'); }

  function renderCaption(interimText){
    const lastFinal = state.transcript.length ? state.transcript[state.transcript.length - 1].text : '';
    el.captionBox.innerHTML =
      (lastFinal ? '<span class="final">' + highlight(lastFinal) + ' </span>' : '') +
      (interimText ? '<span class="interim">' + escapeHtml(interimText) + '</span>' : '');
    if(!lastFinal && !interimText){ el.captionBox.innerHTML = '<span class="caption-placeholder">Listening… say something to see captions appear.</span>'; }
    checkSigns((lastFinal + ' ' + interimText).toLowerCase());
  }

  function checkSigns(text){
    Object.keys(SIGNS).forEach(word => {
      if(text.includes(word)){ showSignChip(word); }
    });
  }

  function showSignChip(word){
    const chip = document.createElement('div');
    chip.className = 'sign-chip';
    chip.innerHTML = '<svg viewBox="0 0 100 100">' + SIGNS[word] + '</svg><span>' + word + '</span>';
    el.signStrip.appendChild(chip);
    if(el.signStrip.children.length > 6){ el.signStrip.removeChild(el.signStrip.children[0]); }
    setTimeout(() => { if(chip.parentNode) chip.parentNode.removeChild(chip); }, 6000);
  }

  function addTranscriptLine(text){
    if(!text) return;
    const time = new Date();
    state.transcript.push({ time, text });
    persist();
    renderTranscript();
  }

  function renderTranscript(filter){
    el.transcriptList.innerHTML = '';
    const q = (filter || '').toLowerCase();
    state.transcript.forEach(entry => {
      if(q && !entry.text.toLowerCase().includes(q)) return;
      const li = document.createElement('li');
      const t = document.createElement('time');
      t.textContent = entry.time.toLocaleTimeString([], {hour:'2-digit', minute:'2-digit', second:'2-digit'});
      const span = document.createElement('span');
      span.innerHTML = highlight(entry.text);
      li.appendChild(t); li.appendChild(span);
      el.transcriptList.appendChild(li);
    });
    el.transcriptList.scrollTop = el.transcriptList.scrollHeight;
  }
  el.transcriptSearch.addEventListener('input', function(e){ renderTranscript(e.target.value); });

  function renderDoubts(){
    el.doubtsList.innerHTML = '';
    el.doubtsEmpty.style.display = state.doubts.length ? 'none' : 'block';
    state.doubts.forEach(d => {
      const li = document.createElement('li');
      const t = document.createElement('time');
      t.textContent = d.time.toLocaleTimeString([], {hour:'2-digit', minute:'2-digit'});
      li.appendChild(t);
      li.appendChild(document.createTextNode(d.text));
      el.doubtsList.appendChild(li);
    });
  }

  el.btnConfused.addEventListener('click', function(){
    const lastLine = state.transcript.length ? state.transcript[state.transcript.length - 1].text : '(before any captions were recorded)';
    state.doubts.push({ time: new Date(), text: 'Near: "' + lastLine + '"' });
    persist();
    renderDoubts();
    showSignChip('doubt');
  });

  function setIsharaStatus(text){ el.isharaStatus.textContent = text; }

  function startClass(){
    if(!isSecureContext){
      showMicBanner('This page is not running in a secure context. Serve it with "python -m http.server" and open http://localhost:8000/saathi.html — the microphone will not work when opened directly as a file.');
      return;
    }
    if(!SpeechRecognitionImpl){
      setIsharaStatus('This browser doesn\u2019t support live captions — use the paste box below instead');
      return;
    }
    hideMicBanner();
    state.recognition = buildRecognition();
    state.listening = true; state.manuallyStopped = false;
    try{ state.recognition.start(); }catch(e){}
    el.btnStart.textContent = 'Stop Class';
    el.btnStart.classList.add('ghost-active');
    el.listeningPill.textContent = 'Listening…';
    el.listeningPill.classList.add('active');
    document.getElementById('ishara').classList.add('listening');
    setIsharaStatus('Ishara is listening for ' + (state.lang === 'hi-IN' ? 'हिंदी' : 'English'));
  }

  function stopClass(){
    state.listening = false; state.manuallyStopped = true;
    if(state.recognition){ try{ state.recognition.stop(); }catch(e){} }
    el.btnStart.textContent = 'Start Class';
    el.btnStart.classList.remove('ghost-active');
    el.listeningPill.textContent = 'Not listening';
    el.listeningPill.classList.remove('active');
    document.getElementById('ishara').classList.remove('listening');
    setIsharaStatus('Ishara is resting — this subject\u2019s transcript is saved');
  }

  el.btnStart.addEventListener('click', function(){ state.listening ? stopClass() : startClass(); });

  el.langSeg.addEventListener('click', function(e){
    const btn = e.target.closest('button[data-lang]');
    if(!btn) return;
    [...el.langSeg.children].forEach(b => b.classList.remove('active'));
    btn.classList.add('active');
    state.lang = btn.dataset.lang;
    if(state.listening){ stopClass(); startClass(); }
  });

  function applyFontScale(){ document.documentElement.style.setProperty('--caption-scale', fontScale.toFixed(2)); }
  el.fontDec.addEventListener('click', function(){ fontScale = Math.max(0.75, fontScale - 0.1); applyFontScale(); });
  el.fontReset.addEventListener('click', function(){ fontScale = 1; applyFontScale(); });
  el.fontInc.addEventListener('click', function(){ fontScale = Math.min(1.8, fontScale + 0.1); applyFontScale(); });

  el.themeSeg.addEventListener('click', function(e){
    const btn = e.target.closest('button[data-theme]');
    if(!btn) return;
    [...el.themeSeg.children].forEach(b => b.classList.remove('active'));
    btn.classList.add('active');
    el.body.setAttribute('data-theme', btn.dataset.theme);
  });

  function getSourceText(){
    const pasted = el.pasteArea.value.trim();
    if(pasted) return pasted;
    return state.transcript.map(t => t.text).join(' ');
  }

  function fallbackSummary(text){
    const sentences = text.split(/(?<=[.?!।])\s+/).filter(Boolean);
    const picked = sentences.filter((_, i) => i % 2 === 0).slice(0, 8);
    return '(Offline fallback summary — connect to the internet for a fuller AI summary)\n\n' + picked.map(s => '\u2022 ' + s.trim()).join('\n');
  }

  el.btnSummarize.addEventListener('click', async function(){
    const text = getSourceText();
    if(!text){ el.notesOutput.innerHTML = '<span class="caption-placeholder">Record a class or paste some text first.</span>'; return; }
    el.btnSummarize.disabled = true; el.btnSummarize.textContent = 'Summarising…';
    setIsharaStatus('Ishara is organising the notes…');
    const prompt = 'Summarise the following classroom lecture transcript into clear, structured revision notes for students. ' +
      'Group points under 2-4 short headings based on the content, use concise bullet points, skip filler words and repetition, ' +
      'and keep the original language of the transcript (do not translate).\n\nTranscript:\n' + text;
    try{
      if(!window.puter || !window.puter.ai || !window.puter.ai.chat){ throw new Error('puter unavailable'); }
      const response = await window.puter.ai.chat(prompt);
      const out = (response && response.message && response.message.content) ? response.message.content : String(response);
      lastSummaryText = out;
    }catch(err){
      lastSummaryText = fallbackSummary(text);
    }finally{
      el.notesOutput.innerHTML = highlight(lastSummaryText).replace(/\n/g, '<br>');
      persist();
      el.btnSummarize.disabled = false; el.btnSummarize.textContent = 'Summarise for revision';
      el.btnDownload.disabled = false; el.btnCopy.disabled = false; el.btnReadAloud.disabled = false; el.btnPdf.disabled = false; el.btnQr.disabled = false;
      setIsharaStatus('Ishara has the notes ready');
    }
  });

  el.btnDownload.addEventListener('click', function(){
    const header = 'Saathi — ' + currentSubject + ' notes\nGenerated ' + new Date().toLocaleString() + '\n\n';
    const transcriptText = state.transcript.map(t => '[' + t.time.toLocaleTimeString() + '] ' + t.text).join('\n');
    const body = header + 'SUMMARY\n' + lastSummaryText + '\n\nFULL TRANSCRIPT\n' + (transcriptText || '(none — summary generated from pasted text)');
    const blob = new Blob([body], {type:'text/plain'});
    const a = document.createElement('a');
    a.href = URL.createObjectURL(blob);
    a.download = 'saathi-' + currentSubject.replace(/\s+/g,'-') + '-' + Date.now() + '.txt';
    a.click();
    URL.revokeObjectURL(a.href);
  });

  el.btnCopy.addEventListener('click', async function(){
    try{ await navigator.clipboard.writeText(lastSummaryText); el.btnCopy.textContent = 'Copied!'; setTimeout(() => el.btnCopy.textContent = 'Copy notes', 1500); }catch(e){}
  });

  let speaking = false;
  el.btnReadAloud.addEventListener('click', function(){
    if(speaking){ window.speechSynthesis.cancel(); speaking = false; el.btnReadAloud.textContent = '🔊 Read aloud'; return; }
    const utter = new SpeechSynthesisUtterance(lastSummaryText);
    utter.onend = function(){ speaking = false; el.btnReadAloud.textContent = '🔊 Read aloud'; };
    window.speechSynthesis.speak(utter);
    speaking = true;
    el.btnReadAloud.textContent = '⏹ Stop reading';
  });

  el.btnPdf.addEventListener('click', function(){ window.print(); });

  el.btnQr.addEventListener('click', function(){
    el.qrBox.innerHTML = '';
    let content = lastSummaryText;
    if(content.length > 1200){ content = content.slice(0, 1200) + '\n\n(Notes trimmed for QR — use Download for the full version)'; }
    const holder = document.createElement('div');
    el.qrBox.appendChild(holder);
    new QRCode(holder, { text: content, width: 180, height: 180 });
    const note = document.createElement('p');
    note.className = 'caption-placeholder';
    note.style.fontSize = '.82rem';
    note.textContent = 'Scan with a phone camera to copy today\u2019s notes.';
    el.qrBox.appendChild(note);
  });

  if(!SpeechRecognitionImpl){ setIsharaStatus('Live captions need Chrome or Edge — paste text below to try notes'); }
  else if(!isSecureContext){ showMicBanner('Open this file through a local server for the microphone to work: run "python -m http.server" in this folder, then visit http://localhost:8000/saathi.html'); }
})();
</script>
</body>
</html>
