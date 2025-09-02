# Leitfaden „Ortskennzeichen“ (Ortsaspekt „+“/„++“) im Schaltschrankbau & PLC

- [Leitfaden „Ortskennzeichen“ (Ortsaspekt „+“/„++“) im Schaltschrankbau \& PLC](#leitfaden-ortskennzeichen-ortsaspekt--im-schaltschrankbau--plc)
  - [1) Normativer Rahmen (was gilt)](#1-normativer-rahmen-was-gilt)
  - [2) Auswahl des **richtigen Ortskennzeichens** – Schritt für Schritt](#2-auswahl-des-richtigen-ortskennzeichens--schritt-für-schritt)
    - [Schritt A – Entscheiden: **Site (++)** und/oder **Host (+)**](#schritt-a--entscheiden-site--undoder-host-)
    - [Schritt B – **Hierarchie** festlegen (von grob nach fein)](#schritt-b--hierarchie-festlegen-von-grob-nach-fein)
    - [Schritt C – **Buchstabenklasse** gemäß **IEC 81346-2** wählen](#schritt-c--buchstabenklasse-gemäß-iec-81346-2-wählen)
    - [Schritt D – **Nummerierung** vergeben](#schritt-d--nummerierung-vergeben)
    - [Schritt E – **Aspekte kombinieren** (bei Bedarf)](#schritt-e--aspekte-kombinieren-bei-bedarf)
  - [3) **Ortskennzeichen in bestehenden Plänen finden** (Vorgehensweise)](#3-ortskennzeichen-in-bestehenden-plänen-finden-vorgehensweise)
  - [4) **Beispielhafte, normkonforme Muster**](#4-beispielhafte-normkonforme-muster)
  - [5) **Qualitätssicherung \& Do/Don’t**](#5-qualitätssicherung--dodont)
  - [6) **Minimaler Projektstandard (empfohlen)**](#6-minimaler-projektstandard-empfohlen)
    - [Quellen](#quellen)

## 1) Normativer Rahmen (was gilt)

- **Aspekte & Vorzeichen.** Referenzkennzeichnungen bestehen aus unabhängigen Aspekten. Relevante Vorzeichen: `+` **Host-Installation (Einbauort)**, `++` **Site-Installation (Standort)**; daneben `=` Funktion, `−` Produkt, `%` Typ, `#` Management. ([Iteh Standards][1])
- **Klassifikationsbuchstaben.** Die **Buchstaben kommen aus IEC 81346-2** (aktuell: 2019). Für ortsbezogene Träger/Einbauten ist die **Hauptklasse „U“ (holding object / Objekt zum Lokalisieren/Halten)** maßgeblich; Unterklassen differenzieren z. B. Umschließen/Tragen/Stützen. ([Iteh Standards][2])
- **Darstellung im Plan.** Die **Platzierung von Referenzkennzeichen** an Symbolen regelt **IEC 61082-1** (z. B. oberhalb bei horizontalen, links bei vertikalen Anschlussrichtungen). ([Iteh Standards][3])
- **CAE-Praxis (Beispiel EPLAN).** Strukturierung nach **Funktion/Ort/Produkt** erfolgt über **Identifier-Blocks** („Struktursegmente“). ([eplan.help][4])

---

## 2) Auswahl des **richtigen Ortskennzeichens** – Schritt für Schritt

### Schritt A – Entscheiden: **Site (++)** und/oder **Host (+)**

1. **Site (`++`)** verwenden, wenn der **Standort absolut** ist (Gebäude → Geschoss → Raum, Aufstellplatz, Feld).
2. **Host (`+`)** verwenden, wenn der **Einbauort relativ** zum Produkt/Schrank ist (Schaltschrank → Montageplatte → Träger/DIN-Schiene → Position).
   *(Die Trennung „++“ vs. „+“ ist normativ festgelegt.)* ([Iteh Standards][1])

### Schritt B – **Hierarchie** festlegen (von grob nach fein)

- **Site (`++`)**: z. B. `++GEBAEUDE1++EG++R015`.
- **Host (`+`)**: z. B. `+SCHRANK1+PLATTE1+SCHIENE1`.
  *(Mehrstufige Bezeichnungen entstehen durch **Verketten** von Einzelniveaus.)* ([Readijip][5])

### Schritt C – **Buchstabenklasse** gemäß **IEC 81346-2** wählen

- Für **Orte/Träger/Einbauten** gilt **Hauptklasse „U“** (holding/localising object).
  **Beispiele (typisch im Schaltschrankbau):**
  – Schaltschrank/Umhausung (**U…**),
  – Kabelpritsche/Leiter/Kanäle (**U…**),
  – Montageplatte/Konsolen/Stützen (**U…**).
  *(Detail-Unterklassen liefert die IEC 81346-2:2019.)* ([Iteh Standards][2])

> **Wichtig:** Keine „freien“ Buchstaben erfinden. **„H…“** steht nach 81346-2 **nicht** für „Host/Ort“, sondern (Hauptklasse **H**) für **Stoffverarbeitung** – also **falsch** für Ortskennzeichen. ([Wikipedia][6])

### Schritt D – **Nummerierung** vergeben

- **Zähler nur zur Unterscheidung** gleichartiger Elemente; **keine Bedeutungen** in Nummern „codieren“ (z. B. „01=Hauptfeld“ vermeiden). ([Readijip][5])

### Schritt E – **Aspekte kombinieren** (bei Bedarf)

- Aspekte sind **nebeneinander** nutzbar, z. B.:
  `++WERK1++HALL1 +SCHRANK1+SCHIENE2 −M1`
  *(Site) · (Host) · (Produktkomponente)*.
  **Jeder Aspekt bleibt inhaltlich „rein“.** ([Readijip][5])

---

## 3) **Ortskennzeichen in bestehenden Plänen finden** (Vorgehensweise)

1. **Titel-/Kopfbereich & Strukturboxen prüfen.** Viele CAE-Systeme zeigen **Projektstruktur** (Installation/Ort) in Kopfzeile/Seiteneinstellungen oder als **Identifier-Blöcke** an. In EPLAN z. B. über „Projektstruktur nach EN 81346“ → **Identifier-Blocks**. ([eplan.help][4])
2. **Am Symbol nachsehen.** Die **Position der Referenzkennzeichen** richtet sich nach IEC 61082-1 (oberhalb/links je nach Anschlussrichtung). Dort stehen häufig **Kurzformen** der Ortssegmente. ([Iteh Standards][3])
3. **Seitennavigation/Verzeichnisse.** Stücklisten, Geräte-/Klemmen-/Aufstellungslisten enthalten oft **Ortsspalten** (Site/Location). Diese sind i. d. R. direkt aus den **Strukturselektoren** generiert. ([eplan.help][4])
4. **Segmentierung erkennen.** Achte auf **Vorzeichen** (`++`, `+`, `=`, `−`). **„++“** deutet **Standort**, **„+“** den **Einbauort** an. ([Iteh Standards][1])
5. **Altpläne (IEC 81346-2:2009).** Räume/Flächen konnten damals **innerhalb der U-Klasse** geführt sein; seit **2019** existiert ein **eigenes Schema für „Spaces“** (und „++“/„+“ ist beschrieben). Prüfe daher bei Altbeständen die **Legende**/Dokumentation zur Klassifikation. ([ISO][7], [Iteh Standards][2])

---

## 4) **Beispielhafte, normkonforme Muster**

> **Nur Syntaxmuster – Buchstabenklassen immer der IEC 81346-2 entnehmen.** ([Iteh Standards][2])

```text
# Site-Only (absoluter Ort)
++GEBAEUDE1++EG++R015

# Host-Only (Einbauort im Produkt)
+U1+U11+U111          # z. B. Schrank → Platte → Träger

# Kombiniert (Site + Host + Produkt)
++WERK1++HALL1 +U1+U11 −M5
```

*(Mehrstufig: Aneinanderreihung der Einzelniveaus; Nummern ohne semantische Sonderbedeutung.)* ([Readijip][5])

---

## 5) **Qualitätssicherung & Do/Don’t**

**Do**  

- **„++“ vs. „+“** strikt unterscheiden (Standort vs. Einbauort). ([Iteh Standards][1])
- **Buchstaben aus IEC 81346-2** verwenden; für Orts-/Trägerobjekte **Klasse „U“**. ([Iteh Standards][2])
- **Nummern rein sequenziell** verwenden (keine Bedeutungs-Kodierung). ([Readijip][5])
- **Platzierung** der Kennzeichen gemäß **IEC 61082-1** prüfen. ([Iteh Standards][3])

**Don’t**  

- **Buchstaben „frei“ vergeben** (z. B. „H“ für Host/Ort). **Falsch.** ([Wikipedia][6])
- **Aspekte mischen** (z. B. Host-Info in Produktaspekt stecken). Aspekte sind **unabhängig**. ([Readijip][5])

---

## 6) **Minimaler Projektstandard (empfohlen)**

1. **Aspektpolitik dokumentieren:** Welche **Site-Ebenen (`++`)** und **Host-Ebenen (`+`)** werden genutzt? (z. B. Gebäude/Geschoss/Raum sowie Schrank/Platte/Schiene). ([Iteh Standards][1])
2. **Klassifikationsliste beilegen:** Verweis auf die **IEC 81346-2:2019** (welche U-Unterklassen sind zulässig). ([Iteh Standards][2])
3. **Nummerierungsregel notieren:** **laufend, ohne Bedeutungen**; Stellenzahl optional (z. B. 1…n). ([Readijip][5])
4. **CAD-Umsetzung fixieren:** Aktivierte **Identifier-Blocks** / Struktursegmente (z. B. in EPLAN-Projektrahmen). ([eplan.help][4])
5. **Planerstprüfung:** Sichtkontrolle nach **IEC 61082-1** (Lesbarkeit, Positionierung). ([Iteh Standards][3])

---

### Quellen

- **ISO 81346-10:2022** – Host-Installation `+` und Site-Installation `++`; Mehrstufigkeit gem. IEC 81346-1. ([Iteh Standards][1])
- **IEC 81346-2:2019** – Klassifikation & Buchstaben (Hauptklasse **U** für Halte-/Lokalisiere-Objekte). ([Iteh Standards][2])
- **IEC 61082-1** – Präsentationsregeln, Position von Referenzkennzeichnungen. ([Iteh Standards][3])
- **EPLAN-Doku** – Strukturierung nach EN 81346 via Identifier-Blocks. ([eplan.help][4])
- **RDS-O\&G-Manual (2019/2020)** – Ausführliche, frei zugängliche Erläuterungen zu Aspekten, **Verkettung**, **Zähler ohne Bedeutung**. ([Readijip][5])

Dieses Vorgehen ist normenkonform, in der Praxis prozesssicher und erleichtert Suche, Montage und Instandhaltung.

[1]: https://cdn.standards.iteh.ai/samples/75471/56f3f60a9e094355865b5c6927f2c97e/ISO-81346-10-2022.pdf?utm_source=chatgpt.com "international standard iso 81346-10"
[2]: https://cdn.standards.iteh.ai/samples/75265/18f2fefeec2248278a850dd80a7a1179/IEC-81346-2-2019.pdf?utm_source=chatgpt.com "[PDF] IEC 81346-2 - iTeh Standards"
[3]: https://cdn.standards.iteh.ai/samples/19897/2d9fca205e194863a04013d515c0e149/IEC-61082-1-2014.pdf?utm_source=chatgpt.com "IEC 61082-1"
[4]: https://www.eplan.help/en-us/Infoportal/Content/Plattform/2026/Content/htm/projectstructure_k_referenzkennzeichnung.htm?utm_source=chatgpt.com "Structuring of Projects in Accordance with EN 81346"
[5]: https://readi-jip.org/wp-content/uploads/2020/06/RDS-OG-Manual-revision-1st-revision-2020-06-19.pdf "RDS-O&G manual, rev. 1"
[6]: https://de.wikipedia.org/wiki/EN_IEC_81346?utm_source=chatgpt.com "EN IEC 81346"
[7]: https://www.iso.org/standard/50858.html?utm_source=chatgpt.com "IEC 81346-2:2009 - Industrial systems, installations and ..."
