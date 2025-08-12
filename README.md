# **Personal KiCAD Symbol Library**

![LOGO](./.assets/logo.png)

- [**Personal KiCAD Symbol Library**](#personal-kicad-symbol-library)
  - [Informationen](#informationen)
  - [Anleitung](#anleitung)
    - [MyCustomLib – KiCad Symbol Library](#mycustomlib--kicad-symbol-library)
      - [Direkteinbindung in KiCad 9](#direkteinbindung-in-kicad-9)
  - [**Fertiger sym-lib-table-Ausschnitt**](#fertiger-sym-lib-table-ausschnitt)
  - [Abkürzungen Elektronik](#abkürzungen-elektronik)
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

## Abkürzungen Elektronik

```plaintext
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
```

---

## License

(c) 2025 - Adam Skotarczak
