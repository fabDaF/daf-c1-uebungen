# DaF — Masterplan für interaktive HTML-Übungsdateien
## Gültig für: C1

Dieses Dokument ist die **einzige verbindliche Referenz** für alle C1-HTML-Übungsdateien.
Es wird **vor jeder Arbeit** an einer C1-HTML-Datei gelesen — ohne Ausnahme.

---

## ⚠️ Stand 2026-04-27 — Kursrichtungswechsel

Mit der Bereitstellung des vollständigen Lingoda-C1-Korpus (200 PDFs in vier Kursen
C1.1 – C1.4) wurde am 2026-04-27 entschieden: **C1 folgt ab sofort dem Lingoda-Schema 1:1**,
analog zur C2-Pipeline. Die zuvor unter den Codes 1011G–1071G geführte eigene Themenreihe
wurde in einen Sonderblock 9011G–9071G überführt und bleibt dort als „Vertiefungsblock"
erhalten.

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

## 📚 Lingoda-Quellmaterial

| Kurs | Pfad | PDFs |
|------|------|------|
| C1.1 | `lingoda c1/C 1.1/` | 50 |
| C1.2 | `lingoda c1/C 1.2/` | 50 |
| C1.3 | `lingoda c1/C 1.3/` | 50 |
| C1.4 | `lingoda c1/C 1.4/` | 50 |

**Lingoda-Schema pro Kurs:** 6 Einheiten × 8 Lektionen + 2W
- Pro Einheit: `xx1G` (Grammatik) · `xx2X` (Extra/Kommunikation) ·
  `xx3R` `xx5R` `xx7R` (3× Lesen) · `xx4S` `xx6S` `xx8S` (3× Sprechen)
- Am Kursende: `xx71W` + `xx72W` (Schreiben)

**Wichtig:** Anders als in der ursprünglichen Masterplan-Fassung gilt jetzt:
**Lingoda-Codes 1:1 übernehmen.** Eine Datei `1011G` heißt 1011G,
weil die Lingoda-PDF so heißt — auch wenn das ursprüngliche Lingoda-Material
für die HTML-Übung neu geschrieben werden muss.

---

## 🗂️ Datei-Typen

| Typ | Bedeutung | Tab-Struktur (5 Tabs) |
|-----|-----------|----------------------|
| G | Grammatik | Entdeckung · Zuordnung · Lückentext · Satzbau · Wortschatz |
| X | Extra / Kommunikation | Vorentlastung · Lesetext · Lückentext · Satzbau · Wortschatz |
| R | Lesetext | Vorentlastung · Lesetext · Genus · Lückentext · MC · Satzbau · Wortschatz |
| S | Speaking | Vorentlastung · Lesetext · Genus · Lückentext · MC · Satzbau · Schreibwerkstatt · Wortschatz |
| W | Schreiben | Anleitung · Modelltext · Mikroaufgaben · Wortschatz |

Vorlagen pro Typ:
- **G:** `DE_C1_1011G-redewiedergabe.html` (Pilot, ab 27.04.2026)
- **R/S:** `DE_C2_0407S-online-shopping.html` (C2-Goldstandard, adaptiert)
- **X/W:** noch zu pilotieren

---

## 🛠️ Pipeline pro Lektion

```bash
# 1. Vorlage kopieren
cd /sessions/<mnt>/mnt/fabDaF/htmlS/C1
cp DE_C1_1011G-redewiedergabe.html DE_C1_1012X-thema.html  # ggf. R/S/W-Vorlage

# 2. Code & Titel umstellen
FILE=DE_C1_1012X-thema.html
sed -i 's/1011G/1012X/g' "$FILE"
sed -i 's|<title>[^<]*</title>|<title>NEU – C1 Grammatik</title>|' "$FILE"
sed -i 's|<h1>[^<]*</h1>|<h1>NEU</h1>|' "$FILE"

# 3. Build-Script (Sec-Inhalte + Datenblöcke ersetzen)
python3 /sessions/<mnt>/mnt/outputs/build_C1_1012X.py

# 4. Audit + Dashboard + safe-commit
scripts/safe-commit.sh "C1 1012X: Titel" htmlS/C1/DE_C1_1012X-thema.html htmlS/dashboard.html
```

---

## 🖼️ Bild-Workflow

**Phase 1 — Während der Erstellung:** Pexels-Bilder als externe URL einbinden.
**Phase 2 — Nach Fertigstellung:** Skill `pexels-bild-check` für Überprüfung und Einbettung.

Pexels-Banner aus dem Pilot 1011G (Themenfeld Sprache/Schreiben/Presse) — 1:1 für G-Dateien
übernehmbar:
- 1591056 — Zeitungen (Entdeckung)
- 1181396 — Redaktion (Zuordnung)
- 5710614 — Schreiben (Lückentext)
- 267669 — Sprache (Satzbau)
- 256541 — Bücher (Wortschatz)

---

## 📊 Dashboard

```
htmlS/dashboard.html
file:///Users/frankburkert/Cowork/htmlS/dashboard.html
```

**Pflicht nach jeder neuen C1-HTML-Datei:** Sofort ins Dashboard eintragen.

Die C1-Sektion ist gegliedert in:
1. **101x – 107x:** C1.1 (6 Einheiten + Schreibwerkstatt)
2. **201x – 207x:** C1.2 (analog)
3. **301x – 307x:** C1.3 (analog)
4. **401x – 407x:** C1.4 (analog)
5. **90xx:** Vertiefungsblock — frühere eigene G-Reihe
6. **308x:** Sonder­projekt Geistesgeschichte & Bundespolitik

---

## 📋 Lingoda-Themenkatalog C1.1 – C1.4 (Grammatik-Schwerpunkte)

### C1.1 — Konjunktiv-Welt & Stilfundament
| Code | Thema |
|---|---|
| 1011G | Redewiedergabe für Fortgeschrittene (Konjunktiv I) ✅ |
| 1021G | Zukunft in der Vergangenheit (würde-Form, Futur II) |
| 1031G | Der Ärger mit hätte (Konjunktiv II Vergangenheit + Modalverben) |
| 1041G | Nominalstil |
| 1051G | Modalpartikeln für Fortgeschrittene |
| 1061G | Ausdrücke der Schriftsprache (Genitiv-Präpositionen) |
| 1071W | Vergleichender Essay |
| 1072W | Rezension |

### C1.2 — Argumentation & Stilausbau
| Code | Thema |
|---|---|
| 2011G | Logische Konnektoren (Argumente anbringen) |
| 2021G | Subjektive Bedeutung der Modalverben |
| 2031G | Partizipialkonstruktionen |
| 2041G | Sonderstellung im Satz |
| 2051G | Sich raffinierter ausdrücken |
| 2061G | Immer wieder hätte |
| 2071W / 2072W | Schreiben |

### C1.3 — Vertiefung
| Code | Thema |
|---|---|
| 3011G | Verben mit Genitiv |
| 3021G | Nominalisierung komplexer Strukturen |
| 3031G | Konnektoren für Fortgeschrittene |
| 3041G | Mehr über Partizipialkonstruktionen |
| 3051G | Sich raffinierter ausdrücken (Wdh.) |
| 3061G | Variable Verbpräfixe |
| 3071W / 3072W | Schreiben |

### C1.4 — Feinschliff
| Code | Thema |
|---|---|
| 4011G | Fortgeschrittene Verwendung von Adjektiven |
| 4021G | Fortgeschrittene Präpositionen der formalen Sprache |
| 4031G | Das Passiv für Fortgeschrittene |
| 4041G | (PDF-Encoding-Fehler — Inhalt nachprüfen) |
| 4051G | Verben mit Präpositionen für Fortgeschrittene |
| 4061G | Verb-Präfixe für Fortgeschrittene |
| 4071W / 4072W | Schreiben |

---

## 📚 Kollokationswörterbuch — Quasthoff (Pflicht-Ressource)

| Ressource | Pfad |
|-----------|------|
| PDF | `Grammatik/Worterbuch-Der-Kollokationen.pdf` |
| TXT | `Grammatik/Worterbuch-Der-Kollokationen.txt` |

---

## 6. Fortschrittsstand (2026-04-27)

| Kurs | G | X | R | S | W | Σ | Stand |
|---|---|---|---|---|---|---|---|
| C1.1 | 1/6 | 0/6 | 0/18 | 0/18 | 0/2 | **1/50** | Einheit 1 (1011G ✅) |
| C1.2 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | offen |
| C1.3 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | offen |
| C1.4 | 0/6 | 0/6 | 0/18 | 0/18 | 0/2 | 0/50 | offen |
| **Σ** | **1/24** | **0/24** | **0/72** | **0/72** | **0/8** | **1/200** | |

**Sonderblock** (außerhalb der 200): 9011G–9071G (7 ✅) + 308x (6 + 1 ✅).

---

## 7. Vorgehen pro Turn

Pro Turn: **so viele Lektionen wie möglich**, in Lingoda-Reihenfolge. Reihenfolge innerhalb
einer Einheit: G → X → R → S → R → S → R → S. Wenn eine Einheit komplett ist, weiter zur
nächsten — bis Kontext oder Energie an Grenzen stoßen.

Erst-Pilot pro Datei-Typ ist der Goldstandard für alle nachfolgenden Lektionen desselben Typs.

**1011G ist der G-Pilot — fertig am 27.04.2026.**
