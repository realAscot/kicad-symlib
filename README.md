# **Personal KiCAD Symbol Library**

![LOGO](./.assets/logo.png)

- [**Personal KiCAD Symbol Library**](#personal-kicad-symbol-library)
  - [Informationen](#informationen)
  - [Anleitung](#anleitung)
    - [MyCustomLib – KiCad Symbol Library](#mycustomlib--kicad-symbol-library)
      - [Direkteinbindung in KiCad 9](#direkteinbindung-in-kicad-9)
  - [**Fertiger sym-lib-table-Ausschnitt**](#fertiger-sym-lib-table-ausschnitt)
  - [Betriebsmittelkennzeichnung Industrie](#betriebsmittelkennzeichnung-industrie)
    - [Kennbuchstaben (A1) nach DIN EN IEC 81346-2 2019 / DIN EN IEC 81346-2 2020-10](#kennbuchstaben-a1-nach-din-en-iec-81346-2-2019--din-en-iec-81346-2-2020-10)
    - [Auszug typische Unterklassen (A2) für die Praxis](#auszug-typische-unterklassen-a2-für-die-praxis)
  - [Abkürzungen Betriebsmittel - Elektronik](#abkürzungen-betriebsmittel---elektronik)
  - [License](#license)

## Informationen

- [x] [Weitere KiCAD Symbole](https://kicad.github.io/symbols/)

## Anleitung

Hier eine saubere **Vorlage für ein GitHub-Repository**, damit andere deine **KiCad-Symbollibrary** direkt per URL in ihre `sym-lib-table` einbinden können.

### MyCustomLib – KiCad Symbol Library

Diese Bibliothek enthält Symbole für Bauteile aus dem Schaltschrankbau.

#### Direkteinbindung in KiCad 9

1. Schaltplan-Editor öffnen → `Einstellungen → Symbolbibliotheken verwalten`
2. Tab „Globale Bibliotheken“ oder „Projektbibliotheken“
3. „Hinzufügen“ klicken (`+`)
4. Name: `MyCustomLib`
5. URL (Raw-Link):  

  ```plaintext
  [https://raw.githubusercontent.com/](https://raw.githubusercontent.com/)<USER>/<REPO>/main/MyCustomLib.kicad\_sym
  ```

6. Mit OK bestätigen – fertig.

---

## **Fertiger sym-lib-table-Ausschnitt**

```scheme
(lib (name MyCustomLib)
     (type KiCad)
     (uri https://raw.githubusercontent.com/MeinUser/my-kicad-symbols/main/MyCustomLib.kicad_sym)
     (options "")
     (descr "Eigene Symbolbibliothek von GitHub"))
```

---

## Betriebsmittelkennzeichnung Industrie

### Kennbuchstaben (A1) nach DIN EN IEC 81346-2 2019 / DIN EN IEC 81346-2 2020-10

| Kennbuchstabe | Verwendung / Funktion (Kurzfassung)                                             | Quelle                                                          |
| ------------- | ------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| A             | Nicht anzuwenden                                                                | DIN EN IEC 81346-2:2019/2020-10 (Übersichten). ([Wikipedia][1]) |
| B             | Erfassen/Darstellen von Informationen (Sensorik, Schutzrelais …)                | ([Wikipedia][1])                                                |
| C             | Speichern von Material/Energie/Information (z. B. Kondensator, Batterie)        | ([Wikipedia][1])                                                |
| D             | Für spätere Normung reserviert                                                  | ([Wikipedia][3])                                                |
| E             | **Aussenden** (z. B. Beleuchtung/Lampe, Heizung)                                | ([Wikipedia][1])                                                |
| F             | Schutz vor gefährlichen/unerwünschten Zuständen (z. B. Sicherungen, RCD)        | ([Wikipedia][1])                                                |
| G             | Bereitstellen eines steuerbaren Durchflusses/Energieflusses (Generator, Lüfter) | ([Wikipedia][1])                                                |
| H             | **Behandlung von Stoffen** (z. B. Reaktor, Zentrifuge, Filter)                  | ([Wikipedia][1])                                                |
| I             | Nicht anzuwenden                                                                | ([Wikipedia][3])                                                |
| J             | Für spätere Normung reserviert                                                  | ([Wikipedia][3])                                                |
| K             | Verarbeitung von Signalen/Information (z. B. CPU, Regler, Relais für Logik)     | ([Wikipedia][1])                                                |
| L             | Für spätere Normung reserviert                                                  | ([Wikipedia][3])                                                |
| M             | Mechanische Bewegung/Kraft ausführen (z. B. Motor, Aktor)                       | ([Wikipedia][1])                                                |
| N             | **Einschließende Objekte** (neu in 2019; z. B. Gehäuse, Dichtung)               | ([Wikipedia][1])                                                |
| O             | Nicht anzuwenden                                                                | ([Wikipedia][3])                                                |
| P             | Wahrnehmbare Information bereitstellen (Anzeige, Hupe, LED, Messgerät)          | ([Wikipedia][1])                                                |
| Q             | Zugang/Durchfluss steuern (z. B. **Schütz**, Leistungsschalter, Thyristor)      | ([Wikipedia][1])                                                |
| R             | Begrenzen/Stabilisieren (z. B. Widerstand, Drossel, Diode)                      | ([Wikipedia][1])                                                |
| S             | Menschliche Betätigung erfassen/reaktiv umsetzen (Taster, Wahlschalter)         | ([Wikipedia][1])                                                |
| T             | Transformieren (z. B. Trafo, Wandler, Verstärker)                               | ([Wikipedia][1])                                                |
| U             | Verorten/Tragen (z. B. Schrank, Montageplatte, Mast)                            | ([Wikipedia][1])                                                |
| V             | Für spätere Normung reserviert                                                  | ([Wikipedia][3])                                                |
| W             | Leiten/Führen (Kabel, Bus, LWL, Sammelschiene, Rohrleitung)                     | ([Wikipedia][1])                                                |
| X             | Schnittstellen/Verbinden (Klemmen, Steckverbinder)                              | ([Wikipedia][1])                                                |
| Y             | Für spätere Normung reserviert                                                  | ([Wikipedia][3])                                                |
| Z             | Für spätere Normung reserviert                                                  | ([Wikipedia][3])                                                |

**Normquellen/Übersichten:** Zusammenfassungen der Klassen inkl. Beispiele und Erläuterungen finden sich in den verlinkten Übersichten; die deutsche Wikipedia-Seite fasst die 2019er Ausgabe (deutsche Übernahme 2020-10) prägnant zusammen. Für Praxisbeispiele/Unterklassen existieren zudem kompakte Tabellen (z. B. IHK PAL). ([Wikipedia][1], [Industrie- und Handelskammer][4])

### Auszug typische Unterklassen (A2) für die Praxis

| Kennz. (A2) | Verwendung                                                      | Quelle                                                                                       |
| ----------- | --------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| **EA**      | **Leuchte/Lampe (Beleuchtung)**                                 | Praxisbeispiel: Leuchten als **EA**; historisch oft **H** verwendet. ([Elektropraktiker][2]) |
| **KF**      | Relais/Zeitrelais (elektrische Signale)                         | ([Industrie- und Handelskammer][4])                                                          |
| **QA**      | Schütz, Hauptschalter                                           | ([Industrie- und Handelskammer][4])                                                          |
| **SJ**      | Fingerbetätigte Ventile, **Taster/Schalter**                    | ([Industrie- und Handelskammer][4])                                                          |
| **MM**      | Motor / Zylinder (fluidische Kraft)                             | ([Industrie- und Handelskammer][4])                                                          |
| **MB**      | Ventilmagnet/Spule, Elektromagnet, Schrittmotor                 | ([Industrie- und Handelskammer][4])                                                          |
| **RN**      | Drossel-Rückschlagventil / Stromregelventil                     | ([Industrie- und Handelskammer][4])                                                          |
| **BG/BP**   | Näherungs-/Endschalter (**BG**), Druck-/Vakuumschalter (**BP**) | ([Industrie- und Handelskammer][4])                                                          |

**Hinweis zur Historik:** In vielen älteren Schaltplänen wurden **Leuchtmittel mit „-H“** und **Schütze mit „-K“** gekennzeichnet. Die aktuelle 81346-2 ordnet **Leuchten → E/EA** und **Schütze → Q/QA**. ([Elektropraktiker][2], [Wikipedia][1])

[1]: https://de.wikipedia.org/wiki/Betriebsmittel_%28Elektrotechnik%29?utm_source=chatgpt.com "Betriebsmittel (Elektrotechnik)"
[2]: https://www.elektropraktiker.de/nachrichten/nachricht/kennzeichnung-von-betriebsmitteln-leuchten?p=all&utm_source=chatgpt.com "Kennzeichnung von Betriebsmitteln (Leuchten)"
[3]: https://de.wikipedia.org/wiki/EN_IEC_81346 "EN IEC 81346 – Wikipedia"
[4]: https://www.ihk.de/blueprint/servlet/resource/blob/5090560/d005ab9b73c3e45d81920e28f72b7160/din-en-iec-81346-2-2020-10-referenzkennzeichnung-data.pdf "DIN_EN_IEC_81346_2_2020_10_Referenzkennzeichnung"

---

## Abkürzungen Betriebsmittel - Elektronik

| Abkürzung | Bauteil                 | Beschreibung                       |
|-----------|-------------------------|----------------------------------|
| R         | Widerstand              | Elektrischer Widerstand           |
| C         | Kondensator             | Elektrischer Kondensator          |
| L         | Spule / Induktivität    | Induktive Bauelemente             |
| D         | Diode                   | Halbleiter-Diode                 |
| Q         | Transistor (BJT)        | Bipolartransistor                 |
| M         | MOSFET                  | Metall-Oxid-Halbleiter-FET        |
| U         | IC (Integrierter Schaltkreis) | Integrierte Schaltung      |
| J         | Anschluss / Verbindung   | Jumper, Stecker, Verbindung       |
| F         | Sicherung               | Schmelzsicherung                 |
| S         | Schalter                | Schalter                        |
| T         | Transformator           | Elektrischer Transformator        |
| Z         | Z-Diode / Zener-Diode   | Spannungsstabilisierende Diode    |
| B         | Batterie                | Stromquelle                      |
| K         | Relais / Kontakt        | Elektromechanischer Schalter      |
| G         | Masse / Ground          | Bezugspotential / Masse           |
| X         | Bauteil, sonstiges      | Allgemeiner Platzhalter           |
| IC        | Integrierter Schaltkreis| Synonym für U, oft verwendet     |
| OPT       | Optokoppler             | Optische Kopplungseinheit         |
| LED       | Leuchtdiode             | Lichtemittierende Diode           |
| SW        | Schalter (Switch)       | Manuell bedienbarer Schalter      |
| VR        | Variabler Widerstand    | Potentiometer oder Trimmer        |
| SCR       | Thyristor               | Steuerbare Halbleiterdiode        |
| MOS       | MOSFET                  | Metall-Oxid-Halbleiter-FET        |
| MCU       | Mikrocontroller         | Mikroprozessor mit Peripherie     |
| SENSOR    | Sensor                  | Sensorisches Bauelement           |
| REL       | Relais                  | Elektromechanischer Schalter      |
| BUZ       | Power MOSFET (Bezeichnung häufig verwendet) | Spezielle MOSFET-Familie    |

---

## License

(c) 2025 - Adam Skotarczak
