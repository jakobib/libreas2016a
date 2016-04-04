Dieses git-Repository enthält eine Artikel-Einreichung zum Thema "Wikidata als (Universal)bibliographie" für [LIBREAS](http://www.libreas.eu/) ([Q1798120](http://www.wikidata.org/entity/Q1798120)). Das [Thema der Ausgabe 29 ist Bibliographien](https://libreas.wordpress.com/2015/11/10/libreas-29-bibliographien-call-for-papers/). Die Deadline wurde auf Bitten bis zum 16.4. verlängert.

---

Der Artikel im Markdown-Format steht in der Datei `master.md` und die Metadaten
in `meta.yaml`. Die Literaturangaben sind in `bibliography.bib` enthalte. Zur
Erstellung einer HTML-Version:

    pandoc -S -s --bibliography=bibliography.bib -o master.html meta.yaml master.md
  
Die Stylesheet- und Template-Dateien `libreas-*` sind so angepasst, dass
mittels Pandoc eine HTML-Ansicht im LIBREAS-Layout erstellt werden kann (siehe
`Makefile`). Zusätzlich wird eine Kurzvita der Autoren benötigt (`vita.md`).
