<!DOCTYPE html>
<html lang="it">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Festa della Carteria 2026 — Cruscotto</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
<style>
:root {
  --rosso: #c0392b; --rosso-scuro: #96281b;
  --verde: #1a7a4a; --verde-chiaro: #e8f5ee;
  --oro: #c9902a; --oro-chiaro: #fdf3e0;
  --grigio-bg: #f5f3ef; --grigio-card: #ffffff;
  --grigio-testo: #2c2c2c; --grigio-muted: #7a7570; --bordo: #e0dbd3;
}
* { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: 'DM Sans', sans-serif; background: var(--grigio-bg); color: var(--grigio-testo); min-height: 100vh; }
header { background: var(--rosso); color: white; padding: 2rem 2.5rem 1.5rem; display: flex; align-items: flex-end; justify-content: space-between; flex-wrap: wrap; gap: 1rem; }
header h1 { font-family: 'DM Serif Display', serif; font-size: 2rem; line-height: 1.1; font-weight: 400; }
header h1 span { display: block; font-family: 'DM Sans', sans-serif; font-size: 0.8rem; font-weight: 300; letter-spacing: 0.12em; text-transform: uppercase; opacity: 0.8; margin-bottom: 4px; }
.header-right { text-align: right; font-size: 0.78rem; opacity: 0.85; line-height: 1.6; }
.btn-refresh { display: inline-flex; align-items: center; gap: 6px; margin-top: 8px; background: rgba(255,255,255,0.18); border: 1px solid rgba(255,255,255,0.4); color: white; padding: 5px 14px; border-radius: 20px; font-family: 'DM Sans', sans-serif; font-size: 0.78rem; cursor: pointer; transition: background 0.2s; }
.btn-refresh:hover { background: rgba(255,255,255,0.28); }
.btn-refresh.loading svg { animation: spin 1s linear infinite; }
@keyframes spin { to { transform: rotate(360deg); } }
main { padding: 2rem 2.5rem; max-width: 1100px; margin: 0 auto; }
.nota { background: var(--oro-chiaro); border-left: 3px solid var(--oro); border-radius: 4px; padding: 0.7rem 1rem; font-size: 0.82rem; color: #6b4c10; margin-bottom: 1.5rem; line-height: 1.5; }
.sezione-titolo { font-size: 0.72rem; font-weight: 600; letter-spacing: 0.12em; text-transform: uppercase; color: var(--grigio-muted); margin: 2rem 0 1rem; display: flex; align-items: center; gap: 8px; }
.sezione-titolo::after { content: ''; flex: 1; height: 1px; background: var(--bordo); }
.kpi-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 12px; margin-bottom: 0.5rem; }
.kpi { background: var(--grigio-card); border: 1px solid var(--bordo); border-radius: 10px; padding: 1.1rem 1.2rem; }
.kpi-label { font-size: 0.75rem; color: var(--grigio-muted); margin-bottom: 6px; font-weight: 500; }
.kpi-value { font-family: 'DM Serif Display', serif; font-size: 1.9rem; color: var(--grigio-testo); line-height: 1; margin-bottom: 5px; }
.kpi-diff { font-size: 0.78rem; font-weight: 500; }
.kpi-diff.pos { color: var(--verde); }
.kpi-diff.neg { color: var(--rosso); }
.kpi-diff.neu { color: var(--grigio-muted); }
.kpi.highlight { border-color: var(--verde); background: var(--verde-chiaro); }
.chart-card { background: var(--grigio-card); border: 1px solid var(--bordo); border-radius: 10px; padding: 1.2rem 1.4rem; margin-bottom: 1.2rem; }
.chart-title { font-size: 0.82rem; font-weight: 600; color: var(--grigio-muted); margin-bottom: 1rem; }
.legend { display: flex; gap: 18px; font-size: 0.75rem; color: var(--grigio-muted); margin-bottom: 10px; }
.legend span { display: flex; align-items: center; gap: 5px; }
.legend-dot { width: 10px; height: 10px; border-radius: 2px; display: inline-block; }
.giorni-table { width: 100%; border-collapse: collapse; font-size: 0.83rem; margin-top: 0.5rem; }
.giorni-table th { font-size: 0.72rem; font-weight: 600; letter-spacing: 0.06em; text-transform: uppercase; color: var(--grigio-muted); text-align: right; padding: 6px 10px; border-bottom: 1px solid var(--bordo); }
.giorni-table th:first-child { text-align: left; }
.giorni-table td { padding: 8px 10px; text-align: right; border-bottom: 1px solid var(--bordo); font-variant-numeric: tabular-nums; }
.giorni-table td:first-child { text-align: left; font-weight: 500; }
.giorni-table tr:last-child td { border-bottom: none; }
.giorni-table tr.totale td { font-weight: 600; background: var(--grigio-bg); border-top: 2px solid var(--bordo); }
.diff-pos { color: var(--verde); font-weight: 500; }
.diff-neg { color: var(--rosso); font-weight: 500; }
.chiusi-cell { color: var(--bordo); font-style: italic; }
.error-msg { background: #fdecea; border: 1px solid #f5c6c3; border-radius: 8px; padding: 1rem 1.2rem; color: #a0281e; font-size: 0.85rem; }
footer { text-align: center; font-size: 0.75rem; color: var(--grigio-muted); padding: 2rem; border-top: 1px solid var(--bordo); margin-top: 2rem; }
</style>
</head>
<body>
<header>
  <h1><span>Festa della</span>Carteria 2026</h1>
  <div class="header-right">
    <div>Aggiornamento: <span id="last-update">—</span></div>
    <div id="giorni-count" style="font-size:0.72rem;opacity:0.75;"></div>
    <button class="btn-refresh" id="btnRefresh" onclick="caricaDati()">
      <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="23 4 23 10 17 10"/><polyline points="1 20 1 14 7 14"/><path d="M3.51 9a9 9 0 0 1 14.85-3.36L23 10M1 14l4.64 4.36A9 9 0 0 0 20.49 15"/></svg>
      Aggiorna
    </button>
  </div>
</header>
<main><div id="contenuto"><div style="text-align:center;padding:3rem;color:var(--grigio-muted);"><div style="font-size:1.1rem;margin-bottom:0.5rem;">Caricamento dati...</div><div style="font-size:0.8rem;">Connessione a Google Sheets in corso</div></div></div></main>
<footer>Cruscotto Festa della Carteria · Dati aggiornati in tempo reale dal foglio Google Sheets</footer>

<script>
const CSV_URL = 'https://docs.google.com/spreadsheets/d/e/2PACX-1vRxvPw7GkLWP0FxkBID3tHQe1acQ94dxCM27OAuq0br29_P39VNF9GqsuUZbt3R7hFmycPk1G4Urv9H/pub?gid=2124551819&single=true&output=csv';
let chartInstances = [];

// Parser CSV robusto: gestisce \r\n e virgole dentro virgolette
function parseCSV(text) {
  const rows = [];
  const lines = text.split(/\r?\n/);
  for (const line of lines) {
    const row = [];
    let inQ = false, cell = '';
    for (let i = 0; i < line.length; i++) {
      const c = line[i];
      if (c === '"') {
        if (inQ && line[i+1] === '"') { cell += '"'; i++; }
        else inQ = !inQ;
      } else if (c === ',' && !inQ) {
        row.push(cell); cell = '';
      } else {
        cell += c;
      }
    }
    row.push(cell);
    rows.push(row);
  }
  return rows;
}

// Converte stringa formato euro italiano in numero
function num(v) {
  if (!v) return null;
  const s = v.trim();
  if (!s || s === '#REF!' || s === '#N/A' || s === '#VALUE!') return null;
  if (s.toLowerCase() === 'chiusi') return null;
  // "€ 6.498,00" → rimuovi euro e spazi → "6.498,00" → togli punti → "6498,00" → virgola→punto → "6498.00"
  let n = s.replace(/€/g, '').replace(/\s/g, '').replace(/\./g, '').replace(',', '.');
  n = n.replace(/[^\d.\-]/g, '');
  const f = parseFloat(n);
  return isNaN(f) ? null : f;
}

function fmtEuro(v) {
  if (v == null) return '—';
  return '€\u00a0' + Math.round(v).toLocaleString('it-IT');
}
function fmtEuro2(v) {
  if (v == null) return '—';
  return '€\u00a0' + v.toLocaleString('it-IT', {minimumFractionDigits:2, maximumFractionDigits:2});
}
function fmtNum(v) {
  if (v == null) return '—';
  return Math.round(v).toLocaleString('it-IT');
}
function diffStr(v, fmt) {
  if (v == null) return '—';
  return (v >= 0 ? '▲ +' : '▼ ') + fmt(Math.abs(v));
}
function diffCls(v) {
  return v == null ? '' : v >= 0 ? 'diff-pos' : 'diff-neg';
}

async function caricaDati() {
  const btn = document.getElementById('btnRefresh');
  btn.classList.add('loading');
  try {
    const res = await fetch(CSV_URL + '&nocache=' + Date.now());
    if (!res.ok) throw new Error('HTTP ' + res.status);
    const text = await res.text();
    renderDashboard(parseCSV(text));
    document.getElementById('last-update').textContent = new Date().toLocaleTimeString('it-IT');
  } catch(e) {
    document.getElementById('contenuto').innerHTML =
      '<div class="error-msg"><strong>Impossibile caricare i dati.</strong><br>Verifica la connessione o che il foglio sia ancora pubblicato sul web.<br><small>' + e.message + '</small></div>';
  }
  btn.classList.remove('loading');
}

function renderDashboard(rows) {
  // Colonne (0-indexed): 1=data, 3=inc25, 4=inc26, 11=cop25, 12=cop26, 19=sc25, 20=sc26, 23=ost25, 24=ost26
  // Dati dalla riga 9 (indice 8). Righe da saltare: intestazioni, note, righe vuote
  const SKIP = ['', 'data', 'nel 2025', 'totale'];

  const giorni = [];
  let tot25=0, tot26=0, cop25t=0, cop26t=0, ost25t=0, ost26t=0;

  for (let i = 8; i < rows.length; i++) {
    const r = rows[i];
    if (!r || r.length < 5) continue;
    const rawData = (r[1] || '').trim();
    if (!rawData) continue;
    const rd = rawData.toLowerCase();
    if (SKIP.some(s => s && rd.startsWith(s))) continue;

    const chiusi = rd.includes('chiusi') || (r[3]||'').toLowerCase().includes('chiusi');

    const inc25 = num(r[3]);
    const inc26 = num(r[4]);
    const cop25 = num(r[11]);
    const cop26 = num(r[12]);
    const sc25  = num(r[19]);
    const sc26  = num(r[20]);
    const ost25 = num(r[22]);
    const ost26 = num(r[23]);

    giorni.push({ data: rawData, chiusi, inc25, inc26, cop25, cop26, sc25, sc26, ost25, ost26,
      diffInc: (inc25!=null && inc26!=null) ? inc26-inc25 : null,
      diffCop: (cop25!=null && cop26!=null) ? cop26-cop25 : null });

    // Totali SOLO per i giorni dove esiste il dato 2026
    if (inc26 != null) {
      tot26 += inc26;
      if (inc25 != null) tot25 += inc25;
    }
    if (cop26 != null) {
      cop26t += cop26;
      if (cop25 != null) cop25t += cop25;
    }
    // Osteria: solo dove ost26 > 0 (esclude i giorni futuri con 0 inserito)
    if (ost26 != null && ost26 > 0) {
      ost26t += ost26;
      if (ost25 != null) ost25t += ost25;
    }
  }

  const diffTot  = tot26 - tot25;
  const diffCop  = cop26t - cop25t;
  const diffOst  = ost26t - ost25t;
  const sc26med  = cop26t > 0 ? tot26 / cop26t : null;
  const sc25med  = cop25t > 0 ? tot25 / cop25t : null;
  const diffSc   = (sc26med!=null && sc25med!=null) ? sc26med - sc25med : null;

  const giorniAperti = giorni.filter(g => g.inc26 != null && !g.chiusi).length;
  document.getElementById('giorni-count').textContent = giorniAperti + ' giorni con dati 2026';

  chartInstances.forEach(c => c.destroy());
  chartInstances = [];

  const C25 = '#96281b', C26 = '#1a7a4a';
  const gridCol = 'rgba(0,0,0,0.06)', textCol = '#7a7570';
  const gG = giorni.filter(g => !g.chiusi);
  const labG = gG.map(g => g.data.replace(/^(lun|mar|mer|gio|ven|sab|dom)\s+/i,'').trim());

  const legenda = `<div class="legend"><span><span class="legend-dot" style="background:${C25}"></span>2025</span><span><span class="legend-dot" style="background:${C26}"></span>2026</span></div>`;

  const scaleY_euro = { ticks: { color: textCol, font:{size:11}, callback: v => '€'+Math.round(v).toLocaleString('it-IT') }, grid: { color: gridCol } };
  const scaleY_num  = { ticks: { color: textCol, font:{size:11} }, grid: { color: gridCol } };
  const scaleX = { ticks: { color: textCol, font:{size:10}, autoSkip:false, maxRotation:45 }, grid: { color: gridCol } };

  document.getElementById('contenuto').innerHTML = `
    <div class="nota">⚠️ Nel 2025 la festa è durata una settimana in più. Tutti i confronti mostrano solo i giorni dove esistono dati 2026.</div>

    <div class="sezione-titolo">Riepilogo progressivo — stessa finestra temporale</div>
    <div class="kpi-grid">
      <div class="kpi ${diffTot>=0?'highlight':''}">
        <div class="kpi-label">Incassi 2026</div>
        <div class="kpi-value">${fmtEuro(tot26)}</div>
        <div class="kpi-diff ${diffCls(diffTot)}">${diffStr(diffTot, fmtEuro)} vs 2025</div>
      </div>
      <div class="kpi">
        <div class="kpi-label">Incassi 2025 (stesso periodo)</div>
        <div class="kpi-value">${fmtEuro(tot25)}</div>
        <div class="kpi-diff neu">periodo equivalente</div>
      </div>
      <div class="kpi ${diffCop>=0?'highlight':''}">
        <div class="kpi-label">Coperti 2026</div>
        <div class="kpi-value">${fmtNum(cop26t)}</div>
        <div class="kpi-diff ${diffCls(diffCop)}">${diffStr(diffCop, fmtNum)} vs 2025</div>
      </div>
      <div class="kpi ${diffSc!=null&&diffSc>=0?'highlight':''}">
        <div class="kpi-label">Scontrino medio 2026</div>
        <div class="kpi-value">${fmtEuro2(sc26med)}</div>
        <div class="kpi-diff ${diffCls(diffSc)}">${diffStr(diffSc, fmtEuro2)} vs 2025</div>
      </div>
      <div class="kpi ${diffOst>=0?'highlight':''}">
        <div class="kpi-label">Osteria 2026</div>
        <div class="kpi-value">${fmtEuro(ost26t)}</div>
        <div class="kpi-diff ${diffCls(diffOst)}">${diffStr(diffOst, fmtEuro)} vs 2025</div>
      </div>
    </div>

    <div class="sezione-titolo">Incassi giornalieri — cucina</div>
    <div class="chart-card">${legenda}<div style="position:relative;height:260px"><canvas id="ch1"></canvas></div></div>

    <div class="sezione-titolo">Coperti giornalieri</div>
    <div class="chart-card">${legenda}<div style="position:relative;height:230px"><canvas id="ch2"></canvas></div></div>

    <div class="sezione-titolo">Scontrino medio pro capite</div>
    <div class="chart-card">${legenda}<div style="position:relative;height:210px"><canvas id="ch3"></canvas></div></div>

    <div class="sezione-titolo">Dettaglio giornaliero</div>
    <div class="chart-card" style="overflow-x:auto">
      <table class="giorni-table">
        <thead><tr>
          <th>Giorno</th>
          <th>Incassi 2025</th><th>Incassi 2026</th><th>Diff.</th>
          <th>Coperti 2025</th><th>Coperti 2026</th><th>Diff.</th>
          <th>Scontrino 2025</th><th>Scontrino 2026</th>
        </tr></thead>
        <tbody>
          ${giorni.map(g => g.chiusi
            ? `<tr><td>${g.data}</td><td colspan="8" class="chiusi-cell" style="text-align:center">chiusi</td></tr>`
            : `<tr>
                <td>${g.data}</td>
                <td>${fmtEuro(g.inc25)}</td><td>${fmtEuro(g.inc26)}</td>
                <td class="${diffCls(g.diffInc)}">${diffStr(g.diffInc, fmtEuro)}</td>
                <td>${fmtNum(g.cop25)}</td><td>${fmtNum(g.cop26)}</td>
                <td class="${diffCls(g.diffCop)}">${diffStr(g.diffCop, fmtNum)}</td>
                <td>${fmtEuro2(g.sc25)}</td><td>${fmtEuro2(g.sc26)}</td>
              </tr>`).join('')}
          <tr class="totale">
            <td>Totale</td>
            <td>${fmtEuro(tot25)}</td><td>${fmtEuro(tot26)}</td>
            <td class="${diffCls(diffTot)}">${diffStr(diffTot, fmtEuro)}</td>
            <td>${fmtNum(cop25t)}</td><td>${fmtNum(cop26t)}</td>
            <td class="${diffCls(diffCop)}">${diffStr(diffCop, fmtNum)}</td>
            <td>${fmtEuro2(sc25med)}</td><td>${fmtEuro2(sc26med)}</td>
          </tr>
        </tbody>
      </table>
    </div>`;

  const mkBar = (id, data25, data26, scaleY) => {
    const c = new Chart(document.getElementById(id), {
      type: 'bar',
      data: { labels: labG, datasets: [
        { label:'2025', data: data25, backgroundColor: C25+'aa', borderColor: C25, borderWidth:1.5, borderRadius:3 },
        { label:'2026', data: data26, backgroundColor: C26+'aa', borderColor: C26, borderWidth:1.5, borderRadius:3 }
      ]},
      options: { responsive:true, maintainAspectRatio:false, plugins:{legend:{display:false}}, scales:{x:scaleX, y:scaleY} }
    });
    chartInstances.push(c);
  };

  mkBar('ch1', gG.map(g=>g.inc25), gG.map(g=>g.inc26), scaleY_euro);
  mkBar('ch2', gG.map(g=>g.cop25), gG.map(g=>g.cop26), scaleY_num);

  const c3 = new Chart(document.getElementById('ch3'), {
    type: 'line',
    data: { labels: labG, datasets: [
      { label:'2025', data: gG.map(g=>g.sc25), borderColor:C25, backgroundColor:'transparent', pointRadius:5, tension:0.3 },
      { label:'2026', data: gG.map(g=>g.sc26), borderColor:C26, backgroundColor:'transparent', pointRadius:5, borderDash:[5,3], tension:0.3 }
    ]},
    options: { responsive:true, maintainAspectRatio:false, plugins:{legend:{display:false}},
      scales:{ x:scaleX, y:{ ticks:{color:textCol, font:{size:11}, callback: v=>'€'+v.toFixed(2)}, grid:{color:gridCol} } } }
  });
  chartInstances.push(c3);
}

caricaDati();
</script>
</body>
</html>
