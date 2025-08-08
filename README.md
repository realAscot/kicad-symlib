# **Personal KiCAD Symbol Library**

![LOGO](./.assets/logo.png)

- [**Personal KiCAD Symbol Library**](#personal-kicad-symbol-library)
  - [Informationen](#informationen)
  - [Anleitung](#anleitung)
    - [**Inhalt `README.md` (Beispiel)**](#inhalt-readmemd-beispiel)
      - [MyCustomLib – KiCad Symbol Library](#mycustomlib--kicad-symbol-library)
        - [Direkteinbindung in KiCad 9](#direkteinbindung-in-kicad-9)
  - [**Fertiger sym-lib-table-Ausschnitt**](#fertiger-sym-lib-table-ausschnitt)
  - [License](#license)

## Informationen

- [x] [Weitere KiCAD Symbole](https://kicad.github.io/symbols/)

## Anleitung

Hier eine saubere **Vorlage für ein GitHub-Repository**, damit andere deine **KiCad-Symbollibrary** direkt per URL in ihre `sym-lib-table` einbinden können.

### **Inhalt `README.md` (Beispiel)**

#### MyCustomLib – KiCad Symbol Library

Diese Bibliothek enthält Symbole für XYZ-Bauteile.

##### Direkteinbindung in KiCad 9

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

## License

(c) 2025 - Adam Skotarczak
