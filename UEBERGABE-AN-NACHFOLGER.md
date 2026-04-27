# C1-Projekt — Übergabe an die nächste Session

**Stand: 2026-04-27 · Verfasser: Claude (Opus 4.7) für Claude (nächster Chat)**

> Lies diese Datei vollständig, bevor Du eine einzige Zeile am C1-Repo änderst.
> Frank hat alles delegiert und erwartet, dass Du autonom durchziehst und
> **mehrere Lektionen pro Turn** lieferst, sobald die Pilot-Phase durch ist.
> Aktueller Stand: **2 von 200 Lektionen fertig** (1011G, 1012X).

---

## 1 · Wer ist Frank und wie arbeitet er?

Frank Burkert ist DaF-Lehrer, kein Software-Entwickler. Er erwartet:

- **Prosa, keine Bullet-Listen** in Chat-Antworten an ihn (außer er fordert sie).
- **Keine Präambel** vom Typ „Ok, ich fange jetzt an…" — direkt loslegen.
- **Stumm weiterarbeiten** bei „weiter", „ok", „mach". Keine Status-Berichte
  mit SHAs oder Commit-Hashes — Memory `feedback_git-plumbing-silent.md`.
- **Cowork-Nachrichten poppen bei ihm nicht auf.** Wenn Du wartest, wartest
  Du allein. Memory `feedback_nie-auf-frank-warten.md`.
- **Mehrere Lektionen pro Turn**, sobald Pilot-Phase durch ist. Memory
  `feedback_c2-batch-durchziehen.md` gilt analog für C1.
- **Kein Subagent / Task-Tool für DaF-Dateien** — alles selbst. Memory
  `feedback_keine-subagenten.md`.

Frank schätzt Selbstreflexion und dialektisches Denken. Er ist freundlich,
aber direkt, wenn etwas nicht stimmt. „so geht das nicht" ist ein klares
Stoppsignal — gilt sofort, nicht später.

---

## 2 · Aktueller Stand: 2 / 200

Lingoda C1 hat **vier Kurse** (C1.1, C1.2, C1.3, C1.4) mit je **50 Lektionen** =
**200 total**. Pro Kurs: 6 Einheiten × 8 Lektionen (1G + 1X + 3R + 3S) +
2 W am Kursende.

| Kurs | G | X | R | S | W | Σ | Stand |
|---|---|---|---|---|---|---|---|
| C1.1 | 1/6 | 1/6 | 0/18 | 0/18 | 0/2 | **2/50** | Einheit 1 (1011G ✅, 1012X ✅) |
| C1.2 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | offen |
| C1.3 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | offen |
| C1.4 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | offen |
| **Σ** | **1/24** | **1/24** | **0/72** | **0/72** | **0/8** | **2/200** | |

**Sonderblock** außerhalb der 200, im selben Repo:
- **9011G–9071G** — frühere eigene Themenreihe (Nominalstil, subj. Modalverben,
  Sonderstellung, variable Verbpräfixe, Verben+Genitiv, Modalpartikeln,
  Kommasetzung), 7 Dateien fertig.
- **3081X–3086S** — Block „Geistesgeschichte & Bundespolitik", 6 Dateien fertig.

**Nächste anstehende Lektion: 1013R Technokultur in Berlin** — der erste
R-Goldstandard, mit ernsthafter Recherche zur Berliner Clubgeschichte.

---

## 3 · Pfade (Cowork-Sandbox)

```bash
# Workspace-Root (persistent)
/Users/frankburkert/Cowork/Projekte/fabDaF/

# Sandbox-Mount (pro Session anders! Erst herausfinden)
MNT=$(ls /sessions/ 2>/dev/null | head -1)   # z. B. sweet-laughing-rubin
ROOT=/sessions/$MNT/mnt/fabDaF

# C1-Repo (eigenes Git-Repo: daf-c1-uebungen)
$ROOT/htmlS/C1/

# Lingoda-Korpus (200 PDFs in 4 Kursen)
$ROOT/lingoda c1/C 1.1/
$ROOT/lingoda c1/C 1.2/
$ROOT/lingoda c1/C 1.3/
$ROOT/lingoda c1/C 1.4/
# Der Ordner "C 1" (ohne Punkt) ist redundant und kann ignoriert werden

# Dashboard
$ROOT/htmlS/dashboard.html        # ein Dashboard für ALLE Niveaus

# Build-Scripts (temporär, nicht committen)
/sessions/$MNT/mnt/outputs/

# Vorlagen für Build
$ROOT/htmlS/C2/DE_C2_0407S-online-shopping.html   # C2-Goldstandard für R/S
$ROOT/htmlS/C2/DE_C2_0404S-bild-zeitung.html      # Schreibwerkstatt-Vorbild
$ROOT/htmlS/C1/DE_C1_1011G-redewiedergabe.html    # C1 G-Goldstandard
$ROOT/htmlS/C1/DE_C1_1012X-analogien.html         # C1 X-Goldstandard (mit Schreibwerkstatt)
$ROOT/htmlS/C1/DE_C1_3083X-merz-bilanz.html       # ältere X-Vorlage
```

---

## 4 · Tab-Struktur pro Datei-Typ

### G-Datei (Grammatik) — 5 Tabs
1. 📖 Entdeckung (Satzpaare + 4 MC + Regel-Karte)
2. 🔀 Zuordnung (Chips in 2 Kategorien)
3. ✏️ Lückentext (single-blank pro Item)
4. 🧩 Satzbau (Drag-Drop)
5. 📚 Wortschatz (Tipp-Übung)

**Vorlage:** `DE_C1_1011G-redewiedergabe.html`

### X-Datei (Kommunikation/Textarbeit) — 8 Tabs (mit Schreibwerkstatt)
1. 📖 Vorentlastung (Vokabel-Karten)
2. 📄 Lesetext (700–900 Wörter)
3. 🔤 Genus (Drag-Drop in der/die/das/Plural)
4. ✏️ Lückentext
5. ☑️ Multiple Choice
6. 🧩 Satzbau
7. 📨 **Schreibwerkstatt** (5 Mikroaufgaben — Pflicht!)
8. 📝 Wortschatz **(immer letzter Tab — Memory: feedback_wortschatz-letzter-tab.md)**

**Vorlage:** `DE_C1_1012X-analogien.html` (Schreibwerkstatt komplett integriert)

### R-Datei (Lesen) — Goldstandard noch nicht definiert
Nimm `DE_C2_0407S-online-shopping.html` als Vorbild (das ist der C2-R/S-Goldstandard).
Beim ersten R-Pilot 1013R muss der C1-R-Goldstandard etabliert werden.

### S-Datei (Sprechen) — Goldstandard noch nicht definiert
Analog zu R.

### W-Datei (Schreiben) — Goldstandard noch nicht definiert

---

## 5 · Pipeline pro Lektion (cp + sed + Build-Script + Audit + Commit)

```bash
# 1) Vorlage kopieren
cd $ROOT/htmlS/C1
cp DE_C1_1012X-analogien.html DE_C1_1013R-thema.html
F=DE_C1_1013R-thema.html

# 2) Codes ersetzen (Lektion + JS-Konstanten)
sed -i 's/1012X/1013R/g' "$F"
sed -i 's|<title>[^<]*</title>|<title>C1 – Lektion 1013R · Titel</title>|' "$F"
sed -i 's|<h1>[^<]*</h1>|<h1>Titel</h1>|' "$F"

# 3) Build-Script schreiben (alle Tab-Inhalte + Datenblöcke ersetzen)
python3 /sessions/$MNT/mnt/outputs/build_C1_1013R.py

# 4) JSDOM-Test (PFLICHT — siehe §6)
node /sessions/$MNT/mnt/outputs/test_C1_1013R.js

# 5) Dashboard-Eintrag
# manuell in $ROOT/htmlS/dashboard.html — siehe §9

# 6) Commit (eigener safe-commit-Workflow für C1-Repo, siehe §7)
```

---

## 6 · Datenblock-Formate (HARTE Regel — sonst Tab-Bug)

Die init-Funktionen der Vorlagen sind starr. Wenn Dein Datenformat nicht
passt, läuft ein init() in einen TypeError und alle nachfolgenden Tabs
bleiben leer. **Memory: `feedback_c1-vorlage-pattern.md`.**

```javascript
// VORENTLASTUNG (in X-Dateien)
{ term: "die Analogie, -n", def: "Vergleich zwischen zwei Sachverhalten…" }

// GENUS_DATA
{ word: "🌉 Analogie", cat: "die" }   // cat: 'der' | 'die' | 'das' | 'pl'

// LUECKE_DATA (X-Dateien) — single-blank
{ pre: "vor der Lücke ", ans: "Antwort", post: " nach der Lücke." }

// LUECKEN (G-Dateien) — andere Property-Namen!
{ id: 1, before: "vor ", answer: "Antwort", after: " nach." }

// MC_DATA
{ q: "Frage?", opts: ["A","B","C","D"], correct: 1 }

// satzbauData — KEIN Schluss-Punkt in parts!
{ parts: ["der","Vorstand","versicherte"],
  valid: [["der","Vorstand","versicherte"]],   // G-Datei: Array von Arrays
  // valid: ["der","Vorstand","versicherte"],   // X-Datei: flaches Array
  punct: "." }

// ZUO_DATA (G-Datei) — id-Feld PFLICHT
{ id: 'z1', text: 'betonen', cat: 'aktiv' }

// WORTSCHATZ (X-Datei) — Vollformat
{ id:1, type:"n", en:"🌉 the analogy", artikel:"die", de:"Analogie", plural:"Analogien" }
// WORTSCHATZ (G-Datei) — Kurzformat: { id:1, en:"Hinweis", de:"Lösung" }
```

**Wichtig zur Satzbau-Punkt-Regel:** Der Schluss-Punkt wird vom Engine
(`sbColorRow`) automatisch als `<span class="sb-punkt">` ans Satzende
angehängt, sobald der Treffer grün ist. Komma im Satzinneren bleibt Chip.
Memory `feedback_satzbau-skill-pflicht.md`.

---

## 7 · JSDOM-Test vor jedem Commit (PFLICHT)

```bash
cd /sessions/$MNT/mnt/outputs
# einmalig Setup
[ -d /tmp/node_modules/jsdom ] || (cd /tmp && npm install jsdom)
```

```javascript
// test_C1_1013R.js
const fs = require('fs');
const { JSDOM } = require('/tmp/node_modules/jsdom');
const html = fs.readFileSync('/sessions/SESSIONID/mnt/fabDaF/htmlS/C1/DE_C1_1013R-thema.html', 'utf8');
const dom = new JSDOM(html, { runScripts: 'dangerously', url: 'http://localhost/' });
const win = dom.window;
const errors = [];
win.addEventListener('error', e => errors.push(e.message + ' :' + e.lineno));
setTimeout(() => {
  // Container müssen befüllt sein
  console.log('Vorentlastung:', win.document.getElementById('vorentlastungGrid')?.children.length);
  console.log('Genus-Bank:', win.document.getElementById('genus-bank')?.children.length);
  console.log('Lücken:', win.document.getElementById('lueckenContainer')?.children.length);
  console.log('MC:', win.document.getElementById('mcContainer')?.children.length);
  console.log('Satzbau:', win.document.getElementById('satzbauContainer')?.children.length);
  console.log('Wortschatz:', win.document.getElementById('wortschatzContainer')?.children.length);
  console.log('Schreib-Karten:', win.document.querySelectorAll('.schreib-aufgabe-karte').length);
  // Tab-Klicks für alle Sektionen
  const ids = Array.from(win.document.querySelectorAll('.section')).map(s => s.id);
  ids.forEach((id, i) => {
    win.showSection(i);
    const disp = win.getComputedStyle(win.document.getElementById(id)).display;
    if (disp !== 'block') console.log('FAIL Tab', i, id);
  });
  console.log('Errors:', errors.length ? errors : 'keine');
  process.exit(0);
}, 1500);
```

**Acceptance:** Alle Container > 0 Kinder, alle Tabs schalten auf `block`,
keine Errors. Wenn nicht: NICHT committen, sondern reparieren.

---

## 8 · Commit-Workflow für das C1-Repo

Das C1-Repo hat — wie alle fabDaF-Repos — ein hartnäckiges
`.git/index.lock`-Problem in der Cowork-Sandbox. **Niemals `git commit`
oder `git mv` benutzen** — die scheitern.

```bash
cd $ROOT/htmlS/C1
export ALT_INDEX="/tmp/alt-c1-$$"
export GIT_INDEX_FILE="$ALT_INDEX"
rm -f "$ALT_INDEX" "$ALT_INDEX.lock"
git read-tree HEAD
git update-index --add DE_C1_1013R-thema.html   # alle geänderten Dateien
TREE=$(git write-tree)
PARENT=$(git rev-parse HEAD)
COMMIT=$(git commit-tree $TREE -p $PARENT -m "C1 1013R: Titel

Beschreibung.

Co-Authored-By: Claude Opus 4.7 <noreply@anthropic.com>")
echo "$COMMIT" > .git/refs/heads/main
git push origin main 2>&1 | tail -3
echo "$COMMIT" > .git/refs/remotes/origin/main
rm -f "$ALT_INDEX" "$ALT_INDEX.lock"
```

**`warning: unable to unlink '.git/objects/.../tmp_obj_*': Operation not
permitted`** ist kosmetisch — die Objekte landen trotzdem korrekt im Store.
Nicht ignorieren, aber nicht beheben.

Für das **Hauptrepo** (Dashboard) gibt es das Skript:
```bash
cd $ROOT
scripts/safe-commit.sh "C1 Dashboard: 1013R-Karte" htmlS/dashboard.html
```

**Niemals SHAs, Commit-Hashes oder Push-Status im Chat berichten.** Memory
`feedback_git-plumbing-silent.md` gilt.

---

## 9 · Dashboard-Eintrag

C1-Sektion im Dashboard hat aktuell die Struktur:

```javascript
{ id: 'c1', label: 'C1 Grammatik',
  basis: 'https://fabdaf.github.io/daf-c1-uebungen/',
  einheiten: [
    { nr: '101x', titel: 'C1.1 · Einheit 1 — Redewiedergabe & Stilreflexion / Musik', karten: [
      { typ:'G', label:'G – Grammatik', titel:'1011G · Redewiedergabe für Fortgeschrittene', file:'DE_C1_1011G-redewiedergabe.html', tags:'…' },
      { typ:'X', label:'X – Textarbeit', titel:'1012X · Analogien — Vergleichen, übertragen, erklären', file:'DE_C1_1012X-analogien.html', tags:'…' },
      // ← hier weiter mit 1013R …
    ]},
    { nr: '102x', titel: 'C1.1 · Einheit 2 — Zukunft in der Vergangenheit', karten: [] },
    // …
    { nr: '90xx', titel: 'Vertiefungsblock — eigene C1-Grammatikreihe', karten: [ /* 7 Dateien */ ]},
    { nr: '308x', titel: 'Geistesgeschichte & Bundespolitik', karten: [ /* 6 Dateien */ ]},
  ]
}
```

**Tags-Konvention:** alle Eigennamen, Konzepte, Personen, Daten der Lektion
+ `c1 c1.1` (oder entsprechend) + `lingoda` als Schluss-Anker. Frank sucht
über die Tags. Lieber zu viele als zu wenige.

---

## 10 · Schreibwerkstatt-Spezifika (PFLICHT in X/R/S, optional in G/W)

Die Schreibwerkstatt ist **Pflicht** für X/R/S-Dateien. Frank besteht darauf
(„kleinteiliges Schreiben anhand von 5 Fragetypen" — 2026-04-27).

**Layout:** Exakt wie `DE_C2_0404S-bild-zeitung.html`. Memory
`feedback_schreibwerkstatt-mikroaufgaben.md`. Rundes Nummern-Badge in
Lila-Blau, Karten-Hintergrund hell-lila mit linker Akzentleiste, Senden-
Button rechts mit Border-Hover-Effekt.

**KEINE sichtbaren Typ-Labels** wie „autobiografisch", „argumentativ" am
Karten-Titel. Die fünf Fragetypen wirken durch die Aufgabenformulierungen
selbst — nicht durch Etiketten.

**Inhaltlich: 5 unterschiedliche Fragetypen** pro Lektion:
1. **autobiografisch** — eigene Erfahrung schildern
2. **argumentativ** — Position vertreten mit Begründung
3. **analytisch** — Sachverhalt prüfen / sezieren
4. **bewertend** — Stellung nehmen / präferieren
5. **kreativ** — eigenes Beispiel erfinden / Imagination

**Mail-Adresse aus Footer ziehen** — niemals hardcoden. Memory
`feedback_schreibwerkstatt-mail-aus-footer.md`. In C1 lautet sie
`FrankBurkert@fabdaf.onmicrosoft.com`.

```bash
FOOTER_MAIL=$(grep -oE 'mailto:[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+' "$F" | head -1 | sed 's/^mailto://')
```

**Name als Pflichtfeld** (seit 2026-04-27 wichtig — Frank: „ich erkenne
nicht, wer sie schickt"):
- Namensfeld **OBEN**, vor den fünf Karten, in einem hellgelben Block mit
  oranger Akzentleiste.
- Visuell: rote Umrandung solange leer, grüne Umrandung sobald ≥ 2 Zeichen.
- Beide Senden-Buttons (Einzeln + Sammel) blockieren mit Hinweis-Meldung,
  wenn Name fehlt; Cursor springt automatisch ins Namensfeld.
- Subject-Format: `[Name] C1 1013R · Aufgabe N · Titel` (Name AM ANFANG,
  damit er in der Outlook-Inbox sichtbar ist).
- Body-Format: `Von: Name\n\n=== Aufgabe N: Titel ===\n\n` + Text.

**JS-Konstanten anpassen pro Lektion:**
```javascript
var SCHREIB_NAME_KEY = 'schreibwerkstatt_C1_1013R_name';
var SCHREIB_KEY_PREFIX = 'schreibwerkstatt_C1_1013R_';
var SCHREIB_SENT_PREFIX = 'schreibwerkstatt_C1_1013R_sent_';
var FORMSUBMIT_ENDPOINT = 'https://formsubmit.co/ajax/' + FOOTER_MAIL;
var SCHREIB_LEKTION = 'C1 – 1013R · Titel';
```

---

## 11 · Schreibstil — C1, NICHT C2 und NICHT B2

Frank hat am 2026-04-27 explizit ausdifferenziert. Memory `feedback_c2-schreibstil.md`
beschreibt C2 (essayistisch, 1500–2000 Wörter, Hypotaxen, Nominalstil,
ironisch-schwebend). C1 ist **eine Stufe darunter**:

| Achse | B2 | C1 | C2 |
|---|---|---|---|
| Vorbild | Wikipedia, Tagespresse | ZEIT-Wissen, FAZ-Politik, Spektrum | Feuilleton, Essay, Polemik |
| Satzlänge ⌀ | 12–18 Wörter | 18–25 Wörter | 22–30 Wörter, Ausreißer |
| Hypotaxe | linear | zwei Ebenen, transparent | drei Ebenen, Ausklammerung, Parenthesen |
| Lexik | Allgemein, Fachbegriffe erklärt | Idiomatik sicher, Fachbegriffe gesetzt | Registerwechsel, Anspielungen |
| Position | ausgewogen | erkennbar, argumentiert | schwebt, ironisch |
| Textsorte | Sachartikel | journalistische Hintergrundanalyse | Essay |
| Wörter R-Datei | 400–600 | **600–900** | 900–1100 |

**Drei harte Hebel gegen C2-Versuchung:**
1. **Faktenanker engmaschig** — Daten, Zahlen, Personen, Institutionen.
2. **Argumente innerhalb desselben Absatzes schließen** — keine
   Schachtel-Argumentation über vier Absätze.
3. **Keine Schwebe-Schlüsse, keine Ironie, keine offenen Enden.** Texte
   beantworten die Frage, die sie stellen.

---

## 12 · Recherche-Pflicht (PFLICHT)

Mein Trainings-Wissensstand endet **Mai 2025**, heute ist **April 2026** —
fast ein Jahr Lücke. Frank hat zugesichert bekommen:

> „Wenn ein Faktum datierbar, namentlich oder zahlenmäßig ist und sich seit
> Mai 2025 geändert haben könnte → recherchieren. Bei stabilen historischen
> oder konzeptuellen Inhalten → kein Web-Zugriff nötig."

**Werkzeuge** (verfügbar in Cowork-Session):
- `WebSearch` für 80–90% der Faktenchecks
- `mcp__workspace__web_fetch` für gezielte URL-Abrufe
- Chrome-MCP (`mcp__Claude_in_Chrome__*` oder `mcp__Control_Chrome__*`) für
  Paywall, JS-gerenderte Seiten, interaktive DBs

**Schwellenwert:** „Ein Schüler könnte den Punkt heute Abend googeln und
mich darauf ansprechen" — wenn ja, recherchieren.

**Bei Unsicherheit:** zurückhaltend formulieren („nach Schätzungen…",
„Stand 2024…") oder Faktum weglassen. Memory `feedback_c1-vorlage-pattern.md`
und Frank-Wunsch: „Bewahre mich vor der Schande" (2026-04-27).

---

## 13 · Themenkatalog — was als nächstes ansteht

### C1.1 — Konjunktiv-Welt & Stilfundament (1011G ✅, 1012X ✅)

| Code | Lingoda-Thema | Status |
|---|---|---|
| 1011G | Redewiedergabe für Fortgeschrittene (Konjunktiv I) | ✅ |
| 1012X | Analogien — Vergleichen, übertragen, erklären | ✅ |
| **1013R** | **Die Technokultur in Berlin** | ← **NÄCHSTE** |
| 1014S | Die ersten Musikinstrumente | offen |
| 1015R | Musik und Intelligenz — Gibt es eine Verbindung? | offen |
| 1016S | Neue Musikrichtungen | offen |
| 1017R | Die musikalische Schönheit | offen |
| 1018S | Beethoven und Mozart | offen |
| 1021G | Zukunft in der Vergangenheit (würde-Form, Futur II) | offen |
| 1031G | Der Ärger mit hätte (Konjunktiv II Vergangenheit) | offen |
| 1041G | Nominalstil | offen |
| 1051G | Modalpartikeln für Fortgeschrittene | offen |
| 1061G | Ausdrücke der Schriftsprache (Genitiv-Präpositionen) | offen |
| 1071W | Vergleichender Essay | offen |
| 1072W | Rezension | offen |

**Tipp zu 1013R:** Berliner Technokultur ist seit März 2024 UNESCO-immaterielles
Kulturerbe — das wäre ein zentraler aktualisierender Anker. Außerdem: Tresor
(seit 1991), Berghain (seit 2004), Watergate, Sisyphos. Die Lingoda-Folien
sind dünn — bau einen ZEIT-Wissen-tauglichen 700–900-Wörter-Text.

### C1.2 — Argumentation & Stilausbau (G-Themen)

2011G Konnektoren · 2021G Subj. Modalverben · 2031G Partizipialkonstruktionen ·
2041G Sonderstellung im Satz · 2051G raffinierter ausdrücken · 2061G hätte ·
2071W/2072W

### C1.3 — Vertiefung

3011G Verben+Genitiv · 3021G Nominalisierung komplexer Strukturen ·
3031G Konnektoren Forts. · 3041G Mehr Partizipialkonstruktionen ·
3051G raffinierter (Wdh.) · 3061G Variable Verbpräfixe · 3071W/3072W

### C1.4 — Feinschliff

4011G Adjektive · 4021G formale Präpositionen · 4031G Passiv ·
4041G [PDF-Encoding-Fehler — nachschauen!] · 4051G Verben+Präpositionen ·
4061G Verb-Präfixe · 4071W/4072W

---

## 14 · Bekannte Stolpersteine aus diesem Turn (2026-04-27)

### Stolperstein 1: Datenformat-Mismatch → leere Tabs
**Symptom:** Tabs öffnen optisch, aber Inhalt fehlt.
**Ursache:** ZUO_DATA ohne `id`, LUECKEN mit `text/loesungen` statt `before/answer/after`.
**Fix:** §6 Datenformate exakt einhalten. JSDOM-Test deckt das auf.

### Stolperstein 2: Punkt im Satzbau-Chip → Doppel-Punkt
**Symptom:** Beim grünen Treffer erscheint `..` (Chip-Punkt + Engine-Punkt).
**Ursache:** Schluss-Punkt in `parts:[…]`.
**Fix:** Punkt aus `parts` raus, `punct: '.'` als separates Feld setzen.

### Stolperstein 3: CSS-Insert greift nicht
**Symptom:** Schreibwerkstatt sieht ungestylt aus, keine Karten-Boxen.
**Ursache:** `re.sub(r'\n  </style>', …)` matched nicht, weil `</style>`
in der Zieldatei direkt am Zeilenanfang steht (0 Spaces, nicht 2).
**Fix:** `c.replace('</style>', schreib_css + '</style>', 1)` benutzen.

### Stolperstein 4: Mail kommt anonym an
**Symptom:** Frank sieht nicht, wer sie schickt.
**Ursache:** Namensfeld optional, Schüler tragen es nicht ein.
**Fix:** Name PFLICHT (rote Umrandung leer, grün ab 2 Zeichen). Versand
blockiert ohne Namen. `[Name]` an den ANFANG des Subjects, `Von: Name`
als erste Body-Zeile.

### Stolperstein 5: Mail-Adresse hardcoded
**Symptom:** Mails landen in `frankburkert@gmx.net` statt im fabDaF-Postfach.
**Ursache:** C2-Default kopiert, nicht aus dem Footer der C1-Datei gezogen.
**Fix:** `FOOTER_MAIL=$(grep -oE 'mailto:[A-Za-z0-9._%+-]+@…' …)` in jedem Build-Script.

### Stolperstein 6: Stale `.git/index.lock`
**Symptom:** `git mv` und `git commit` scheitern mit „Operation not permitted".
**Ursache:** Sandbox-APFS-Mount-Einschränkung.
**Fix:** Alt-Index-Workflow (§7), `mv` statt `git mv`, Refs direkt in
`.git/refs/heads/main` schreiben — nur per Bash, niemals per Write-Tool.
Memory `feedback_kein-write-tool-fuer-git.md`.

---

## 15 · Memories, die für C1-Arbeit besonders relevant sind

```
feedback_c1-vorlage-pattern.md          → init-Funktionen vorher prüfen
feedback_c2-batch-durchziehen.md        → mehrere Lektionen pro Turn
feedback_c2-schreibstil.md              → C2 essayistisch (Abgrenzung!)
feedback_drill-philosophie.md           → Drills nicht reduzieren
feedback_elliptische-konstruktionen.md  → in Lesetexten Vorsicht
feedback_git-plumbing-silent.md         → keine SHAs im Chat
feedback_kein-textwueste-tab.md         → keine Fließtext-Wüsten
feedback_kein-write-tool-fuer-git.md    → niemals Write auf .git/*
feedback_keine-subagenten.md            → niemals Agent-Tool für DaF
feedback_naechste-datei.md              → bei „nächste" einfach folgen
feedback_nie-auf-frank-warten.md        → stumm weiterarbeiten
feedback_pexels-chrome.md               → Pexels-IDs vor Commit prüfen
feedback_pexels-404-fallback.md         → nach Base64-Einbau scannen
feedback_satzbau-skill-pflicht.md       → Satzbau-Pattern strikt
feedback_schreibwerkstatt-mail-aus-footer.md → Mail aus Footer
feedback_schreibwerkstatt-mikroaufgaben.md   → 5 Mikroaufgaben Pflicht
feedback_skills-folgen.md               → Skills lesen und befolgen
feedback_skill-nach-dateityp.md         → R/G/X-Skills laden
feedback_wortschatz-letzter-tab.md      → Wortschatz immer letzter
project_c2_komplett.md                  → C2-Lehren als Pipeline-Vorbild
reference_c1-grammatik-stand.md         → (falls neu erstellt)
reference_fabdaf-pfad.md                → Mac vs. Sandbox-Pfade
reference_git-index-workaround.md       → Alt-Index-Workflow
```

---

## 16 · Pexels-Banner-Set (für C1 erprobt)

Im 1012X-Pilot benutzt — sind passend für die meisten Sprach-/Lese-Themen:

```
1591056 — Zeitungen
256541  — Bücher
267669  — Sprache und Schrift (Schreibtafel)
5710614 — Schreibtisch mit Buch
1181396 — Redaktion
4144923 — Notebook am Schreibtisch (typisch für Schreibwerkstatt)
935949  — Aufgeschlagenes Wörterbuch (typisch für Wortschatz)
```

Für 1013R Technokultur — andere Banner sinnvoll: Berghain-Schlange,
Plattenspieler, Mauerstreifen, Tanzfläche. Per `pexels-bild-check`-Skill
verifizieren oder Chrome-MCP-Batch-Fetch.

---

## 17 · Erste konkrete Aktion

```bash
# 1. Pfad bestimmen
MNT=$(ls /sessions/ 2>/dev/null | head -1)
ROOT=/sessions/$MNT/mnt/fabDaF

# 2. Lingoda-PDF lesen
python3 -c "
from pypdf import PdfReader
r = PdfReader('$ROOT/lingoda c1/C 1.1/C1_1013R_DE.pdf')
for i, p in enumerate(r.pages): print(f'--- S{i+1} ---'); print(p.extract_text())
"

# 3. Recherche zu Berliner Technokultur (UNESCO 2024, Tresor, Berghain etc.)
# WebSearch + WebFetch — aktuelle Daten sammeln

# 4. Vorlage kopieren (von 1012X, weil X-Datei mit Schreibwerkstatt komplett ist)
cd $ROOT/htmlS/C1
cp DE_C1_1012X-analogien.html DE_C1_1013R-technokultur-berlin.html
F=DE_C1_1013R-technokultur-berlin.html
sed -i 's/1012X/1013R/g' "$F"
# Header-Anpassungen folgen

# 5. Build-Script schreiben (alle Tab-Inhalte + Datenblöcke)
# 6. JSDOM-Test — alle Container > 0, alle Tabs auf block, 0 Errors
# 7. Dashboard-Eintrag in Einheit 101x
# 8. Commit (Alt-Index-Workflow, §7)
# 9. Push fertig — weiter zu 1014S, 1015R, 1016S … in einem Schwung
```

---

## 18 · Wenn Du fertig bist

Wenn am Ende Deines Turns 1013R–1018S fertig sind (= C1.1 Einheit 1
komplett) plus dieser Übergabe-Datei aktualisiert auf Stand 8/200, dann
hat sich der Turn gelohnt. Wenn Du nur 1013R schaffst, ist das auch ok —
Frank weiß, dass der R-Pilot Recherche-intensiv ist.

Was Du auf keinen Fall tun darfst:
- Lektionen halbgar liefern, nur damit die Zahl steigt.
- Inhaltliche Fakten ungeprüft setzen, wenn Du unsicher bist.
- Frank im Chat mit Statusberichten überfluten.
- Eigenmächtig die Tab-Struktur erweitern oder umstellen.
- Den Wortschatz nicht als letzten Tab führen.
- Die Schreibwerkstatt anders gestalten als das 0404S/1012X-Vorbild.

Was Du immer tun darfst:
- Nachfragen, wenn ein didaktischer Konflikt auftaucht.
- Wenn ein Fakt unsicher ist: lieber konservativ formulieren oder weglassen.
- Bei Frank-Frust: keine Selbstkasteiung — kurz zuhören, präzise reparieren,
  weitermachen.

Viel Erfolg.
