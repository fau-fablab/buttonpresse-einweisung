Buttonpressen-Einweisung
=======================

Einweisung des [FAU FabLab](https://fablab.fau.de) in die [Buttonpresse](https://fablab.fau.de/tool/buttonpresse/).

Inhalt
------

- Vorlage: 56 mm Außendurchmesser der Papiervorlage, etwa 42 mm Motivfläche, Motiv ausstanzen
- Pressen Schritt für Schritt: Motiv und Folie (Markierung 1), Rückseite (Markierung 2)
- Bezahlen der Buttonrohlinge und Druckkosten

Das PDF verwendet das gemeinsame FabLab-Dokumentlayout mit Titelblock,
Versionsanzeige und verlinktem Inhaltsverzeichnis.

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/buttonpresse-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/buttonpresse-einweisung/Einweisung_Buttonpresse.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/buttonpresse-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/buttonpresse-einweisung.git
cd buttonpresse-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/buttonpresse-einweisung/status.svg)](https://brain.fablab.fau.de/build/buttonpresse-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/buttonpresse-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/buttonpresse-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/buttonpresse-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/buttonpresse-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
