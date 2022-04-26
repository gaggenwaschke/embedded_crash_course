# Embedded crash course

In diesem Dokument sind alle Informationen für den Embedded crash course gelistet oder gelinkt.

## Installation

Vor dem Coden, sollte die Entwicklungsmaschine folgende Tools installiert haben.
Dabei ist es sinnvoll, die Programme der Pfadvariable hinzuzufügen. Das macht später ein Aufrufen einfacher, z.B.
```gcc``` statt  ```C:\Programme\MeinEwigLangerUndNervigerPfad\gcc```.

### Programme

Name | URL | Kommentar
-|-|-
Arduino IDE | https://www.arduino.cc/en/software | Wegen der Arduino CLI und dem Plot.
Visual Studio Code | https://code.visualstudio.com/Download | Open Source IDE mit sehr vielen guten Extensions.
Ninja-Build: | https://github.com/ninja-build/ninja/releases | Build engine, ähnlich wie Make, nur besser.
CMake | https://cmake.org/download/ | Generiert gut strukturierte build Instruktionen für die Build Engine (z.B. Ninja oder Make). Kann noch einiges mehr.
Git | https://git-scm.com/downloads | Version Cotrol Tool. Organisiert und parrallelisiert Arbeit an Code. Sehr sehr viele Projekte nutzen git, manche werden auch auf git deployed.

### Einige empfehlenswerte Extensions für Visual Studio Code

Name | Visual Studio Code ID | Kommentar
-|-|-
Arduino | vsciot-vscode.vscode-arduino | Unterstützung zum Aufrufen von Arduino Commands.
C/C++ | ms-vscode.cpptools | Ermöglicht gescheites Arbeiten mit C und C++ Code.
CMake Tools | ms-vscode.cmake-tools | Syntax highlighting und Intellicense für CMake. Zeigt CMake Konfigurierte Targets and und ermöglicht es mit hübscher GUI zu bauen.
Git Graph | mhutchie.git-graph | Sehr schöne, übersichtliches GUI für git. Unterstützt aber nicht alle git Kommandos.
Git Blame | waderyan.gitblame | Werden wir wohl eher nicht brauchen, zeigt beim Markieren von Quellcode an, wer diesen zuletzt geändert hat.
