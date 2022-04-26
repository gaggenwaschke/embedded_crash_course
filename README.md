# Embedded crash course

In diesem Dokument sind alle Informationen für den Embedded crash course gelistet oder gelinkt.

## Installation

Vor dem Coden, sollte die Entwicklungsmaschine folgende Tools installiert haben.
Dabei ist es sinnvoll, die Programme der Pfadvariable hinzuzufügen.
Das macht später ein Aufrufen einfacher, z.B.
```gcc``` statt  ```C:\Programme\MeinEwigLangerUndNervigerPfad\gcc```.

Programm | URL | Kommentar
-|-|-
Arduino IDE | https://www.arduino.cc/en/software | Wegen der Arduino CLI und dem Plot.
Visual Studio Code | https://code.visualstudio.com/Download | Open Source IDE mit sehr vielen guten Extensions.
Ninja-Build: | https://github.com/ninja-build/ninja/releases | Build engine, ähnlich wie Make, nur besser.
CMake | https://cmake.org/download/ | Generiert gut strukturierte build Instruktionen für die Build Engine (z.B. Ninja oder Make). Kann noch einiges mehr.
Git | https://git-scm.com/downloads | Version Cotrol Tool. Organisiert und parrallelisiert Arbeit an Code. Sehr sehr viele Projekte nutzen git, manche werden auch auf git deployed.

Einige empfehlenswerte Extensions für Visual Studio Code:

Extension Name | Visual Studio Code ID | Kommentar
-|-|-
Arduino | vsciot-vscode.vscode-arduino | Unterstützung zum Aufrufen von Arduino Commands. In den Entsprechenden Einstellungen den Pfad zur Arduino Installation einstellen.
C/C++ Extension Pack | ms-vscode.cpptools-extension-pack | Ermöglicht gescheites Arbeiten mit C und C++ Code.
CMake Tools | ms-vscode.cmake-tools | Syntax highlighting und Intellicense für CMake. Zeigt CMake Konfigurierte Targets and und ermöglicht es mit hübscher GUI zu bauen.
Git Graph | mhutchie.git-graph | Sehr schöne, übersichtliches GUI für git. Unterstützt aber nicht alle git Kommandos.
Git Blame | waderyan.gitblame | Werden wir wohl eher nicht brauchen, zeigt beim Markieren von Quellcode an, wer diesen zuletzt geändert hat.

Jetzt brauchen wir noch die Board extension für den Arduino Nano 33. Dafür muss man ```strg+shift+p``` drücken. Das bringt einen in die allgemeine Visual Studio Code Kommando Palette. Von hier aus kann man Extensions und Built Ins aufrufen.
Hier sucht man jetzt nach "Arduino: Board Manager" und öffnet Diesen.

Dann sucht man nach "Arduino Mbed OS Nano Boards" und installiert diese. Wenn die Installation durch ist, kann man mit ```strg+shit+p``` wieder in die Kommandopalette und diesmal "Arduino: Board Config" aufrufen. Dort wählt man "Arduino NANO 33 BLE" aus.

Jetzt wird über die Kommandopalette noch der Serielle Port für den Arduino ausgewählt und dann kann man den ersten Sketch kompilieren und hochladen.

## Datenblätter

Es macht für alle Sinn, das Datenblatt des verwendeten Controllers und das Datenblatt des Arduino griffbereit zu haben:
- [Controller](https://infocenter.nordicsemi.com/pdf/nRF52840_PS_v1.7.pdf)
- [Arduino Nano33 BLE](https://docs.arduino.cc/static/505e27403b33044763004a5453e012d7/ABX00030-datasheet.pdf)