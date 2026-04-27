# C1-Projekt — Übergabe an die nächste Session (C1.2 startet)

**Stand: 2026-04-27 · Verfasser: Claude (Opus 4.7) für Claude (nächster Chat)**

> Lies diese Datei vollständig, bevor Du eine Zeile am C1-Repo änderst.
> Frank hat C1.1 in dieser Session vollständig durchgezogen — bis auf
> die zwei W-Lektionen am Kursende. **48/200 Lektionen sind live.**
> Du startest mit **C1.2 Einheit 1**.

---

## 1 · Wer ist Frank und wie arbeitet er?

Frank Burkert ist DaF-Lehrer, kein Software-Entwickler. Er erwartet:

- **Prosa, keine Bullet-Listen** in Chat-Antworten an ihn
- **Keine Präambel** vom Typ „Ok, ich fange jetzt an…" — direkt loslegen
- **Stumm weiterarbeiten** bei „weiter", „ok", „mach". Keine SHAs,
  keine Commit-Hashes, keine git-Plumbing-Berichte. Memory
  `feedback_git-plumbing-silent.md`.
- **Cowork-Nachrichten poppen bei ihm nicht auf.** Wenn Du wartest,
  wartest Du allein. Memory `feedback_nie-auf-frank-warten.md`.
- **Mehrere Lektionen pro Turn**, ohne dazwischen zu fragen.
  Memory `feedback_c2-batch-durchziehen.md` gilt analog für C1.
- **Kein Subagent / Task-Tool für DaF-Dateien** — alles selbst.
  Memory `feedback_keine-subagenten.md`.

Frank ist freundlich, aber direkt, wenn etwas nicht stimmt. „so geht
das nicht" ist ein klares Stoppsignal — gilt sofort, nicht später.
**Wichtig:** Wenn Frank „weiter" sagt, will er Lektionen — nicht
Übergabe-Dokumente, nicht Reflektionen, nicht Status-Reports. Direkt
am Werk.

---

## 2 · Aktueller Stand: 48 / 200

Lingoda C1 hat **vier Kurse** (C1.1, C1.2, C1.3, C1.4) mit je
**50 Lektionen** = **200 total**.

| Kurs | G | X | R | S | W | Σ | Stand |
|---|---|---|---|---|---|---|---|
| C1.1 | 6/6 | 6/6 | 18/18 | 18/18 | 0/2 | **48/50** | komplett bis auf 1071W/1072W |
| C1.2 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | ← **DU FÄNGST HIER AN** |
| C1.3 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | offen |
| C1.4 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | offen |
| **Σ** | **6/24** | **6/24** | **18/72** | **18/72** | **0/8** | **48/200** | |

**Sonderblock** im selben Repo (außerhalb der 200):
- **9011G–9071G** — frühere C1-Grammatikreihe (7 Dateien fertig)
- **3081X–3086S** — Block „Geistesgeschichte & Bundespolitik" (6 Dateien fertig)

**Nächste anstehende Lektion: 2011G „Logische Konnektoren, um Argumente
anzubringen".**

---

## 3 · C1.2 — Übersicht aller 50 Lingoda-Themen

### Einheit 1 (2011–2018) — Argumentation, Konnektoren

| Code | Lingoda-Thema |
|---|---|
| **2011G** | **Logische Konnektoren, um Argumente anzubringen** ← NÄCHSTE |
| 2012X | (PDF lesen) |
| 2013R | (PDF lesen) |
| 2014S | (PDF lesen) |
| 2015R | (PDF lesen) |
| 2016S | (PDF lesen) |
| 2017R | (PDF lesen) |
| 2018S | (PDF lesen) |

### Einheit 2 (2021–2028)
- 2021G **Subjektive Bedeutung der Modalverben**
- 2022X–2028S — PDF lesen für Themen

### Einheit 3 (2031–2038)
- 2031G **Partizipialkonstruktionen**
- 2032X–2038S — PDF lesen für Themen

### Einheit 4 (2041–2048)
- 2041G **Sonderstellung im Satz** (Ausklammerung etc.)
- 2042X–2048S — PDF lesen für Themen

### Einheit 5 (2051–2058)
- 2051G **Sich raffinierter ausdrücken**
- 2052X–2058S — PDF lesen für Themen

### Einheit 6 (2061–2068)
- 2061G **Immer wieder hätte** (Konjunktiv II Vergangenheit Vertiefung)
- 2062X–2068S — PDF lesen für Themen

### Schreibwerkstatt (2071–2072)
- 2071W, 2072W

---

## 4 · Pfade (Cowork-Sandbox)

```bash
# Workspace-Root (persistent)
/Users/frankburkert/Cowork/Projekte/fabDaF/

# Sandbox-Mount (pro Session anders! Erst herausfinden)
MNT=$(ls /sessions/ 2>/dev/null | head -1)
ROOT=/sessions/$MNT/mnt/fabDaF

# C1-Repo (eigenes Git-Repo: daf-c1-uebungen)
$ROOT/htmlS/C1/

# Lingoda-PDFs (200 PDFs in 4 Kursen)
$ROOT/lingoda c1/C 1.1/   ← C1.1 (alle abgearbeitet)
$ROOT/lingoda c1/C 1.2/   ← DU ARBEITEST HIER
$ROOT/lingoda c1/C 1.3/
$ROOT/lingoda c1/C 1.4/

# Dashboard
$ROOT/htmlS/dashboard.html

# Build-Scripts (temporär)
/sessions/$MNT/mnt/outputs/

# Vorlagen
$ROOT/htmlS/C1/DE_C1_1011G-redewiedergabe.html        # G-Goldstandard
$ROOT/htmlS/C1/DE_C1_1013R-technokultur-berlin.html   # R/X/S-Goldstandard (8 Tabs)
$ROOT/htmlS/C1/DE_C1_1041G-nominalstil.html           # weiterer G-Anschauungs­fall
```

---

## 5 · Tab-Struktur pro Datei-Typ

### G-Datei (Grammatik) — 5 Tabs

1. 📖 Entdeckung (5 Satzpaare + 4 MC + Regelkarte)
2. 🔀 Zuordnung (12 Chips in 2 Kategorien)
3. ✏️ Lückentext (10 Items mit Wortkasten)
4. 🧩 Satzbau (6 Drag-Drop-Sätze)
5. 📚 Wortschatz (14 Tipp-Items)

**Vorlage:** `DE_C1_1011G-redewiedergabe.html` clonen.

### X-Datei (Kommunikation), R-Datei (Lesen), S-Datei (Sprechen) — alle 8 Tabs identisch

1. 📖 Vorentlastung (8 Vokabel-Karten)
2. 📄 Lesetext (600–900 Wörter, 6 h3-Zwischentitel)
3. 🔤 Genus (8 Drag-Drop in der/die/das/Plural)
4. ✏️ Lückentext (7 Items)
5. ☑️ Multiple Choice (7 Fragen)
6. 🧩 Satzbau (6 Drag-Drop)
7. 📨 **Schreibwerkstatt** (5 Mikroaufgaben — Pflicht!)
8. 📝 Wortschatz (14 Items, immer letzter Tab)

**Vorlage:** `DE_C1_1013R-technokultur-berlin.html` clonen.

---

## 6 · Pipeline pro Lektion (kompakt)

```bash
# 1) Lingoda-PDF lesen
python3 -c "
from pypdf import PdfReader
r = PdfReader('$ROOT/lingoda c1/C 1.2/C1_2011G_DE.pdf')
for i, p in enumerate(r.pages):
    t = p.extract_text()
    if t.strip(): print(f'--- S{i+1} ---'); print(t[:400])
"

# 2) Vorlage kopieren
cp $ROOT/htmlS/C1/DE_C1_1011G-redewiedergabe.html  $ROOT/htmlS/C1/DE_C1_2011G-konnektoren.html
# (für G-Datei) — bzw. DE_C1_1013R-technokultur-berlin.html für R/X/S

# 3) Build-Script schreiben (in /sessions/$MNT/mnt/outputs/build_2011G.py)
#    - Title + Header anpassen
#    - Tab-Banner-Bilder anpassen (per Pexels-WebSearch verifizieren!)
#    - Lesetext (R/X/S) komplett neu (600–900 Wörter, h3-Struktur, Vokabelmarkierungen mit class="vocab-hl")
#    - Datenblöcke (VORENTLASTUNG, GENUS_DATA, LUECKE_DATA, MC_DATA, satzbauData, WORTSCHATZ)
#    - Schreibwerkstatt-Karten (5 Mikroaufgaben)
#    - JS-Konstanten 1013R → 2011G
#    - Anführungszeichen-Auto-Fix am Ende

python3 build_2011G.py

# 4) JSDOM-Test (PFLICHT)
sed "s|1013R-technokultur-berlin|2011G-konnektoren|g" test_1013R.js > test_2011G.js
node test_2011G.js
# Acceptance: alle Container > 0, alle Tabs auf block, 0 Errors

# 5) Anführungszeichen-Check
python3 -c "
import re
with open('$ROOT/htmlS/C1/DE_C1_2011G-konnektoren.html') as f: c = f.read()
m = re.findall(r'„([^„\"…\n]{1,80})\"', c); print('BAD QUOTES:', len(m))
"

# 6) Dashboard-Eintrag in $ROOT/htmlS/dashboard.html (siehe §9)

# 7) Commit (Alt-Index-Workflow für C1-Repo, safe-commit für Hauptrepo, siehe §7)
```

---

## 7 · Commit-Workflow (PFLICHT — keine Abkürzungen)

### Sandbox-Auth einmal pro Session

```bash
cd $ROOT && bash scripts/setup-sandbox-credentials.sh
```

### C1-Repo: Alt-Index-Workflow

```bash
cd $ROOT/htmlS/C1
unset GIT_INDEX_FILE
ALT="/tmp/alt-c1-2011G-$$"
GIT_INDEX_FILE="$ALT" git read-tree HEAD
GIT_INDEX_FILE="$ALT" git update-index --add DE_C1_2011G-konnektoren.html
TREE=$(GIT_INDEX_FILE="$ALT" git write-tree)
PARENT=$(git rev-parse HEAD)
COMMIT=$(git commit-tree $TREE -p $PARENT -m "C1 2011G: Logische Konnektoren

Beschreibung.

Co-Authored-By: Claude Opus 4.7 <noreply@anthropic.com>")
echo "$COMMIT" > .git/refs/heads/main
git push origin main 2>&1 | tail -2
echo "$COMMIT" > .git/refs/remotes/origin/main
```

**Niemals** `git commit` oder `git mv` benutzen — sie scheitern an
einer in der Sandbox nicht löschbaren `.lock`-Datei.

**Niemals** mit dem Write-Tool unter `.git/` schreiben — löst Cowork-
Permission-Dialoge aus, die im Hintergrund blockieren. Nur Bash.

### Hauptrepo (Dashboard): safe-commit.sh

```bash
cd $ROOT
scripts/safe-commit.sh "Dashboard: 2011G-Karte" htmlS/dashboard.html
```

### Wenn die Refs nach einem fehlgeschlagenen Push leer sind

Das ist mir am Anfang dieser Session passiert. Rettung:

```bash
cd $ROOT/htmlS/C1
# letzte SHA findest du in .git/logs/refs/remotes/origin/main
echo "DEINE_LETZTE_BEKANNTE_SHA" > .git/refs/heads/main
echo "DEINE_LETZTE_BEKANNTE_SHA" > .git/refs/remotes/origin/main
git rev-parse HEAD origin/main   # muss übereinstimmen
```

---

## 8 · Datenblock-Formate (HARTE Regel — sonst Tab-Bug)

Die init-Funktionen der Vorlagen sind starr. Wenn Dein Datenformat
nicht passt, läuft init() in einen TypeError und alle nachfolgenden
Tabs bleiben leer. **Memory `feedback_c1-vorlage-pattern.md`.**

```javascript
// === R/X/S-Vorlage (1013R) ===

VORENTLASTUNG:  { term: "die Begriff, -e", def: "Erklärung..." }
GENUS_DATA:     { word: "🌉 Wort", cat: "die" }   // 'der'/'die'/'das'/'pl'
LUECKE_DATA:    { pre: "vor ", ans: "Antwort", post: " nach." }   // single-blank
MC_DATA:        { q: "Frage?", opts: ["A","B","C","D"], correct: 1 }
satzbauData:    { parts: ["x","y","z"], valid: ["x","y","z"], punct: "." }   // FLACHES Array bei R/X/S
WORTSCHATZ:     { id:1, type:"n", en:"🌉 the X", artikel:"die", de:"X", plural:"Xen" }

// === G-Vorlage (1011G) ===

ZUO_DATA:       { id:'z1', text:'Begriff', cat:'aktiv' }   // ID PFLICHT, nicht weglassen
LUECKEN:        { id:1, before:'vor ', answer:'Antwort', after:' nach.' }   // anders als R/X/S!
satzbauData:    { parts:[...], valid:[[...]], punct:'.' }   // ARRAY VON ARRAYS bei G
WORTSCHATZ:     { id:1, en:'Hinweis', de:'Lösung' }   // Kurzformat
```

**Satzbau-Punkt-Regel:** Schluss-Punkt NIE in `parts:[]`. Engine
hängt ihn als `<span class="sb-punkt">` automatisch an. Komma im
Satzinneren bleibt Chip.

---

## 9 · Dashboard-Eintrag

C1-Sektion im Dashboard hat folgende Struktur:

```javascript
{ id: 'c1', label: 'C1 Grammatik',
  basis: 'https://fabdaf.github.io/daf-c1-uebungen/',
  einheiten: [
    { nr: '101x', titel: 'C1.1 · Einheit 1 — …', karten: [ /* fertig */ ]},
    { nr: '102x', titel: 'C1.1 · Einheit 2 — …', karten: [ /* fertig */ ]},
    { nr: '103x', titel: 'C1.1 · Einheit 3 — …', karten: [ /* fertig */ ]},
    { nr: '104x', titel: 'C1.1 · Einheit 4 — …', karten: [ /* fertig */ ]},
    { nr: '105x', titel: 'C1.1 · Einheit 5 — …', karten: [ /* fertig */ ]},
    { nr: '106x', titel: 'C1.1 · Einheit 6 — …', karten: [ /* fertig */ ]},
    // ← HIER NEU: { nr: '201x', titel: 'C1.2 · Einheit 1 — …', karten: [
    //                 { typ:'G', label:'G – Grammatik', titel:'2011G · Konnektoren', file:'DE_C1_2011G-…html', tags:'…' },
    //                 …
    //               ]},
    { nr: '90xx', titel: 'Vertiefungsblock — …', karten: [ /* alt */ ]},
    { nr: '308x', titel: 'Geistesgeschichte & Bundespolitik', karten: [ /* alt */ ]},
  ]
}
```

**Tags-Konvention:** alle Eigennamen, Konzepte, Personen, Daten der
Lektion + `c1 c1.2` + `lingoda` als Schluss-Anker. Frank sucht über
Tags. Lieber zu viele als zu wenige.

---

## 10 · Pexels-Banner — Pflicht zur Verifikation

**Memory `feedback_pexels-chrome.md`.** Auch übernommene IDs aus
früheren Lektionen MÜSSEN vor Commit verifiziert werden.

### Kurzer Workflow

```python
# In WebSearch (allowed_domains=["pexels.com"]) suchen, z.B.:
# "pexels.com photo X stock"
# Aus URL-Slug die Korrektheit ablesen:
# https://www.pexels.com/photo/black-vinyl-record-1486064/   ← Slug = Verifikation
```

### Bewährter Banner-Pool für Lektionen rund um Lesen/Bücher

```
207703  Federkiel und Tinte
2128249 Aufgeschlagenes altes Buch
256541  Bücherregal
1005012 Alte Bibliothek
2090650 Schreibtisch mit Buch
3137890 Filmrolle Vintage
2873486 Vintage Filmkamera
799443  Kinosaal
4144923 Notebook (Schreibwerkstatt-Standard)
267669  Wörterbuch im Bokeh (Wortschatz-Standard)
```

Für andere Themen einzeln neu suchen.

---

## 11 · Schreibwerkstatt-Spezifika (PFLICHT in X/R/S)

Memory `feedback_schreibwerkstatt-mikroaufgaben.md` und
`feedback_schreibwerkstatt-mail-aus-footer.md`.

**5 Mikroaufgaben** pro X/R/S-Lektion:
1. autobiografisch — eigene Erfahrung schildern
2. argumentativ — Position vertreten mit Begründung
3. analytisch — Sachverhalt prüfen / sezieren
4. bewertend — Stellung nehmen / präferieren
5. kreativ — eigenes Beispiel erfinden / Imagination

**KEINE sichtbaren Typ-Labels** wie „autobiografisch" am Karten-Titel.

**Pflicht-Namensfeld** oben (rote Umrandung leer, grün ab 2 Zeichen).

**JS-Konstanten anpassen pro Lektion:**
```javascript
var SCHREIB_NAME_KEY     = 'schreibwerkstatt_C1_2011G_name';
var SCHREIB_KEY_PREFIX   = 'schreibwerkstatt_C1_2011G_';
var SCHREIB_SENT_PREFIX  = 'schreibwerkstatt_C1_2011G_sent_';
var SCHREIB_LEKTION      = 'C1 – 2011G · Titel';
var BEST_KEY             = 'best_2011C1_';
```

**Footer-Mail dynamisch ziehen** (nicht hardcoden, Memory):
```javascript
var FOOTER_MAIL = 'FrankBurkert@fabdaf.onmicrosoft.com';
var FORMSUBMIT_ENDPOINT = 'https://formsubmit.co/ajax/' + FOOTER_MAIL;
```

**Bug-Fix nicht vergessen:** Im DOMContentLoaded-Handler unbedingt
`initSchreibwerkstatt()` aufrufen — sonst keine localStorage-
Wiederherstellung. (In 1012X-Original fehlte das.)

---

## 12 · Schreibstil C1 (NICHT C2, NICHT B2)

Memory `feedback_c2-schreibstil.md` beschreibt C2 (essayistisch,
1500–2000 Wörter). C1 ist **eine Stufe darunter**:

| Achse | C1 |
|---|---|
| Vorbild | ZEIT-Wissen, FAZ-Politik, Spektrum |
| Satzlänge ⌀ | 18–25 Wörter, Hypotaxen zwei Ebenen |
| Lexik | Idiomatik sicher, Fachbegriffe gesetzt |
| Position | erkennbar, argumentiert |
| Textsorte | journalistische Hintergrundanalyse |
| Wörter R-Text | **600–900** |

**Drei harte Hebel gegen C2-Versuchung:**
1. **Faktenanker engmaschig** — Daten, Zahlen, Personen, Institutionen
2. **Argumente innerhalb desselben Absatzes schließen** — keine
   Schachtel-Argumentation über vier Absätze
3. **Keine Schwebe-Schlüsse, keine Ironie, keine offenen Enden.**
   Texte beantworten die Frage, die sie stellen.

---

## 13 · Recherche-Pflicht

Trainings-Wissensstand endet **Mai 2025**, heute ist **April 2026** —
fast ein Jahr Lücke.

**Werkzeuge** (verfügbar in Cowork-Session):
- `WebSearch` für 80–90 % der Faktenchecks
- `mcp__workspace__web_fetch` für gezielte URL-Abrufe
- Chrome-MCP für interaktive Recherche

**Schwellenwert:** „Ein Schüler könnte den Punkt heute Abend googeln
und mich darauf ansprechen" — wenn ja, recherchieren.

**Bei Unsicherheit:** zurückhaltend formulieren („nach Schätzungen…",
„Stand 2024…") oder Faktum weglassen.

---

## 14 · Bewährte Routinen aus C1.1 (was zur Standardform geworden ist)

1. **Aktualisierender Anker** in jedem Lesetext — etwa „2024 wurde …
   UNESCO-Erbe" oder „Seit 2025 …" oder „Im April 2026 …". Macht
   den Text gegenwärtig statt geschichtslos.
2. **5 Mikroaufgaben mit Diversität** — mindestens eine
   autobiografische, eine analytische, eine kreative. Variiere:
   nicht jedes Mal „erfinde einen Krimi 2026", sondern Mustersammlung,
   Mini-Manifest, Brief, Schlagzeile, Trickfilm-Plot, Gegen-Pamphlet.
3. **JSDOM-Test BEVOR Commit** — nicht nachher.
4. **Anführungszeichen-Check VOR Commit** mit Auto-Fix:
   ```python
   c = re.sub(r'„([^„"…\n]{1,80})"', lambda m: '„' + m.group(1) + '"', c)
   ```
5. **Pexels-IDs verifizieren** vor Commit (per WebSearch URL-Slug).
6. **Stumm committen** — keine SHA-Berichte im Chat.

---

## 15 · Memories, die für C1.2 besonders relevant sind

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
reference_fabdaf-pfad.md                → Mac vs. Sandbox-Pfade
reference_git-index-workaround.md       → Alt-Index-Workflow
```

---

## 16 · Bekannte Stolpersteine aus C1.1 (was Zeit gekostet hat)

### Stolperstein 1: Refs-Korruption nach gescheiterten Push-Versuchen
Der Alt-Index-Workflow überschrieb ein Mal die ref-Datei mit leerem
String, weil `$COMMIT` leer war. Reparatur: SHA aus
`.git/logs/refs/heads/main` zurückschreiben, dann normal weiter.

### Stolperstein 2: Pexels-Banner-Pool von 1012X war systematisch falsch beschriftet
Die in der ersten Übergabe empfohlenen IDs (1486064 = „Man Holding
Chin", nicht Vinyl; 935949 = „Photo of Men Having Conversation",
nicht Wörterbuch) müssen für jede neue Lektion neu gesucht und
verifiziert werden.

### Stolperstein 3: initSchreibwerkstatt() im DOMContentLoaded vergessen
Im 1012X-Original wurde es nie aufgerufen — keine localStorage-
Wiederherstellung, keine Namensvalidierung beim Laden. Bei jeder
neuen R/X/S-Datei prüfen, dass `initSchreibwerkstatt();` im
DOMContentLoaded-Handler steht.

### Stolperstein 4: Anführungszeichen U+0022 statt U+201C
Beim Replace mit Python-Strings rutscht regelmäßig ein ASCII-Quote
durch. Auto-Fix-Regex am Ende jedes Build-Scripts.

### Stolperstein 5: Lesetext-Wortzahl
600–900 Wörter ist der Zielkorridor. Unter 500 wirkt zu dünn, über
1000 wandert in C2-Territorium. Zähle nach JSDOM-Test.

---

## 17 · Erste konkrete Aktion

```bash
# 1. Pfad bestimmen
MNT=$(ls /sessions/ 2>/dev/null | head -1)
ROOT=/sessions/$MNT/mnt/fabDaF

# 2. Sandbox-Auth einrichten
cd $ROOT && bash scripts/setup-sandbox-credentials.sh

# 3. Lingoda-PDF 2011G lesen
python3 -c "
from pypdf import PdfReader
r = PdfReader('$ROOT/lingoda c1/C 1.2/C1_2011G_DE.pdf')
for i, p in enumerate(r.pages):
    t = p.extract_text()
    if t.strip(): print(f'--- S{i+1} ---'); print(t)
"

# 4. Themen der gesamten Einheit 1 (2011G–2018S) überblicken
for f in 2011G 2012X 2013R 2014S 2015R 2016S 2017R 2018S; do
  echo \"=== $f ===\"
  python3 -c \"
from pypdf import PdfReader
r = PdfReader('$ROOT/lingoda c1/C 1.2/C1_${f}_DE.pdf')
print(r.pages[0].extract_text()[:200])
\"
done

# 5. Vorlage kopieren (G-Vorlage von 1011G)
cp $ROOT/htmlS/C1/DE_C1_1011G-redewiedergabe.html $ROOT/htmlS/C1/DE_C1_2011G-konnektoren.html

# 6. Build-Script schreiben (in /sessions/$MNT/mnt/outputs/build_2011G.py)
# 7. Ausführen, JSDOM-Test, Anführungszeichen-Check, Dashboard-Eintrag, Commit
# 8. Weiter zu 2012X, 2013R, 2014S, 2015R, 2016S, 2017R, 2018S

# Wenn am Ende des Turns Einheit 1 (8 Lektionen) komplett ist, hat
# sich der Turn gelohnt. Mehr ist mehr.
```

---

## 18 · Wenn Du fertig bist

Wenn am Ende Deines Turns Einheit 1 von C1.2 komplett ist (= 8/200
weitere = neue Gesamtsumme 56/200), aktualisiere diese Datei auf den
neuen Stand und committe sie zusammen mit den Lektionen.

**Was Du auf keinen Fall tun darfst:**
- Lektionen halbgar liefern, nur damit die Zahl steigt.
- Inhaltliche Fakten ungeprüft setzen, wenn Du unsicher bist.
- Frank im Chat mit Statusberichten oder SHA-Listen überfluten.
- Eigenmächtig die Tab-Struktur erweitern oder umstellen.
- Den Wortschatz nicht als letzten Tab führen.
- Die Schreibwerkstatt anders gestalten als das 1013R-Vorbild.
- Mit eigenem Code statt Vorlagen-Klon arbeiten.

**Was Du immer tun darfst:**
- Nachfragen, wenn ein didaktischer Konflikt auftaucht.
- Wenn ein Fakt unsicher ist: konservativ formulieren oder weglassen.
- Bei Frank-Frust: keine Selbstkasteiung — kurz zuhören, präzise
  reparieren, weitermachen.

**Was Du immer mitbringen musst:**
- Aktualisierende Anker (2024–2026-Bezüge).
- Saubere Quellen-Angabe in der story-source-Zeile.
- Tags-dichten Dashboard-Eintrag.

Viel Erfolg.
