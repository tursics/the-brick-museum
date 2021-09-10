[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

# The Brick Museum

Nehme dein Museum mit nach Hause. So in echt. Baue es mit der ganzen Familie nach und stelle es ins Kinder- oder Wohnzimmer.

Da die Originaldaten unter einer CC BY-SA 4.0-Lizenz stehen, ist dieses Projekt ebenfalls unter der [Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa] lizensiert.

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg

## Aufbauanleitung

In diesem Projekt gibt es zwei Modelle vom Museum. Im großen Modell kann man die Etagen einzeln abnehmen und in das Museum hineinschauen. Im kleinen Modell ist dies nicht möglich - verbraucht aber auch deutlich weniger Steine.

|[![big-still]](https://github.com/tursics/the-brick-museum/raw/main/dist/museum.pdf)   |Das große Museums-Modell. _Der Aufbau dauert sehr lange_  |
|---------------|---------------------------|
|[![small-cover]](https://github.com/tursics/the-brick-museum/raw/main/dist/museum-small.pdf) |Das kleine Museums-Modell  |


|Museum in groß |                           |
|---------------|---------------------------|
|![big-still]   |![big-video]               |
|mit einem Blick nach innen   |  |
| |![big-still-detail]        |
|Erdgeschoss    |                           |
|![big-still-eg]   |![big-video-eg]        |
|Obergeschoss    |                           |
|![big-still-og]   |![big-video-og]        |
|Dach    |                           |
|![big-still-dach]   |        |

|Museum in klein|                           |
|---------------|---------------------------|
|![small-still] |![small-video]             |

(klicke auf ein Bild um es zu vergrößern)

## Beschreibung

Museen und andere Kultureinrichtungen sind während der Corona-Pandemie für längere Zeit geschlossen. Beim Dithmarscher Landesmuseum dauert der Lockdown auf Grund von Bauarbeiten noch bis Oktober 2022 an. Derzeit besteht nur die Möglichkeit das Museum digital zu besuchen. Dazu hat das Museum seine Innenräume komplett in 3D eingescannt und stellt auf seiner Webseite einen virtuellen Rundgang bereit.

Was macht man also in einem Hackathon für ein Projekt? Bei einem, der nur remote stattfinden kann? Als Software-Entwickler? Mit super aufwändig erzeugten 3D-Daten? Einem Event, das digitale Ergebnisse erzeugt? Genau. Etwas nicht-digitales. Etwas, das man in die Hand nehmen kann. Bei einem 3D-Modell bietet sich ein 3D-Druck an. Aber nicht jeder hat einen 3D-Drucker zu Hause. Es muss also etwas simpleres sein.

Die bunten Plastiksteine aus Dänemark kennt jeder und mit Klemmbausteinen kann man Gebäude sehr gut nachbauen. Der Spaß liegt in der gesamten Familie und ist unabhängig vom Alter.

## Benutzte Daten

- [Rohdaten aus dem 3D-Scan des Dithmarscher Landesmuseums](https://codingdavinci.de/daten/rohdaten-aus-dem-3d-scan-des-dithmarscher-landesmuseums)
- [Erklär-Video zu den Daten](https://www.youtube.com/watch?v=NF7MXZgoYto)

## Erste Ideen - erste Probleme

Das Bauen von Modellen mit Klemmbausteinen ist sehr einfach, man braucht nur eine Kiste mit entsprechend vielen Teilen. Es gibt auch Software, die einem dabei unterstützt. Mit "Studio 2.0" existiert eine kostenlose Software, die auf einem Rechner installiert werden kann und wo man seine Modelle entwirft.

**Idee 1: In "Studio 2.0" kann man 3D-Daten importieren.** Das Museum bietet 3D-Daten an und diese kann man einfach so in dem Programm importieren. Heraus fällt ein Modell aus Blöcken. Die Qualität vom Modell war ... sehr bescheiden. Es sah aus wie eine Ansammlung von 2x4-Blöcken, die nicht mal die Form eines Hauses hatte. Überall waren Löcher, der "Innenraum" war nicht vorhanden und hatte etwas von schweizer Käse.

**Das Problem:** Das 3D-Modell des Museums ist zu feingliedrig aufgebaut. Als einzige Lösung bleibt übrig, das Modell per Hand nach zu bauen. Stein für Stein. Das macht sogar mehr Sinn, weil dann auch Elemente wie Fenster, Türen, Dachsteine und Co verwendet werden können.

**Idee 2: das 3D-Modell erlaubt den Nachbau des Museums.** Das 3D-Modell ist sehr gut. Man kann bereits auf der Webseite des Museums eine Wanderung innerhalb der Räume unternehmen. Das nachbauen des Innenraums ist kein Problem. Allerdings wurden (bis auf den Innenhof) keine Außenwände aufgenommen. Das 3D-Modell enthällt keine klare Abgrenzung nach außen. Das sieht auf einem einfarbigen Modell aus wie eine schrumplige Apfelsine.

**Die Lösung / das Problem:** Um die Außenwände nachbauen zu können musste auf Fotos zugegriffen werden. Im Internet findet man einige Foto aus verschiedenen Blickwinkeln. Eine Bilddatenbank mit sehr guten Außenaufnahmen befindet sich im Museum. Das Museum wird saniert und die Rechner mit den Bildern stehen gut verstaut auf der Baustelle. Also gibt es auch nur die Bilder aus dem Internet.

## Projektstruktur

```bash
README.md            <- dieser Text
/src                 <- Quell-Ordner mit allen Arbeitsdateien
   museum.io           <- Arbeitsdatei, die in Studio 2.0 geöffnet werden kann
   museum-small.io     <- Arbeitsdatei für eine kleinere Version des Museums
/img                 <- Bilder aus dem Museum, die auf den Sticker landen werden
/ldraw               <- Grafik-Dateien für die Sticker im .dat-Format
/dist                <- Auslieferungs-Ordner für das fertige Produkt
   museum.gif          <- animiertes Foto
   museum.png          <- Cover-Foto
   museum.pdf          <- Aufbauanleitung
   museum-small.gif    <- animiertes Foto
   museum-small.png    <- Cover-Foto
   museum-small.pdf    <- Aufbauanleitung
/doc                 <- Ordner für die Dokumentation
   *                   <- alte Dateien aus dem dist-Ordner, um diese Info-Seite zu bebildern
```

## Wie funktioniert das Projekt

Als erstes musst du dir "Studio 2.0" auf deinem Rechner installieren. Das Programm ist für Windows und Mac verfügbar. [Lade es hier herunter](https://www.bricklink.com/v3/studio/download.page) und installiere es. Öffne die Datei `museum.io`.

Im Studio 2.0 kannst du das Museum in 3D nachbauen. Die Farben, Formen und die Auflösung (die Steine sind ja wie Pixel in 3D) sind beschränkt. Einzelnde Steine kann man gruppieren um sie später einfacher im Modell vervielfältigen zu können (z.B. gleiche Außenfassade).

Das Modell ist angelehnt an die L*** City Reihe, die Gebäude so gestaltet haben, dass man die einzelnen Etage abnehmen kann, um bequemer darin spielen kann. Das Modell muss entsprechend gestaltet werden, damit dies funktioniert.

Aus dem Steine-Modell kann man eine Aufbauanleitung erstellen. Das ist ein komplett eigener Vorgang. Die Steine muss man einzelnd auf jede Seite für jeden Schritt auswählen. Am Ende entsteht der "Quelltext" für das Klemmbausteine-Modell.

**Aufpassen sollte man auf**

- Stabilität (das Gebäude darf nicht einstürzen)
- alle Teile müssen kaufbar sein (nicht alle Formen-Farbe-Kombinationen sind lieferbar)
- der Preis sollte nicht zu hoch sein (spezielle Formen und Farben, Fenster mit "Glas" kosten mehr)
- die Anleitung sollte einfach lesbar sein (von der Schwierigkeit und vom Layout)

**Sticker**

An die Wände gehören Bilder. Für das Modell wird dies mit Stickern gelöst. Vom 3D-Modell des Museums werden Screenshots angefertigt und im Ordner `/img` abgelegt. Diese müssen in das `.dat`-Format umgewandelt werden, damit Studio 2.0 sie verwenden kann.

- PNG-Bilder können [auf dieser Webseite](https://brickhub.org/i/apps/sticker_builder.htm) konvertiert werden
- SVG-Bilder könnnen [auf dieser Webseite](https://www.c-mt.dk/software/svg2ldraw/) konvertiert werden
- größere Bilder müssen ggf. in mehrere kleinere Bilder zerlegt werden. Das [Online-Tool](https://pinetools.com/split-image) hilft dabei.

Die Dateien müssen in einer speziellen Ordner-Struktur im Verzeichnis `/ldraw` abelegt werden. Der komplette Ordner muss nach `~/Application/Studio 2.0/ldraw` kopiert werden (oder ein Symlink erstellt werden).

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
|![big-still-7]  |![big-video-7]  |bessere Stirnseite und Dachfenster  |
|![big-still-8]  |![big-video-8]  |die Rückseite wurde gestaltet  |
|                |![big-still]    |aktuelle Version  |

Danach kam der Innenausbau:

|Erdgeschoss      |Obergeschoss      |Dach      |Kommentar  |
|-----------------|-----------------|-----------------|-----------|
|![big-still-8-eg]|![big-still-8-og]|![big-still-8-dach]|noch ist nur die Außenhülle zu sehen  |
|![big-still-9-eg]|![big-video-9-eg]|  |Parkett und Holzbalken werden im Erdgeschoss verlegt  |
|![big-still-10-eg]|![big-video-10-eg]|  |Alle Fenster werden verhangen und die Treppe eingesetzt  |
| |![big-still-10-og]|![big-video-10-og]| Das gleiche für das Obergeschoss  |

An die Wände gehören Bilder. Für das Modell wird dies mit Stickern gelöst.

|Bild                    |Kommentar  |
|------------------------|-----------|
| |![big-still-9-detail]| Die ersten 3 Bilder hängen an der Wand  |

---

Für das zweite Modell gibt es auch ältere Bilder:

|Foto            |Animiert        |Kommentar  |
|----------------|----------------|-----------|
|![small-still-1]|![small-video-1]|erste Version  |
|![small-still-2]|![small-video-2]|auch hier ist die Stirnseite modelliert worden  |
|![small-still-3]|![small-video-3]|ein erstes vollständiges Haus, mit schrägem Dach |
 |                |![small-still]  |aktuelle Version  |

[big-still]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum.png "Modell des Museums"
[big-still-1]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-1.png "älteres Modell des Museums"
[big-still-2]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-2.png "älteres Modell des Museums"
[big-still-3]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-3.png "älteres Modell des Museums"
[big-still-4]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-4.png "älteres Modell des Museums"
[big-still-5]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-5.png "älteres Modell des Museums"
[big-still-6]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-6.png "älteres Modell des Museums"
[big-still-7]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-7.png "älteres Modell des Museums"
[big-still-8]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-8.png "älteres Modell des Museums"
[big-still-9]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-9.png "älteres Modell des Museums"
[big-still-10]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-10.png "älteres Modell des Museums"

[big-still-detail]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-detail.png "Modell des Museums von innen"
[big-still-8-detail]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-8-detail.png "älteres Modell des Museums von innen"
[big-still-9-detail]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-9-detail.png "älteres Modell des Museums von innen"
[big-still-10-detail]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-10-detail.png "älteres Modell des Museums von innen"

[big-still-eg]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-eg.png "Modell des Museums"
[big-still-8-eg]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-8-eg.png "älteres Modell des Museums"
[big-still-9-eg]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-9-eg.png "älteres Modell des Museums"
[big-still-10-eg]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-10-eg.png "älteres Modell des Museums"

[big-still-og]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-og.png "Modell des Museums"
[big-still-8-og]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-8-og.png "älteres Modell des Museums"
[big-still-9-og]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-9-og.png "älteres Modell des Museums"
[big-still-10-og]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-10-og.png "älteres Modell des Museums"

[big-still-dach]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-dach.png "Modell des Museums"
[big-still-8-dach]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-8-dach.png "älteres Modell des Museums"
[big-still-9-dach]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-9-dach.png "älteres Modell des Museums"
[big-still-10-dach]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-10-dach.png "älteres Modell des Museums"

[small-still]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-small.png "kleines Modell des Museums"
[small-still-1]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-1.png "kleines, älteres Modell des Museums"
[small-still-2]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-2.png "kleines, älteres Modell des Museums"
[small-still-3]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-3.png "kleines, älteres Modell des Museums"
[small-still-4]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-4.png "kleines, älteres Modell des Museums"
[small-still-5]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-5.png "kleines, älteres Modell des Museums"
[small-still-6]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-6.png "kleines, älteres Modell des Museums"
[small-still-7]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-7.png "kleines, älteres Modell des Museums"
[small-still-8]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-8.png "kleines, älteres Modell des Museums"
[small-still-9]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-9.png "kleines, älteres Modell des Museums"
[small-still-10]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-10.png "kleines, älteres Modell des Museums"

[big-video]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum.gif "animiertes Modell des Museums"
[big-video-1]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-1.gif "animiertes, älteres Modell des Museums"
[big-video-2]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-2.gif "animiertes, älteres Modell des Museums"
[big-video-3]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-3.gif "animiertes, älteres Modell des Museums"
[big-video-4]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-4.gif "animiertes, älteres Modell des Museums"
[big-video-5]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-5.gif "animiertes, älteres Modell des Museums"
[big-video-6]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-6.gif "animiertes, älteres Modell des Museums"
[big-video-7]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-7.gif "animiertes, älteres Modell des Museums"
[big-video-8]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-8.gif "animiertes, älteres Modell des Museums"
[big-video-9]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-9.gif "animiertes, älteres Modell des Museums"
[big-video-10]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-10.gif "animiertes, älteres Modell des Museums"

[big-video-eg]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-eg.gif "animiertes Modell vom Erdgeschoss"
[big-video-9-eg]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-9-eg.gif "animiertes, älteres Modell vom Erdgeschoss"
[big-video-10-eg]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-10-eg.gif "animiertes, älteres Modell vom Erdgeschoss"

[big-video-og]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-og.gif "animiertes Modell vom Obergeschoss"
[big-video-9-og]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-9-og.gif "animiertes, älteres Modell vom Obergeschoss"
[big-video-10-og]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-10-og.gif "animiertes, älteres Modell vom Obergeschoss"

[small-video]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-small.gif "kleines animiertes Modell des Museums"
[small-video-1]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-1.gif "kleines animiertes älteres Modell des Museums"
[small-video-2]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-2.gif "kleines animiertes älteres Modell des Museums"
[small-video-3]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-3.gif "kleines animiertes älteres Modell des Museums"
[small-video-4]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-4.gif "kleines animiertes älteres Modell des Museums"
[small-video-5]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-5.gif "kleines animiertes älteres Modell des Museums"
[small-video-6]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-6.gif "kleines animiertes älteres Modell des Museums"
[small-video-7]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-7.gif "kleines animiertes älteres Modell des Museums"
[small-video-8]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-8.gif "kleines animiertes älteres Modell des Museums"
[small-video-9]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-9.gif "kleines animiertes älteres Modell des Museums"
[small-video-10]: https://github.com/tursics/the-brick-museum/raw/main/doc/museum-small-10.gif "kleines animiertes älteres Modell des Museums"

[small-cover]: https://github.com/tursics/the-brick-museum/raw/main/dist/museum-small-cover.png "kleines animiertes älteres Modell des Museums"

## Metadaten zum kleinen Modell

- Breite: 11,2 cm
- Länge: 8,8 cm
- Höhe: 8,3 cm
- Gewicht: 221,9 g
- Teile: 439
- Unterschiedliche Teile: 38
- Gesamtpreis: 40,578 USD (35 Euro laut Währungsrechner)
