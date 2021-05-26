# The Brick Museum

Nehme dein Museum mit nach Hause. So in echt. Baue es mit der ganzen Familie nach und stelle es ins Kinder- oder Wohnzimmer.

![alt text](https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum.gif "Vorschau Museum") ![alt text](https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum-small.gif "Vorschau Museum")

## Beschreibung

Museen und andere Kultureinrichtungen sind während der Corona-Pandemie für längere Zeit geschlossen. Beim Dithmarscher Landesmuseum dauert der Lockdown auf Grund von Bauarbeiten noch bis Oktober 2022 an. Derzeit besteht nur die Möglichkeit das Museum digital zu besuchen. Dazu hat das Museum seine Innenräume komplett in 3D eingescannt und stellt auf seiner Webseite einen virtuellen Rundgang bereit.

Was macht man also in einem Hackathon für ein Projekt? Bei einem, der nur remote stattfinden kann? Als Software-Entwickler? Mit super aufwändig erzeugten 3D-Daten? Einem Event, das digitale Ergebnisse erzeugt? Genau. Etwas nicht-digitales. Etwas, das man in die Hand nehmen kann. Bei einem 3D-Modell bietet sich ein 3D-Druck an. Aber nicht jeder hat einen 3D-Drucker zu Hause. Es muss also etwas simpleres sein.

Lego kennt jeder und mit Klemmbausteinen kann man Gebäude sehr gut nachbauen. Der Spaß liegt in der gesamten Familie und ist unabhängig vom Alter.

## Benutzte Daten

- [Rohdaten aus dem 3D-Scan des Dithmarscher Landesmuseums](https://codingdavinci.de/daten/rohdaten-aus-dem-3d-scan-des-dithmarscher-landesmuseums)
- [Erklär-Video zu den Daten](https://www.youtube.com/watch?v=NF7MXZgoYto)

## Projektstruktur

```
README.md       <- dieser Text
/src
   museum.io    <- Arbeitsdatei, die in Studio 2.0 geöffnet werden kann
   museum-small.io    <- Arbeitsdatei für eine kleinere Version des  Museums
/dist
   museum.gif   <- animiertes Foto
   museum.png   <- Cover-Foto
   museum.pdf   <- Aufbauanleitung
   museum-small.gif   <- animiertes Foto
   museum-small.png   <- Cover-Foto
   museum-small.pdf   <- Aufbauanleitung
```

## Wie funktioniert das Projekt

Als erstes musst du dir "Studio 2.0" auf deinem Rechner installieren. Das Programm ist für Windows und Mac verfügbar. [Lade es von hier herunter](https://www.bricklink.com/v3/studio/download.page) und installiere es. Öffne die Datei `museum.io`.

Im Studio 2.0 kannst du das Museum in 3D nachbauen. Die Farben, Formen und die Auflösung (die Steine sind ja wie Pixel in 3D) sind beschränkt. Einzelnde Steine kann man gruppieren um sie später einfacher im Modell vervielfältigen zu können (z.B. gleiche Außenfassade).

Das Modell ist angelehnt an die Lego City Reihe, die Gebäude so gestaltet haben, dass man die einzelnen Etage abnehmen kann, um bequemer darin spielen kann.

Aus dem Steine-Modell kann man eine Aufbauanleitung erstellen. Das ist ein komplett eigener Vorgang. Die Steine muss man einzelnd auf jede Seite für jeden Schritt auswählen. Am Ende entsteht der "Quelltext" für das Lego-Modell.

Aufpassen sollte man auf
* Stabilität (das Gebäude darf nicht einstürzen)
* alle Teile müssen kaufbar sein (nicht alle Formen-Farbe-Kombinationen sind lieferbar)
* der Preis sollte nicht zu hoch sein (spezielle Formen und Farben, Fenster mit "Glas" kosten mehr)
* die Anleitung sollte einfach lesbar sein (von der Schwierigkeit und vom Layout)

## Aufbauanleitung

![alt text](https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum.png "Modell des Museums")
[museum.pdf](https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum.pdf) für das große Museums-Modell

<br>

![alt text](https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum-small.png "Modell des Museums")
[museum-small.pdf](https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum-small.pdf) für das kleine Museums-Modell
