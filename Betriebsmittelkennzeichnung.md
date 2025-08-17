# Betriebsmittelkennzeichnung in der Elektrotechnik – Alt vs. Neu

> von Adam Skotarczak <adam@Skotarczak.net>  
> Dokument Aktuell in Bearbeitung

## Inhalt

- [Betriebsmittelkennzeichnung in der Elektrotechnik – Alt vs. Neu](#betriebsmittelkennzeichnung-in-der-elektrotechnik--alt-vs-neu)
  - [Inhalt](#inhalt)
  - [1. Hintergrund und Ziel der Betriebsmittelkennzeichnung](#1-hintergrund-und-ziel-der-betriebsmittelkennzeichnung)
  - [2. Die alte Norm: DIN 40719-2 und ihre Nachfolger](#2-die-alte-norm-din-40719-2-und-ihre-nachfolger)
    - [2.1 Historie](#21-historie)
    - [2.2 Kennbuchstaben (alte Logik)](#22-kennbuchstaben-alte-logik)
  - [3. Die neue Norm: DIN EN IEC 81346-2 2020-10](#3-die-neue-norm-din-en-iec-81346-2-2020-10)
    - [3.1 Geltung und Einführung](#31-geltung-und-einführung)
    - [3.2 Zielsetzung der neuen Norm](#32-zielsetzung-der-neuen-norm)
    - [3.3 Beispiel: SPS](#33-beispiel-sps)
  - [4. Alt vs. Neu im Vergleich](#4-alt-vs-neu-im-vergleich)
  - [5. Wann die neue Norm anzuwenden ist](#5-wann-die-neue-norm-anzuwenden-ist)
    - [5.1 Rechtliche Lage](#51-rechtliche-lage)
    - [5.2 Praxis](#52-praxis)
  - [6. Wichtige Unterschiede, die Umsteiger beachten müssen](#6-wichtige-unterschiede-die-umsteiger-beachten-müssen)
  - [6.1 Empfehlung für die Umstellung](#61-empfehlung-für-die-umstellung)
  - [6.2 Alt- vs. Neu-Kennbuchstaben](#62-alt--vs-neu-kennbuchstaben)
  - [6.3 Wichtige Umstellungsregeln](#63-wichtige-umstellungsregeln)
  - [7. Fazit](#7-fazit)

## 1. Hintergrund und Ziel der Betriebsmittelkennzeichnung

Die Betriebsmittelkennzeichnung dient dazu, **technische Komponenten in Schaltplänen, Stücklisten und auf dem Objekt eindeutig zu identifizieren**.
In der Elektrotechnik – besonders im industriellen Anlagenbau – ermöglicht sie:

- **Eindeutige Zuordnung** zwischen Plan, Gerät und Funktion
- **Effiziente Wartung** und Fehlersuche
- **Normgerechte Dokumentation** für Kunden, Behörden und CE-Kennzeichnung

Über Jahrzehnte gab es unterschiedliche Systeme in Deutschland und international, was zu **Inkompatibilitäten** geführt hat.
Heute gilt in Deutschland und der EU die **DIN EN IEC 81346-2**, die ältere nationale Normen abgelöst hat.

---

## 2. Die alte Norm: DIN 40719-2 und ihre Nachfolger

### 2.1 Historie

- **DIN 40719-2**: In Deutschland bis ca. 1995 Standard für Funktionskennzeichnung elektrischer Betriebsmittel.
- Abgelöst durch **DIN EN 61346-2** (1998), die erste internationale Anpassung.
- Letzte Revision: **DIN EN 61346-2:2009**, mittlerweile ersetzt.

### 2.2 Kennbuchstaben (alte Logik)

In der alten DIN 40719 waren die Kennbuchstaben stark praxisorientiert. Beispiele:

| Alt (DIN 40719) | Typische Bedeutung                    | Beispiel                     |
| --------------- | ------------------------------------- | ---------------------------- |
| A               | Baugruppen, Aggregate, SPS-E/A-Module | Siemens SM 321 Digital Input |
| E               | Erzeuger                              | Generator                    |
| F               | Sicherungen                           | Leitungsschutzschalter       |
| H               | Signalisierung                        | Lampe, Summer                |
| K               | Schaltrelais                          | Hilfsrelais                  |
| M               | Motoren                               | Drehstrommotor               |
| S               | Schalter, Taster                      | Hauptschalter                |
| T               | Transformatoren                       | Netztrafo                    |
| X               | Klemmen                               | Reihenklemme                 |

➡ Vorteil: **Intuitiv** für Praktiker, die Kennung oft selbsterklärend.  
➡ Nachteil: **Unterschiedliche Systeme** in verschiedenen Ländern, Überschneidungen, fehlende Einheitlichkeit für andere Gewerke.  

---

## 3. Die neue Norm: DIN EN IEC 81346-2 2020-10

### 3.1 Geltung und Einführung

- Internationale Norm: **IEC 81346-2:2019**
- Europäische Übernahme: **EN IEC 81346-2:2019**
- Deutsche Übernahme: **DIN EN IEC 81346-2:2020-10**
- Ersetzt **DIN EN 61346-2:2009** vollständig.
- In Deutschland seit 2020 gültig.
- In der Industrie **empfohlen** und in manchen Bereichen faktisch vorgeschrieben, wenn harmonisierte Normen über die Maschinenrichtlinie gefordert werden.

### 3.2 Zielsetzung der neuen Norm

- **Gewerkeübergreifend** nutzbar (Elektrotechnik, Mechanik, Verfahrenstechnik)
- **Eindeutigkeit**: Kein Buchstabe steht mehr für völlig unterschiedliche Dinge in verschiedenen Branchen.
- **Flexibilität** durch Unterklassen (A1, A2, A3)
- **Internationale Kompatibilität**

### 3.3 Beispiel: SPS

- SPS-CPU → **K** (Verarbeitung von Signalen)
- SPS-Eingangs-/Ausgangsmodul → **K** (sofern keine Schutzfunktion)
- Sicherheits-SPS → **F** (Schutzfunktion)

---

## 4. Alt vs. Neu im Vergleich

| Alt (DIN 40719) | Neu (DIN EN IEC 81346-2) | Bemerkung                                              |
| --------------- | ------------------------ | ------------------------------------------------------ |
| A = Baugruppe   | Nicht belegt             | Heute meist **K** oder **B**, je nach Funktion         |
| H = Lampe       | E = Aussenden            | E/EA für Beleuchtung, H heute „Behandlung von Stoffen“ |
| K = Relais      | Q oder K                 | K für Logikrelais, Q für Leistungsschalter/Schütze     |
| M = Motor       | M                        | Unverändert in der Grundbedeutung                      |
| S = Schalter    | S                        | Unverändert in der Grundbedeutung                      |
| T = Trafo       | T                        | Unverändert                                            |
| X = Klemme      | X                        | Unverändert                                            |

---

## 5. Wann die neue Norm anzuwenden ist

### 5.1 Rechtliche Lage

- **Normen sind freiwillig** – außer sie werden:

  - In Gesetzen/Verordnungen genannt (z. B. Maschinenrichtlinie → harmonisierte Norm)
  - Vertragsbestandteil
  - Teil interner Werksnormen
- Für **CE-pflichtige Maschinen** gilt:
  Anwendung harmonisierter Normen schafft **Vermutungswirkung** (Erleichterung bei Konformitätsbewertung).
- In vielen Großunternehmen ist 81346 **intern vorgeschrieben**.

### 5.2 Praxis

- **Neuprojekte** → dringend empfohlen, gleich 81346 zu nutzen.
- **Bestandsanlagen** → keine Pflicht zur Umkennzeichnung, aber bei Erweiterungen ist eine Mischung möglich – sollte dokumentiert sein.
- **Dokumentation für Kunden** → wenn der Kunde 81346 fordert, ist das verbindlich.

---

## 6. Wichtige Unterschiede, die Umsteiger beachten müssen

1. **Ein Buchstabe = eine Funktionsklasse**

   - Alte „H = Lampe“ geht nicht mehr → jetzt „E“
   - „A = SPS-Modul“ gibt es nicht mehr → jetzt „K“
2. **Schutzfunktion vs. Steuerfunktion trennen**

   - Sicherheits-SPS und Sicherheitsrelais → **F**
   - Normale Steuergeräte → **K**
3. **Unterklassen nutzen**

   - Hauptklasse „E“ → Unterklasse „EA“ für Lampe, „EH“ für Heizung
4. **Mehr als Elektrotechnik**

   - Norm gilt auch für mechanische und verfahrenstechnische Betriebsmittel → Kennbuchstaben sind universeller.
5. **Interne Übergangslösungen**

   - Falls Umstellung nicht sofort möglich, klare Zuordnungstabelle „alt → neu“ erstellen und in der Projektdokumentation führen.

---

## 6.1 Empfehlung für die Umstellung

- **Schrittweise Migration**:

  - Bei Neuprojekten sofort 81346 anwenden.
  - Bei Umbauten bestehender Anlagen: neue Betriebsmittel nach 81346 kennzeichnen, alte Kennungen in Klammern beibehalten.
- **Legende beilegen**:

  - Alte und neue Buchstaben in den Plänen erklären.
- **Schulungen intern**:

  - Elektriker und Konstrukteure müssen die neue Systematik verstehen.
- **CAD-System vorbereiten**:

  - QElectroTech, EPLAN, WSCAD etc. auf 81346 umstellen und interne Makros/Artikeldaten anpassen.

## 6.2 Alt- vs. Neu-Kennbuchstaben

| Alt (DIN 40719 / Praxis) | Typische Bedeutung alt                                | Neu (DIN EN IEC 81346-2:2020-10) | Neue Funktionsklasse (A1) / Hinweis |
|--------------------------|------------------------------------------------------|-----------------------------------|--------------------------------------|
| A                        | Baugruppe, SPS-E/A-Modul, Aggregat                   | K oder B                          | K = Steuerlogik (CPU, I/O-Module), B = Erfassen (Messmodule) |
| B                        | Signallampe / Summer (manchmal auch Messgerät)       | P                                 | P = Information bereitstellen (Anzeige, Summer) |
| C                        | Kondensator                                          | C                                 | C = Speichern von Energie |
| D                        | Gleichrichter, Ladegerät                              | G oder T                          | G = Energie bereitstellen, T = Transformieren, je nach Funktion |
| E                        | Erzeuger (Generator)                                 | G                                 | G = Energie bereitstellen |
| F                        | Sicherung, FI, LS-Schalter                           | F                                 | F = Schutzobjekt |
| G                        | Signalgeber (akustisch/optisch)                      | P                                 | P = Anzeige/Hupe |
| H                        | Lampe / Leuchte                                      | E (EA)                            | E = Aussenden, EA = Beleuchtung |
| K                        | Relais, Schütz                                       | K oder Q                          | K = Logikrelais, Q = Schütz/Leistungsschalter |
| L                        | Spule, Magnetventilspule                             | M oder Q                          | M = mechanische Bewegung (Magnet), Q = Leistungsschalter |
| M                        | Motor                                                | M                                 | M = mechanische Bewegung |
| N                        | Erdungspunkt / Neutralleiter                         | W                                 | W = Leiten/Führen |
| P                        | Messgerät                                            | P                                 | P = Anzeigen |
| Q                        | Leistungsschalter                                    | Q                                 | Q = Durchfluss/Energiefluss steuern |
| R                        | Widerstand                                           | R                                 | R = Begrenzen/Stabilisieren |
| S                        | Schalter, Taster                                     | S                                 | S = Menschliche Betätigung |
| T                        | Transformator                                        | T                                 | T = Transformieren |
| U                        | Steckdose                                            | X                                 | X = Schnittstelle/Verbinden |
| V                        | Ventil                                               | Q                                 | Q = Durchfluss steuern |
| W                        | Kabel, Leitung                                       | W                                 | W = Leiten/Führen |
| X                        | Klemme                                               | X                                 | X = Schnittstelle |
| Y                        | Spezialgerät (sonst nicht zuordenbar)                | je nach Funktion                  | Funktion ermitteln und zuordnen |
| Z                        | Zeitschaltuhr                                        | K oder F                          | K = Logik, F = Schutzfunktion |

---

## 6.3 Wichtige Umstellungsregeln

1. **Funktion entscheidet, nicht Bauform**

   - Eine SPS-CPU mit Sicherheitsfunktion → **F**, nicht **K**.
   - Ein Relais, das Motoren schaltet → **Q**, nicht **K**.

2. **Unterklassen nutzen**

   - E → EA (Lampe), EH (Heizung)
   - F → FA (Leitungsschutzschalter), FB (FI-Schalter)
   - K → KA (CPU), KB (I/O-Modul)

3. **Bei Mischanlagen**

   - Altkennungen in Klammern beibehalten, z. B.: `=K1 (alt: -A1)`
   - Legende in der Dokumentation hinterlegen.

4. **Häufige Stolperfallen**

   - H ist **nicht** mehr Lampe → jetzt **E/EA**.
   - A ist **nicht** mehr Baugruppe → je nach Funktion **K** oder **B**.
   - K ist **nicht** automatisch Schütz → für Leistungsschütze **Q**.

---

## 7. Fazit

Die Umstellung von DIN 40719/DIN EN 61346 auf **DIN EN IEC 81346-2** ist mehr als ein reiner Buchstabentausch – es ist ein **Paradigmenwechsel**:

- **Von elektrospezifisch → zu gewerkeübergreifend**
- **Von historisch gewachsenen Kürzeln → zu klarer Funktionslogik**
- **Von Deutschland-Standard → zu internationaler Vereinheitlichung**

Für dich als Praktiker bedeutet das:

- Du musst einige liebgewonnene Kennbuchstaben ablegen (H = Lampe, A = Baugruppe …)
- Dafür bekommst du ein System, das weltweit verstanden wird, eindeutig ist und langfristig verpflichtend sein wird.

Hier ist die **Alt-/Neu-Umsetzungstabelle** für Betriebsmittelkennzeichnungen –
links die alte DIN 40719-2 (bzw. gängige Industrie-Praxis), rechts die neue DIN EN IEC 81346-2:2020-10.

---
