# The Brick Museum

Nehme dein Museum mit nach Hause. So in echt. Baue es mit der ganzen Familie nach und stelle es ins Kinder- oder Wohnzimmer.

![big-video] ![small-video]

## Beschreibung

Museen und andere Kultureinrichtungen sind während der Corona-Pandemie für längere Zeit geschlossen. Beim Dithmarscher Landesmuseum dauert der Lockdown auf Grund von Bauarbeiten noch bis Oktober 2022 an. Derzeit besteht nur die Möglichkeit das Museum digital zu besuchen. Dazu hat das Museum seine Innenräume komplett in 3D eingescannt und stellt auf seiner Webseite einen virtuellen Rundgang bereit.

Was macht man also in einem Hackathon für ein Projekt? Bei einem, der nur remote stattfinden kann? Als Software-Entwickler? Mit super aufwändig erzeugten 3D-Daten? Einem Event, das digitale Ergebnisse erzeugt? Genau. Etwas nicht-digitales. Etwas, das man in die Hand nehmen kann. Bei einem 3D-Modell bietet sich ein 3D-Druck an. Aber nicht jeder hat einen 3D-Drucker zu Hause. Es muss also etwas simpleres sein.

Lego kennt jeder und mit Klemmbausteinen kann man Gebäude sehr gut nachbauen. Der Spaß liegt in der gesamten Familie und ist unabhängig vom Alter.

## Benutzte Daten

- [Rohdaten aus dem 3D-Scan des Dithmarscher Landesmuseums](https://codingdavinci.de/daten/rohdaten-aus-dem-3d-scan-des-dithmarscher-landesmuseums)
- [Erklär-Video zu den Daten](https://www.youtube.com/watch?v=NF7MXZgoYto)

## Projektstruktur

```bash
README.md            <- dieser Text
/src                 <- Quell-Ordner mit allen Arbeitsdateien
   museum.io           <- Arbeitsdatei, die in Studio 2.0 geöffnet werden kann
   museum-small.io     <- Arbeitsdatei für eine kleinere Version des Museums
/dist                <- Auslieferungs-Ordner für das fertige Produkt
   museum.gif          <- animiertes Foto
   museum.png          <- Cover-Foto
   museum.pdf          <- Aufbauanleitung
   museum-small.gif    <- animiertes Foto
   museum-small.png    <- Cover-Foto
   museum-small.pdf    <- Aufbauanleitung
/doc                 <- Ordner für die Dokumentation
   *                   <- alte Dateien aus dem dist-Ordner
```

## Wie funktioniert das Projekt

Als erstes musst du dir "Studio 2.0" auf deinem Rechner installieren. Das Programm ist für Windows und Mac verfügbar. [Lade es von hier herunter](https://www.bricklink.com/v3/studio/download.page) und installiere es. Öffne die Datei `museum.io`.

Im Studio 2.0 kannst du das Museum in 3D nachbauen. Die Farben, Formen und die Auflösung (die Steine sind ja wie Pixel in 3D) sind beschränkt. Einzelnde Steine kann man gruppieren um sie später einfacher im Modell vervielfältigen zu können (z.B. gleiche Außenfassade).

Das Modell ist angelehnt an die Lego City Reihe, die Gebäude so gestaltet haben, dass man die einzelnen Etage abnehmen kann, um bequemer darin spielen kann.

Aus dem Steine-Modell kann man eine Aufbauanleitung erstellen. Das ist ein komplett eigener Vorgang. Die Steine muss man einzelnd auf jede Seite für jeden Schritt auswählen. Am Ende entsteht der "Quelltext" für das Lego-Modell.

Aufpassen sollte man auf

- Stabilität (das Gebäude darf nicht einstürzen)
- alle Teile müssen kaufbar sein (nicht alle Formen-Farbe-Kombinationen sind lieferbar)
- der Preis sollte nicht zu hoch sein (spezielle Formen und Farben, Fenster mit "Glas" kosten mehr)
- die Anleitung sollte einfach lesbar sein (von der Schwierigkeit und vom Layout)

## Aufbauanleitung

![big-still]
[museum.pdf](https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum.pdf) für das große Museums-Modell

![small-still]
[museum-small.pdf](https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum-small.pdf) für das kleine Museums-Modell

## Entstehung

Ich bleibe gerne an Bauzäunen stehen und schaue mir den Fortschritt an. Damit du das auch kannst, kommen jetzt ein paar Bilder von früheren Versionen des Museums. Viel Spaß damit (mit einem klick auf das Bild erscheint es in besserer Auflösung).

|Foto            |Animiert        |Kommentar  |
|----------------|----------------|-----------|
|![big-still-1]  |![big-video-1]  |erste Version  |
|![big-still-2]  |![big-video-2]  |eine erste Mauer  |
|![big-still-3]  |![big-video-3]  |mit zweiter Etage  |
|![big-still-4]  |![big-video-4]  |von zwei Seiten (sieht fast schon aus wie ein Haus)  |
|![big-still-5]  |![big-video-5]  |die Stirnseite kommt hinzu  |
|![big-still-6]  |![big-video-6]  |mit Dach  |
|                |![big-still]    |aktuelle Version  |

Für das zweite Modell gibt es auch ältere Bilder:

|Foto            |Animiert        |Kommentar  |
|----------------|----------------|-----------|
|![small-still-1]|![small-video-1]|erste Version  |
|![small-still-2]|![small-video-2]|auch hier ist die Stirnseite modelliert worden  |
|                |![small-still]  |aktuelle Version  |

[big-still]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum.png "Modell des Museums"
[big-still-1]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-1.png "älteres Modell des Museums"
[big-still-2]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-2.png "älteres Modell des Museums"
[big-still-3]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-3.png "älteres Modell des Museums"
[big-still-4]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-4.png "älteres Modell des Museums"
[big-still-5]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-5.png "älteres Modell des Museums"
[big-still-6]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-6.png "älteres Modell des Museums"
[big-still-7]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-7.png "älteres Modell des Museums"
[big-still-8]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-8.png "älteres Modell des Museums"
[big-still-9]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-9.png "älteres Modell des Museums"
[big-still-10]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-10.png "älteres Modell des Museums"
[small-still]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum-small.png "kleines Modell des Museums"
[small-still-1]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-1.png "kleines, älteres Modell des Museums"
[small-still-2]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-2.png "kleines, älteres Modell des Museums"
[small-still-3]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-3.png "kleines, älteres Modell des Museums"
[small-still-4]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-4.png "kleines, älteres Modell des Museums"
[small-still-5]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-5.png "kleines, älteres Modell des Museums"
[small-still-6]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-6.png "kleines, älteres Modell des Museums"
[small-still-7]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-7.png "kleines, älteres Modell des Museums"
[small-still-8]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-8.png "kleines, älteres Modell des Museums"
[small-still-9]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-9.png "kleines, älteres Modell des Museums"
[small-still-10]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-10.png "kleines, älteres Modell des Museums"
[big-video]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum.gif "animiertes Modell des Museums"
[big-video-1]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-1.gif "animiertes, älteres Modell des Museums"
[big-video-2]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-2.gif "animiertes, älteres Modell des Museums"
[big-video-3]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-3.gif "animiertes, älteres Modell des Museums"
[big-video-4]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-4.gif "animiertes, älteres Modell des Museums"
[big-video-5]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-5.gif "animiertes, älteres Modell des Museums"
[big-video-6]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-6.gif "animiertes, älteres Modell des Museums"
[big-video-7]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-7.gif "animiertes, älteres Modell des Museums"
[big-video-8]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-8.gif "animiertes, älteres Modell des Museums"
[big-video-9]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-9.gif "animiertes, älteres Modell des Museums"
[big-video-10]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-10.gif "animiertes, älteres Modell des Museums"
[small-video]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/dist/museum-small.gif "kleines animiertes Modell des Museums"
[small-video-1]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-1.gif "kleines animiertes älteres Modell des Museums"
[small-video-2]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-2.gif "kleines animiertes älteres Modell des Museums"
[small-video-3]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-3.gif "kleines animiertes älteres Modell des Museums"
[small-video-4]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-4.gif "kleines animiertes älteres Modell des Museums"
[small-video-5]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-5.gif "kleines animiertes älteres Modell des Museums"
[small-video-6]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-6.gif "kleines animiertes älteres Modell des Museums"
[small-video-7]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-7.gif "kleines animiertes älteres Modell des Museums"
[small-video-8]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-8.gif "kleines animiertes älteres Modell des Museums"
[small-video-9]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-9.gif "kleines animiertes älteres Modell des Museums"
[small-video-10]: https://git.chaotikum.org/tursics/3d-druck-ohne-3d-druck/-/raw/main/doc/museum-small-10.gif "kleines animiertes älteres Modell des Museums"
