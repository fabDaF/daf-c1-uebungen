# DaF — Masterplan für interaktive HTML-Übungsdateien
## Gültig für: C1

Dieses Dokument ist die **einzige verbindliche Referenz** für alle C1-HTML-Übungsdateien.
Es wird **vor jeder Arbeit** an einer C1-HTML-Datei gelesen — ohne Ausnahme.

---

## ⚠️ PFLICHT: Lingoda-Texte IMMER überarbeiten

> **Die Lingoda-PDFs sind Ausgangsmaterial — kein fertiger Inhalt.**
> Lingoda-C1-Texte sind für den Einsatz in den HTML-Übungen **nicht geeignet** und müssen
> **immer vollständig neu geschrieben** werden.

### Warum Lingoda-C1-Texte nicht verwendet werden dürfen wie sie sind

- **Präsentationsformat:** Die Lingoda-C1-PDFs sind Lehrer-Präsentationsfolien — pro Folie steht kaum Text
- **Keine Substanz:** Übungsanweisungen setzen einen Live-Lehrer voraus, der den Rest erklärt
- **Zu flach für C1:** Sprachniveau und inhaltliche Tiefe entsprechen oft eher B2
- **Keine Kohärenz:** Texte sind auf viele Folien verteilt — kein Lesefluss möglich

### Was stattdessen zu tun ist

#### Für G-Dateien (Grammatik) — Phase 1 Priorität
1. Grammatikthema aus dem Lingoda-PDF entnehmen
2. Eigenständige, präzise **Grammatikerklärung** auf C1-Niveau schreiben
3. Eigene Beispielsätze — authentisch, komplex, mit C1-Wortschatz
4. Beispielsätze spiegeln das **Grammatikthema in natürlichem Kontext** wider
5. Lückentexte: anspruchsvoll, nicht trivial, auf C1-Niveau

#### Für R-Dateien (Lesetexte) — Phase 2
1. Thema aus Lingoda als Ausgangspunkt, Text **vollständig neu schreiben**
2. Mindestens 500–700 Wörter (C1-Niveau)
3. Akademischer oder journalistischer Stil
4. Skill `skill-anspruchsvolle-texte` verwenden

#### Für X- und S-Dateien — Phase 3
1. Kommunikationsanlässe aus Lingoda als **Idee** nutzen
2. Sprachniveau: C1 — komplexe Strukturen, formelle Wendungen, nuancierte Ausdrucksweise

---

## ✍️ Schreibrolle — Verbindliche Haltung für alle C1-Texte

Bevor eine einzige Zeile geschrieben wird, nimmt Claude diese Haltung ein:

> **Ich schreibe für Erwachsene, die Deutsch auf einem fortgeschrittenen Niveau beherrschen.**
> Mein Leser versteht komplexe Satzstrukturen, kennt Fachvokabular und erwartet inhaltliche Tiefe.
> Ich schreibe nicht vereinfacht. Ich schreibe authentisch — wie ein deutschsprachiger Sachbuchautor
> oder Qualitätsjournalist. Das Grammatikthema ist organisch eingebaut, nie aufgesetzt.

**Stilprinzipien C1 (nicht verhandelbar):**

1. **Komplexe Syntax organisch** — Das Grammatikthema muss im Erklärungstext und in Beispielen
   so natürlich vorkommen, dass es nicht als Übung wirkt. Kein künstlicher Einbau.

2. **Akademisch-journalistischer Register** — Kein Schulbuchton. Kein „Wie wir sehen…".
   Stattdessen: präzise, elegant, informativ. Vorbild: ZEIT, FAZ, Spektrum der Wissenschaft.

3. **Intellektuelle Herausforderung** — C1-Lernende sind oft gebildete Erwachsene.
   Themen und Beispiele sollen inhaltlich interessieren — nicht nur grammatisch üben.

4. **Quasthoff-Sprache** — Alle Verb-Nomen-Verbindungen aus dem Kollokationswörterbuch.
   Besonders bei C1 gilt: banale Kollokationen sind inakzeptabel.

5. **Faktenprüfung** — Alle Zahlen, Namen, Sachverhalte mit WebSearch verifizieren.

---

## 📚 Kollokationswörterbuch — Quasthoff (Pflicht-Ressource)

| Ressource | Pfad |
|-----------|------|
| PDF (vollständig) | `/sessions/fervent-sweet-einstein/mnt/fabDaF/Grammatik/Worterbuch-Der-Kollokationen.pdf` |
| TXT (durchsuchbar) | `/sessions/fervent-sweet-einstein/mnt/fabDaF/Grammatik/Worterbuch-Der-Kollokationen.txt` |

---

## 🖼️ Bild-Workflow

**Phase 1 — Während der Erstellung:**
- Pexels-Bilder als externe URL einbinden: `src="https://images.pexels.com/photos/ID/pexels-photo-ID.jpeg"`

**Phase 2 — Nach Fertigstellung:**
- Skill `pexels-bild-check` für Überprüfung und Einbettung

---

## 📊 Dashboard

Das einzige gültige Dashboard ist:
```
/sessions/fervent-sweet-einstein/mnt/fabDaF/htmlS/dashboard.html
file:///Users/frankburkert/Cowork/htmlS/dashboard.html
```

**Neue Kategorie `C1 Grammatik` im Dashboard anlegen.**
**Pflicht nach jeder neuen C1-HTML-Datei:** Sofort ins Dashboard eintragen.

---

## 0. Vor dem Start — Pflichtlektüre Skills

| Skill | Wann |
|-------|------|
| `daf-grammatik-uebungen` | Bei jeder G-Datei |
| `daf-html-layout` | Bei jeder Datei |
| `satzbau-drag-drop` | Wenn Satzbau-Tab enthalten |
| `daf-uebungsformen` | Immer |
| `daf-bilder-pflicht` | Immer |
| `textgestaltung-daf` | Wenn Lesetext-Tab enthalten |
| `lesetext-hervorhebung` | Wenn Lesetext enthalten |
| `daf-browser-test` | Nach Fertigstellung |
| `skill-anspruchsvolle-texte` | Bei R-Dateien |

---

## 1. Nomenklatur

### Dateiname-Schema

```
DE_C1_LLLLx-thema.html
     ^^  ^^^^
     ||  ||||__ x = Datei-Typ (G, R, X, S, W)
     ||  |||___ Lektionsnummer innerhalb der Einheit (1–8)
     ||  ||____ Einheitsnummer (01–07)
     ||  |_____ Kurs (1 = C1.1 / 2 = C1.2 / …)
     ||________ Niveau (C1)
     |_________ Sprache
```

Beispiel: `DE_C1_1011G-nominalstil.html`

### Datei-Typen

| Typ | Bedeutung | Tab-Struktur |
|-----|-----------|--------------|
| G | Grammatik | Entdecken + Regel + Lückentext + Satzbau + Wortschatz |
| R | Lesetext | Vorentlastung + Lesetext + Lückentext + MC + Satzbau |
| X | Extra / Kommunikation | Vorentlastung + Lückentext + Satzbau + Wortschatz |
| S | Speaking | Sprechanlässe + Redemittel + Übungen |
| W | Schreiben | Anleitung + Modelltext + Aufgabe |

### Quellmaterial (Lingoda-PDFs)

| Sub-Level | Pfad |
|-----------|------|
| C1.1 | `/sessions/fervent-sweet-einstein/mnt/fabDaF/lingoda/C 1.1/` |
| C1.2 | `/sessions/fervent-sweet-einstein/mnt/fabDaF/lingoda/C 1.2/` |
| C1.3 | `/sessions/fervent-sweet-einstein/mnt/fabDaF/lingoda/C 1.3/` |
| C1.4 | `/sessions/fervent-sweet-einstein/mnt/fabDaF/lingoda/C 1.4/` |

### HTML-Zielordner

```
/sessions/fervent-sweet-einstein/mnt/fabDaF/htmlS/C1/
```

---

## 2. Satzbau-Pflicht-Fix

⚠️ **Bekannter Bug:** Punct-Chips (`,.`) dürfen NICHT vorab in die Zone gesetzt werden.

```javascript
// RICHTIG:
var shuffled = shuffleArr(item.words);  // alle Wörter inkl. ,.

// FALSCH (nie verwenden!):
var nonPunct = item.words.filter(...);
var shuffled = shuffleArr(nonPunct);
```

---

## 3. C1-Grammatik — Die 7 Kernthemen (Phase 1)

Dies sind die **genuinen C1-Grammatikthemen** — Inhalte, die in B1/B2 nicht systematisch
behandelt werden und echten Mehrwert für Fortgeschrittene bieten.

| Datei | Grammatikthema | Einheit |
|-------|---------------|---------|
| `DE_C1_1011G-nominalstil.html` | Nominalstil | 101x — Schriftsprache & Stil |
| `DE_C1_1021G-subjektive-modalverben.html` | Subjektive Bedeutung der Modalverben | 102x — Modalität & Nuance |
| `DE_C1_1031G-sonderstellung-satz.html` | Sonderstellung im Satz | 103x — Satzarchitektur |
| `DE_C1_1041G-variable-verbpraefixe.html` | Variable Verbpräfixe | 104x — Wortbildung & Bedeutung |
| `DE_C1_1051G-verben-genitiv.html` | Verben mit Genitiv | 105x — Formale Sprache |
| `DE_C1_1061G-modalpartikeln.html` | Modalpartikeln für Fortgeschrittene | 106x — Gesprochene Sprache |
| `DE_C1_1071G-kommasetzung.html` | Kommasetzung & Rechtschreibung | 107x — Schriftliche Korrektheit |

### Thematische Einheiten

| Einheit | Thema | G-Datei | Zukünftige Dateien |
|---------|-------|---------|-------------------|
| 101x | Schriftsprache & Stil | 1011G | 1012R, 1013X, 1014S |
| 102x | Modalität & Nuance | 1021G | 1022R, 1023X, 1024S |
| 103x | Satzarchitektur | 1031G | 1032R, 1033X, 1034S |
| 104x | Wortbildung & Bedeutung | 1041G | 1042R, 1043X, 1044S |
| 105x | Formale Sprache | 1051G | 1052R, 1053X, 1054S |
| 106x | Gesprochene Sprache | 1061G | 1062R, 1063X, 1064S |
| 107x | Schriftliche Korrektheit | 1071G | 1072R, 1073X, 1074S |

---

## 4. Fertigstellungsstatus C1

### Phase 1 — G-Dateien (7 Kernthemen)

| Datei | Grammatikthema | Status |
|-------|---------------|--------|
| DE_C1_1011G-nominalstil.html | Nominalstil | ✅ Fertig — Browser-Test bestanden (2026-03-28) |
| DE_C1_1021G-subjektive-modalverben.html | Subjektive Bedeutung der Modalverben | ✅ Fertig — gepusht (2026-03-28) |
| DE_C1_1031G-sonderstellung-satz.html | Sonderstellung im Satz | ✅ Fertig — gepusht (2026-03-28) |
| DE_C1_1041G-variable-verbpraefixe.html | Variable Verbpräfixe | ✅ Fertig — gepusht (2026-03-28) |
| DE_C1_1051G-verben-genitiv.html | Verben mit Genitiv | ✅ Fertig — gepusht (2026-03-28) |
| DE_C1_1061G-modalpartikeln.html | Modalpartikeln für Fortgeschrittene | ✅ Fertig — gepusht (2026-03-28) |
| DE_C1_1071G-kommasetzung.html | Kommasetzung & Rechtschreibung | ✅ Fertig — gepusht (2026-03-28) |

### Phase 2 — R-, X-, S-Dateien (pro Einheit, nach Abschluss Phase 1)

Für jede Einheit nach Abschluss der G-Datei:
1. R-Datei (Lesetext zum Einheitsthema)
2. X-Datei (Kommunikation & Extra-Übungen)
3. S-Datei (Sprechen & Diskussion)

---

## 5. Qualitäts-Checkliste C1

### G-Dateien
- [ ] Mindestens 10 Beispielsätze — authentisch, komplex, C1-Niveau?
- [ ] Entdecken-Tab: Lernende erschließen die Regel selbst (nicht erklärt, sondern entdeckt)?
- [ ] Lückentext: Kontext ist anspruchsvoll — kein banaler Schulbuchsatz?
- [ ] Satzbau: Sätze haben 7–12 Chips, zeigen echte C1-Syntax?
- [ ] Wortschatz: 12–16 Karten, C1-Niveau, Quasthoff-Kollokationen?
- [ ] Kollokationen aus Quasthoff-Wörterbuch überprüft?
- [ ] Kein Lehrton, kein Schulbuchstil?

### R-Dateien (Phase 2)
- [ ] Mindestens 500 Wörter?
- [ ] Akademisch-journalistischer Stil?
- [ ] Grammatikthema organisch eingebaut (nicht spürbar)?
- [ ] Fakten mit WebSearch verifiziert?

---

## 6. Zusammenfassung — Was ist zu tun?

### Schritt 1 — Infrastruktur ✅
- [x] Ordner `htmlS/C1/` anlegen
- [x] C1-MASTERPLAN.md erstellen
- [ ] Neue Kategorie „C1 Grammatik" im Dashboard anlegen

### Schritt 2 — Phase 1: Die 7 G-Dateien
Empfohlene Reihenfolge nach didaktischem Gewicht:
1. **1011G Nominalstil** — häufigste Hürde bei C1-Lernenden, hoher Praxiswert
2. **1021G Subjektive Modalverben** — subtiler Bedeutungsunterschied, großer Aha-Effekt
3. **1041G Variable Verbpräfixe** — spielerisch, kontrastreich (umfahren vs. umfahren)
4. **1031G Sonderstellung im Satz** — wichtig für gehobene Schriftsprache
5. **1051G Verben mit Genitiv** — selten, aber korrekt
6. **1061G Modalpartikeln** — für natürliche, nuancierte Kommunikation
7. **1071G Kommasetzung** — systematisch, auch für Muttersprachler wertvoll

### Schritt 3 — Browser-Test nach jeder Datei
Skill `daf-browser-test` — testen bis 0 Fehler.

### Schritt 4 — Dashboard aktualisieren
Nach jeder fertiggestellten Datei sofort ins Dashboard eintragen.

### ⚠️ Satzbau-Hinweis für künftige Dateien
Die erste Datei (1011G) nutzt `pool-0`/`row-0` statt der Standard-IDs `sb-bank-0`/`sb-row-0`.
Funktional bestanden, aber ab der nächsten Datei **immer** `satzbau-drag-drop`-Standard verwenden:
`satzbauContainer` / `sb-bank-N` / `sb-row-N` / `sb-fb-N` / `sbDragged`

### Gesamtumfang Phase 1
| Phase | Dateien | Fertig |
|-------|---------|--------|
| Phase 1 (G-Dateien) | 7 | 7 |
| Phase 2 (R, X, S) | 21 | 0 |
| **Gesamt** | **28** | **7** |
