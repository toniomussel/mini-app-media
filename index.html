<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no" />
  <title>Media e Società Digitale - Hub UniCal</title>
  <script src="https://telegram.org/js/telegram-web-app.js"></script>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet" />
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap');
    body {
      font-family: 'Plus Jakarta Sans', sans-serif;
      background-color: #0b0f17;
      color: #f3f4f6;
      -webkit-tap-highlight-color: transparent;
      user-select: none;
    }
    .glass-card {
      background: rgba(22, 27, 38, 0.85);
      backdrop-filter: blur(16px);
      border: 1px solid rgba(255, 255, 255, 0.08);
    }
    .bottom-nav-item.active {
      color: #ec4899;
    }
    .bottom-nav-item.active i {
      transform: translateY(-2px);
    }
  </style>
</head>
<body class="pb-24 pt-3 px-3 max-w-md mx-auto min-h-screen flex flex-col justify-between">

  <!-- HEADER BRAND E MODALITÀ EDITOR -->
  <header class="glass-card rounded-2xl p-4 mb-4 relative overflow-hidden">
    <div class="absolute -top-10 -right-10 w-28 h-28 bg-pink-500/20 rounded-full blur-2xl"></div>
    <div class="absolute -bottom-10 -left-10 w-28 h-28 bg-amber-500/10 rounded-full blur-2xl"></div>
    
    <!-- TOGGLE MODALITÀ MODIFICA -->
    <div class="flex justify-between items-center mb-3 text-xs border-b border-slate-800 pb-2">
      <span class="text-slate-400 font-medium">Stato App: <strong id="mode-status" class="text-slate-200">Vista Utente</strong></span>
      <button onclick="toggleEditMode()" id="toggle-edit-btn" class="px-2.5 py-1 bg-slate-800 border border-slate-700 rounded-lg text-slate-300 font-semibold flex items-center gap-1.5 hover:border-pink-500/50 transition-all">
        <i class="fa-solid fa-pen-to-square text-pink-400"></i>
        <span id="toggle-edit-text">Modifica</span>
      </button>
    </div>

    <div class="relative z-10 flex flex-col items-center text-center">
      <div class="w-20 h-20 rounded-full p-1 bg-gradient-to-tr from-pink-500 to-amber-400 mb-2 shadow-lg shadow-pink-500/20">
        <div class="w-full h-full bg-slate-900 rounded-full flex items-center justify-center p-1 overflow-hidden">
          <i class="fa-solid fa-graduation-cap text-3xl text-pink-400"></i>
        </div>
      </div>
      <h1 class="text-lg font-extrabold tracking-tight">MEDIA E SOCIETÀ DIGITALE</h1>
      <p class="text-xs text-slate-400 font-medium">Università della Calabria • DiSPeS</p>
    </div>
  </header>

  <!-- BANNER NOTIZIE DILIGENZA -->
  <div id="banner-container" class="mb-4"></div>

  <!-- SEZIONE PRINCIPALE DINAMICA -->
  <main id="main-content" class="space-y-4">
    <!-- Contenuto iniettato via JS -->
  </main>

  <!-- MODALE GENERICO (Aggiunta / Modifica) -->
  <div id="modal" class="fixed inset-0 bg-black/80 backdrop-blur-md z-50 hidden flex items-center justify-center p-4">
    <div class="glass-card rounded-2xl p-5 w-full max-w-sm border-pink-500/30 max-h-[90vh] overflow-y-auto shadow-2xl">
      <div class="flex justify-between items-center mb-4">
        <h3 id="modal-title" class="text-base font-bold text-pink-400">Aggiungi / Modifica</h3>
        <button onclick="closeModal()" class="text-slate-400 hover:text-white"><i class="fa-solid fa-xmark text-lg"></i></button>
      </div>
      <div id="modal-body" class="space-y-3">
        <!-- Form inserito dinamicamente -->
      </div>
    </div>
  </div>

  <!-- NAVIGATION BAR INFERIORE -->
  <nav class="fixed bottom-0 left-0 right-0 z-40 bg-slate-950/90 backdrop-blur-xl border-t border-slate-800/80 px-2 py-2">
    <div class="max-w-md mx-auto grid grid-cols-5 text-center">
      <button onclick="switchTab('insegnamenti')" id="nav-insegnamenti" class="bottom-nav-item active flex flex-col items-center py-1 text-slate-400 transition-all">
        <i class="fa-solid fa-book-open text-lg mb-1 transition-transform"></i>
        <span class="text-[10px] font-semibold">Corsi</span>
      </button>
      <button onclick="switchTab('aule')" id="nav-aule" class="bottom-nav-item flex flex-col items-center py-1 text-slate-400 transition-all">
        <i class="fa-solid fa-location-dot text-lg mb-1 transition-transform"></i>
        <span class="text-[10px] font-semibold">Aule</span>
      </button>
      <button onclick="switchTab('servizi')" id="nav-servizi" class="bottom-nav-item flex flex-col items-center py-1 text-slate-400 transition-all">
        <i class="fa-solid fa-utensils text-lg mb-1 transition-transform"></i>
        <span class="text-[10px] font-semibold">Servizi</span>
      </button>
      <button onclick="switchTab('orari')" id="nav-orari" class="bottom-nav-item flex flex-col items-center py-1 text-slate-400 transition-all">
        <i class="fa-solid fa-calendar-days text-lg mb-1 transition-transform"></i>
        <span class="text-[10px] font-semibold">Orari</span>
      </button>
      <button onclick="switchTab('link')" id="nav-link" class="bottom-nav-item flex flex-col items-center py-1 text-slate-400 transition-all">
        <i class="fa-solid fa-users text-lg mb-1 transition-transform"></i>
        <span class="text-[10px] font-semibold">Gruppi</span>
      </button>
    </div>
  </nav>

  <script>
    // Inizializzazione Telegram WebApp & Feedback Aptico
    const tg = window.Telegram?.WebApp;
    if (tg) {
      tg.expand();
      tg.ready();
    }

    function triggerHaptic() {
      if (tg?.HapticFeedback) {
        tg.HapticFeedback.impactOccurred('light');
      }
    }

    // STATO APPLICAZIONE
    let editMode = false;
    let activeTab = 'insegnamenti';

    // DATI INIZIALI DEFAULT
    const defaultBanner = "Benvenuti nel canale e nell'App Ufficiale di Media e Società Digitale (DiSPeS - UniCal)!";

    const defaultAule = [
      { id: 1, nome: "Aula C2", cubo: "18C", piano: "Piano Terra", note: "Aule DiSPeS", link: "https://maps.app.goo.gl/unical" },
      { id: 2, nome: "Aula C1", cubo: "18C", piano: "Piano Terra", note: "Aule DiSPeS", link: "https://maps.app.goo.gl/unical" },
      { id: 3, nome: "Lab. Informatico 1", cubo: "18B", piano: "1° Piano", note: "Laboratorio per lezioni pratiche", link: "#" }
    ];

    const defaultInsegnamenti = [
      { id: 1, nome: "Sociologia dei Media e della Comunicazione", cfu: 9, docente: "Prof.ssa M. Fagiani", anno: "1° Anno", semestre: "1° Semestre", link: "https://corsi.unical.it/lt-lmcu/media-e-societa-digitale/cds/studiare/" },
      { id: 2, nome: "Culture Digitali e Social Media", cfu: 6, docente: "Prof. E. G. Parini", anno: "1° Anno", semestre: "2° Semestre", link: "https://corsi.unical.it/lt-lmcu/media-e-societa-digitale/cds/studiare/" }
    ];

    const defaultLink = [
      { id: 1, titolo: "Sito Ufficiale DiSPeS", desc: "Dipartimento Scienze Politiche e Sociali", url: "https://www.unical.it/dispes/", icona: "fa-globe" },
      { id: 2, titolo: "Instagram Community", desc: "@mediaesocietadigitale", url: "https://instagram.com/mediaesocietadigitale", icona: "fa-instagram" }
    ];

    // CARICAMENTO DA LOCALSTORAGE
    let bannerText = localStorage.getItem('app_banner') || defaultBanner;
    let aule = JSON.parse(localStorage.getItem('app_aule')) || defaultAule;
    let insegnamenti = JSON.parse(localStorage.getItem('app_insegnamenti')) || defaultInsegnamenti;
    let linkGruppi = JSON.parse(localStorage.getItem('app_link')) || defaultLink;

    // SALVATAGGIO IN LOCALSTORAGE
    function saveData() {
      localStorage.setItem('app_banner', bannerText);
      localStorage.setItem('app_aule', JSON.stringify(aule));
      localStorage.setItem('app_insegnamenti', JSON.stringify(insegnamenti));
      localStorage.setItem('app_link', JSON.stringify(linkGruppi));
    }

    function resetToDefaults() {
      if (confirm("Vuoi davvero ripristinare i dati iniziali di default?")) {
        localStorage.clear();
        bannerText = defaultBanner;
        aule = [...defaultAule];
        insegnamenti = [...defaultInsegnamenti];
        linkGruppi = [...defaultLink];
        saveData();
        renderBanner();
        switchTab(activeTab);
      }
    }

    // TOGGLE EDIT MODE
    function toggleEditMode() {
      triggerHaptic();
      editMode = !editMode;
      const status = document.getElementById('mode-status');
      const btnText = document.getElementById('toggle-edit-text');
      const btn = document.getElementById('toggle-edit-btn');

      if (editMode) {
        status.innerText = "Modalità Modifica Attiva";
        status.className = "text-pink-400 font-bold";
        btnText.innerText = "Chiudi Modifica";
        btn.classList.add('bg-pink-500/20', 'border-pink-500');
      } else {
        status.innerText = "Vista Utente";
        status.className = "text-slate-200 font-medium";
        btnText.innerText = "Modifica";
        btn.classList.remove('bg-pink-500/20', 'border-pink-500');
      }

      renderBanner();
      switchTab(activeTab);
    }

    // RENDER BANNER
    function renderBanner() {
      const container = document.getElementById('banner-container');
      container.innerHTML = `
        <div class="glass-card p-3 rounded-xl border-l-4 border-l-pink-500 relative flex justify-between items-center gap-2">
          <p class="text-xs text-slate-300 leading-snug"><i class="fa-solid fa-bullhorn text-pink-400 mr-1.5"></i>${bannerText}</p>
          ${editMode ? `
            <button onclick="editBannerModal()" class="px-2 py-1 bg-slate-800 text-pink-400 rounded-lg text-[10px] font-bold border border-slate-700 hover:border-pink-500">
              <i class="fa-solid fa-pen"></i>
            </button>
          ` : ''}
        </div>
      `;
    }

    // RENDER TAB: INSEGNAMENTI
    function renderInsegnamenti() {
      return `
        <div class="flex justify-between items-center mb-2">
          <h2 class="text-sm font-bold flex items-center gap-2"><i class="fa-solid fa-graduation-cap text-pink-400"></i> Insegnamenti ed Esami</h2>
          ${editMode ? `
            <button onclick="openAddCorsoModal()" class="px-2.5 py-1 bg-pink-500 text-white rounded-lg text-xs font-bold shadow-md shadow-pink-500/20">
              <i class="fa-solid fa-plus mr-1"></i>Nuovo Corso
            </button>
          ` : ''}
        </div>
        <p class="text-xs text-slate-400 mb-3">Elenco aggiornato dei corsi di studio con CFU e docenti.</p>
        <div class="space-y-2.5">
          ${insegnamenti.map(c => `
            <div class="glass-card p-3.5 rounded-xl border-l-4 border-l-pink-500 flex justify-between items-start gap-2">
              <div class="flex-1">
                <span class="text-[10px] font-bold text-pink-400 uppercase tracking-wider">${c.anno} •${c.semestre}</span>
                <h3 class="font-bold text-sm text-white mt-0.5">\${c.nome}</h3>
                <p class="text-xs text-slate-300 mt-1"><i class="fa-solid fa-user-tie text-slate-400 mr-1"></i>\${c.docente}</p>
                <p class="text-xs text-slate-400"><i class="fa-solid fa-award text-amber-400 mr-1"></i>\${c.cfu} CFU</p>
              </div>
              <div class="flex flex-col items-end gap-1.5">
                <a href="\${c.link}" target="_blank" class="p-2 bg-slate-800 rounded-lg text-pink-400 border border-slate-700 hover:border-pink-500">
                  <i class="fa-solid fa-arrow-up-right-from-square text-xs"></i>
                </a>
                \${editMode ? `
                  <button onclick="deleteCorso(${c.id})" class="p-1.5 bg-rose-500/10 text-rose-400 rounded-lg text-xs border border-rose-500/20 hover:bg-rose-500/20">
                    <i class="fa-solid fa-trash-can"></i>
                  </button>
                ` : ''}
              </div>
            </div>
          `).join('')}
        </div>
      `;
    }

    // RENDER TAB: AULE
    function renderAule() {
      return `
        <div class="flex justify-between items-center mb-2">
          <h2 class="text-sm font-bold flex items-center gap-2"><i class="fa-solid fa-location-dot text-pink-400"></i> Posizione Aule</h2>
          ${editMode ? `
            <button onclick="openAddAulaModal()" class="px-2.5 py-1 bg-pink-500 text-white rounded-lg text-xs font-bold shadow-md shadow-pink-500/20">
              <i class="fa-solid fa-plus mr-1"></i>Nuova Aula
            </button>
          ` : ''}
        </div>
        <p class="text-xs text-slate-400 mb-3">Trova il cubo e l'ubicazione esatta delle tue lezioni.</p>
        <div class="space-y-2">
          ${aule.map(a => `
            <div class="glass-card p-3.5 rounded-xl flex justify-between items-center gap-2">
              <div>
                <h3 class="font-bold text-sm text-pink-300">\${a.nome}</h3>
                <p class="text-xs text-slate-300"><i class="fa-solid fa-cube text-slate-400 mr-1"></i>Cubo \${a.cubo} • ${a.piano}</p>${a.note ? `<p class="text-[11px] text-slate-400 mt-0.5">${a.note}</p>` : ''}
              </div>
              <div class="flex items-center gap-2">
                \${a.link && a.link !== '#' ? `
                  <a href="${a.link}" target="_blank" class="px-2.5 py-1.5 bg-slate-800 border border-slate-700 rounded-lg text-xs font-medium text-pink-400 flex items-center gap-1 hover:border-pink-500">
                    <i class="fa-solid fa-map-pin"></i> Mappa
                  </a>
                ` : ''}
                \${editMode ? `
                  <button onclick="deleteAula(${a.id})" class="p-1.5 bg-rose-500/10 text-rose-400 rounded-lg text-xs border border-rose-500/20 hover:bg-rose-500/20">
                    <i class="fa-solid fa-trash-can"></i>
                  </button>
                ` : ''}
              </div>
            </div>
          `).join('')}
        </div>
      `;
    }

    // RENDER TAB: SERVIZI
    function renderServizi() {
      return `
        <h2 class="text-sm font-bold mb-3 flex items-center gap-2"><i class="fa-solid fa-utensils text-pink-400"></i> Servizi Studenti UniCal</h2>
        
        <!-- MENSA E PUNTI -->
        <div class="glass-card p-4 rounded-2xl mb-3 space-y-2.5 border-l-4 border-l-amber-500">
          <div class="flex items-center gap-2 border-b border-slate-800 pb-2">
            <i class="fa-solid fa-burger text-amber-400 text-lg"></i>
            <div>
              <h3 class="font-bold text-sm">Mensa Universitaria & Punti</h3>
              <p class="text-[10px] text-slate-400">Gestione tramite app Smart UniCal</p>
            </div>
          </div>
          <p class="text-xs text-slate-300 leading-relaxed">
            Per usufruire della mensa occorre generare il QR Code dall'app <strong>Smart UniCal</strong> al momento della cassa.
          </p>
          <div class="bg-slate-900/80 p-3 rounded-xl text-xs space-y-1.5 text-slate-300 border border-slate-800">
            <p><strong class="text-pink-400">Punti Pasto:</strong> Ad ogni pasto viene scalato un punteggio predefinito dalla tua fascia ISEE (Primo, Secondo, Contorno, Pane e Bevanda).</p>
            <p><strong class="text-pink-400">Mense Attive:</strong> Martensson, Campus, San Gennaro.</p>
          </div>
        </div>

        <!-- CLA LOGIN -->
        <div class="glass-card p-4 rounded-2xl flex justify-between items-center border-l-4 border-l-pink-500">
          <div>
            <h3 class="font-bold text-sm flex items-center gap-1.5"><i class="fa-solid fa-language text-pink-400"></i> CLA (Centro Linguistico)</h3>
            <p class="text-xs text-slate-400 mt-0.5">Accedi al portale CLA OLA per i corsi di lingua</p>
          </div>
          <a href="https://claola.unical.it/cla-angular/login" target="_blank" class="px-3.5 py-2 bg-pink-500 text-white rounded-xl text-xs font-bold hover:bg-pink-600 shadow-md shadow-pink-500/20">
            Accedi
          </a>
        </div>
      `;
    }

    // RENDER TAB: ORARI
    function renderOrari() {
      return `
        <h2 class="text-sm font-bold mb-2 flex items-center gap-2"><i class="fa-solid fa-calendar-days text-pink-400"></i> Orario Lezioni Ufficiale</h2>
        <p class="text-xs text-slate-400 mb-3">Consulta il calendario aggiornato delle lezioni su DiSPeS UniCal.</p>
        
        <div class="glass-card p-6 rounded-2xl text-center space-y-3.5">
          <div class="w-14 h-14 bg-pink-500/10 text-pink-400 rounded-full flex items-center justify-center mx-auto text-2xl border border-pink-500/20">
            <i class="fa-solid fa-clock"></i>
          </div>
          <div>
            <h3 class="font-bold text-sm text-white">Calendario Didattico</h3>
            <p class="text-xs text-slate-400 mt-1">Verifica eventuali variazioni di aule od orari sulla pagina del Corso di Studi.</p>
          </div>
          <a href="https://corsi.unical.it/lt-lmcu/media-e-societa-digitale/cds/studiare/orario-lezioni/" target="_blank" class="inline-block w-full py-3 bg-gradient-to-r from-pink-500 to-rose-500 text-white font-bold rounded-xl text-xs shadow-lg shadow-pink-500/25">
            Apri Orario Lezioni Ufficiale
          </a>
        </div>
      `;
    }

    // RENDER TAB: LINK & GRUPPI
    function renderLink() {
      return `
        <div class="flex justify-between items-center mb-2">
          <h2 class="text-sm font-bold flex items-center gap-2"><i class="fa-solid fa-users text-pink-400"></i> Link Utili & Gruppi</h2>
          ${editMode ? `
            <button onclick="openAddLinkModal()" class="px-2.5 py-1 bg-pink-500 text-white rounded-lg text-xs font-bold shadow-md shadow-pink-500/20">
              <i class="fa-solid fa-plus mr-1"></i>Nuovo Link
            </button>
          ` : ''}
        </div>
        <p class="text-xs text-slate-400 mb-3">Canali social e portali del Corso di Laurea e del DiSPeS.</p>

        <div class="space-y-2">
          ${linkGruppi.map(l => `
            <div class="glass-card p-3.5 rounded-xl flex items-center justify-between gap-2">
              <a href="\${l.url}" target="_blank" class="flex items-center gap-3 flex-1">
                <i class="fa-solid \${l.icona || 'fa-link'} text-pink-400 text-lg"></i>
                <div>
                  <h3 class="font-bold text-sm text-white">\${l.titolo}</h3>
                  <p class="text-xs text-slate-400">\${l.desc}</p>
                </div>
              </a>
              <div class="flex items-center gap-2">
                <a href="\${l.url}" target="_blank" class="text-slate-500 hover:text-pink-400">
                  <i class="fa-solid fa-chevron-right text-xs"></i>
                </a>
                \${editMode ? `
                  <button onclick="deleteLink(${l.id})" class="p-1.5 bg-rose-500/10 text-rose-400 rounded-lg text-xs border border-rose-500/20 hover:bg-rose-500/20">
                    <i class="fa-solid fa-trash-can"></i>
                  </button>
                ` : ''}
              </div>
            </div>
          `).join('')}
        </div>

        ${editMode ? `
          <div class="mt-6 pt-4 border-t border-slate-800 text-center">
            <button onclick="resetToDefaults()" class="px-3 py-1.5 bg-rose-500/20 text-rose-300 border border-rose-500/30 rounded-xl text-xs font-bold hover:bg-rose-500/30">
              <i class="fa-solid fa-rotate-left mr-1"></i>Ripristina Dati Iniziali
            </button>
          </div>
        ` : ''}
      `;
    }

    // GESTIONE CAMBIO TAB
    function switchTab(tab) {
      triggerHaptic();
      activeTab = tab;
      document.querySelectorAll('.bottom-nav-item').forEach(el => el.classList.remove('active', 'text-pink-400'));
      document.getElementById(`nav-${tab}`)?.classList.add('active', 'text-pink-400');

      const main = document.getElementById('main-content');
      switch (tab) {
        case 'insegnamenti': main.innerHTML = renderInsegnamenti(); break;
        case 'aule': main.innerHTML = renderAule(); break;
        case 'servizi': main.innerHTML = renderServizi(); break;
        case 'orari': main.innerHTML = renderOrari(); break;
        case 'link': main.innerHTML = renderLink(); break;
      }
    }

    // MODALI E AZIONI MODIFICA
    function openModal(title, bodyHtml) {
      document.getElementById('modal-title').innerText = title;
      document.getElementById('modal-body').innerHTML = bodyHtml;
      document.getElementById('modal').classList.remove('hidden');
    }

    function closeModal() {
      document.getElementById('modal').classList.add('hidden');
    }

    function editBannerModal() {
      const html = `
        <textarea id="banner-input" rows="3" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500">${bannerText}</textarea>
        <button onclick="saveBanner()" class="w-full py-2.5 bg-pink-500 text-white font-bold rounded-xl text-xs mt-2 shadow-lg shadow-pink-500/20">Aggiorna Banner</button>
      `;
      openModal("Modifica Banner", html);
    }

    function saveBanner() {
      const val = document.getElementById('banner-input').value;
      if (val) {
        bannerText = val;
        saveData();
        renderBanner();
        closeModal();
      }
    }

    function openAddAulaModal() {
      const html = `
        <input id="a-nome" type="text" placeholder="Nome Aula (es. Aula C1)" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <input id="a-cubo" type="text" placeholder="Cubo (es. 18C)" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <input id="a-piano" type="text" placeholder="Piano (es. Piano Terra)" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <input id="a-note" type="text" placeholder="Note / Dipartimento" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <input id="a-link" type="text" placeholder="Link Mappa (opzionale)" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <button onclick="saveAula()" class="w-full py-2.5 bg-pink-500 text-white font-bold rounded-xl text-xs mt-2">Salva Aula</button>
      `;
      openModal("Aggiungi Aula", html);
    }

    function saveAula() {
      const nome = document.getElementById('a-nome').value;
      const cubo = document.getElementById('a-cubo').value;
      const piano = document.getElementById('a-piano').value || 'Piano Terra';
      const note = document.getElementById('a-note').value;
      const link = document.getElementById('a-link').value || '#';

      if (!nome || !cubo) return alert("Inserisci Nome e Cubo!");
      aule.push({ id: Date.now(), nome, cubo, piano, note, link });
      saveData();
      closeModal();
      switchTab('aule');
    }

    function deleteAula(id) {
      aule = aule.filter(a => a.id !== id);
      saveData();
      switchTab('aule');
    }

    function openAddCorsoModal() {
      const html = `
        <input id="c-nome" type="text" placeholder="Nome Corso" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <div class="grid grid-cols-2 gap-2">
          <input id="c-cfu" type="number" placeholder="CFU (es. 9)" class="bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
          <input id="c-anno" type="text" placeholder="Anno (es. 1° Anno)" class="bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        </div>
        <input id="c-semestre" type="text" placeholder="Semestre (es. 1° Semestre)" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <input id="c-docente" type="text" placeholder="Docente" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <input id="c-link" type="text" placeholder="Link Scheda (opzionale)" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <button onclick="saveCorso()" class="w-full py-2.5 bg-pink-500 text-white font-bold rounded-xl text-xs mt-2">Salva Corso</button>
      `;
      openModal("Aggiungi Insegnamento", html);
    }

    function saveCorso() {
      const nome = document.getElementById('c-nome').value;
      const cfu = document.getElementById('c-cfu').value;
      const anno = document.getElementById('c-anno').value || '1° Anno';
      const semestre = document.getElementById('c-semestre').value || '1° Semestre';
      const docente = document.getElementById('c-docente').value || 'Da assegnare';
      const link = document.getElementById('c-link').value || 'https://corsi.unical.it/lt-lmcu/media-e-societa-digitale/cds/studiare/';

      if (!nome || !cfu) return alert("Inserisci Nome e CFU!");
      insegnamenti.push({ id: Date.now(), nome, cfu, anno, semestre, docente, link });
      saveData();
      closeModal();
      switchTab('insegnamenti');
    }

    function deleteCorso(id) {
      insegnamenti = insegnamenti.filter(c => c.id !== id);
      saveData();
      switchTab('insegnamenti');
    }

    function openAddLinkModal() {
      const html = `
        <input id="l-titolo" type="text" placeholder="Titolo Link / Gruppo" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <input id="l-desc" type="text" placeholder="Descrizione breve" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <input id="l-url" type="text" placeholder="URL (https://...)" class="w-full bg-slate-900 border border-slate-700 rounded-xl p-2.5 text-xs text-white focus:outline-none focus:border-pink-500" />
        <button onclick="saveLink()" class="w-full py-2.5 bg-pink-500 text-white font-bold rounded-xl text-xs mt-2">Salva Link</button>
      `;
      openModal("Aggiungi Link / Gruppo", html);
    }

    function saveLink() {
      const titolo = document.getElementById('l-titolo').value;
      const desc = document.getElementById('l-desc').value;
      const url = document.getElementById('l-url').value;

      if (!titolo || !url) return alert("Inserisci Titolo e URL!");
      linkGruppi.push({ id: Date.now(), titolo, desc, url, icona: 'fa-link' });
      saveData();
      closeModal();
      switchTab('link');
    }

    function deleteLink(id) {
      linkGruppi = linkGruppi.filter(l => l.id !== id);
      saveData();
      switchTab('link');
    }

    // AVVIO
    renderBanner();
    switchTab('insegnamenti');
  </script>
</body>
</html>
