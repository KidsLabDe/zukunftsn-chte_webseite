# Generierung von Karten

## Grundlagen

Wir nutzen in Minetest eine Mod von  Florian Rädiker: world2minetest ([https://github.com/FlorianRaediker/world2minetest](https://github.com/FlorianRaediker/world2minetest))

Diese nutzt die Daten von OpenStreetMaps und erzeugt die Strukturen in diese in Minetest

1. Über ein Python-Skript werden die "Features" aus OSM geladen und als JSON-Datei abgelegt
2. Aus diesen Daten wir eine Datei namens `map.dat` erzeugt
3. Eine Mod in Minetest liest die Datei und erzeugt die Strukturen in Minetest, sobald dieser Teil der Welt geladen wird.

Unsere aktuell verwendete Version (mit einigen Bugfixes) ist als Fork hier: [https://github.com/holgerm/world2minetest](https://github.com/holgerm/world2minetest)

## Erstellung der Karten für Minetest

### Vorbereiten der Python Installation

Normalerweise sollte Python bereits mit allen benötigten Modulen installiert sein. Wenn nicht, und man erhält einen entsprechenden Fehler, können die Module mit folgendem Befehl installiert werden:

```bash
pip3 install -r requirements.txt
```

das muss im Unterverzeichnis "

### Auswahl der Region

Zuerst wählt man eine Region aus. Am einfachsten geht das in Google Maps. Man öffnet die Karte und klickt mit der rechten Maustaste auf die linke obere Ecke des Bereiches, man erhält dann die GPS Koordinaten im Dezimal-Format. Ein Klick auf die Koordinaten kopiert diese in die Zwischenablage.



