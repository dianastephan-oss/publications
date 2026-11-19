# Public Publication List of the DES Chair

### Backend for our [Publications Website](https://hpi.de/en/database-group/publications/publications-data-engineering-systems-team/)

## 🇬🇧 How to add a new publication

Copy, edit, and append the following template block to [the YAML file](publications.yaml):

```
  - id: "templatePublication"
    title: "Publication Tutorial: How To Add A New Publication"
    authors:
      - "Erika Mustermann"
      - "Max Mustermann"
    venue: "WLDB '26"
    year: 2026
    type: "Conference Paper"
    abstract: >-
      In this short README, we discuss how to add new publications to the Data Engineering Systems Publications website using the GitHub backend.
    doi: "10.1145/2484848.2484848"
    bibtex: |-
      @article{templatePublication,
        author       = {Erika Mustermann and
                        Max Mustermann},
        title        = {{Publication Tutorial} How To Add A New Publication},
        journal      = {WLDB},
        volume       = {24},
        number       = {48},
        year         = {2026},
        url          = {https://hpi.de/en/database-group/publications/publications-data-engineering-systems-team/},
        doi          = {10.1145/2484848.2484848},
        timestamp    = {Tue, 29 Sep 2026 11:00:23 +0200}
        }
    artifacts:
      "Paper": "https://hpi.de/fileadmin/user_upload/90_Research_Groups/rabl/Documents/papers/2026/templatePublication.pdf"
      "Code": "https://github.com/hpides/publications"
```

- Keep every *id* unique. *abstract*, *doi*, *bibtex*, and *artifacts* may be empty (i.e., ```""``` for *abstract*, *doi* and *bibtex*, ```{}``` for *artifacts* as it expects a mapping list).

- *type* usually is one of "Conference Paper", "Workshop Paper", or "Journal Paper". For further options, check the website. New types will be added as their own group, nonetheless.

- *doi* only needs the identifier suffix after "doi.org". Whole URL-encoded DOI paths would work as well, though.

- *artifacts* can hold as many entries as needed. Links can be internal (TYPO3) and external. Papers linked internally should be saved to ```"https://hpi.de/fileadmin/user_upload/90_Research_Groups/rabl/Documents/papers/YEAR/FILENAME.pdf"```

- ```>-``` and ```|-``` are useful for formatting abstracts and BibTeX entries, respectively. You may omit them, but the following string must then be written on a single line.  ```>-``` folds line breaks into spaces, ```|-``` preserves linebreaks.


Authors that are added to the author block at the very top of the YAML file will receive an author link whenever they appear on a publication.

---

## 🇩🇪 Neue Publikationen hinzufügen

Kopiere die folgende Vorlage, passe sie an und füge sie am Ende der [YAML-Datei](publications.yaml) ein:

```
  - id: "templatePublication"
    title: "Publikationsanleitung: So fügst du eine neue Publikation hinzu"
    authors:
      - "Erika Mustermann"
      - "Max Mustermann"
    venue: "WLDB '26"
    year: 2026
    type: "Conference Paper"
    abstract: >-
      In dieser kurzen README erklären wir, wie du über das GitHub-Backend neue Publikationen zur Publikationsseite des Data-Engineering-Systems-Teams hinzufügst.
    doi: "10.1145/2484848.2484848"
    bibtex: |-
      @article{templatePublication,
        author       = {Erika Mustermann and
                        Max Mustermann},
        title        = {{Publikationsanleitung} So fügst du eine neue Publikation hinzu},
        journal      = {WLDB},
        volume       = {24},
        number       = {48},
        year         = {2026},
        url          = {https://hpi.de/en/database-group/publications/publications-data-engineering-systems-team/},
        doi          = {10.1145/2484848.2484848},
        timestamp    = {Tue, 29 Sep 2026 11:00:23 +0200}
        }
    artifacts:
      "Paper": "https://hpi.de/fileadmin/user_upload/90_Research_Groups/rabl/Documents/papers/2026/templatePublication.pdf"
      "Code": "https://github.com/hpides/publications"
```

- Jede *id* muss eindeutig sein. Die Felder *abstract*, *doi*, *bibtex* und *artifacts* dürfen leer bleiben. Verwende dafür ```""``` bei *abstract*, *doi* und *bibtex* sowie ```{}``` bei *artifacts*, da dieses Feld üblicherweise eine Zuordnung enthält.
  
- Verwende für *type* üblicherweise „Conference Paper“, „Workshop Paper“ oder „Journal Paper“. Weitere Optionen findet man auf der Website. Für jeden neuen Typ wird eine eigene Gruppe angelegt.

- Für *doi* genügt der Teil nach doi.org/. Vollständige URLs würden aber ebenfalls funktionieren.
  
- Unter *artifacts* kann man beliebig viele Einträge hinterlegen. Sowohl interne (TYPO3) als auch externe Links sind möglich. Intern verlinkte Publikationen sollten unter folgendem Pfad abgelegt werden: ```"https://hpi.de/fileadmin/user_upload/90_Research_Groups/rabl/Documents/papers/JAHR/DATEINAME.pdf"```
  
- Mit ```>-``` kann man den Abstract und mit ```|-``` den BibTeX-Eintrag über mehrere Zeilen schreiben. Wenn man diese Zeichen weglässt, muss der jeweilige Text in einer einzigen Zeile stehen. ```>-``` wandelt Zeilenumbrüche in Leerzeichen um, ```|-``` behält Zeilenumbrüche.
  
Autorinnen und Autoren, die ganz oben im Autorenblock der YAML-Datei eingetragen sind, werden bei jeder Publikation verlinkt, in der sie aufgeführt sind.
