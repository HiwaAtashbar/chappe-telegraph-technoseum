# Optischer Telegraf nach Claude Chappe (1794) – Interaktive Simulation

Eine Web-Simulation des optischen Flügeltelegrafen von Claude Chappe, entstanden als Vibe-Coding-Projekt nach einem Besuch im TECHNOSEUM Mannheim.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**Live-Demo / Live demo:** [Insert GitHub Pages Link]

---

## Deutsch

### Worum es geht

Die Anwendung zeigt, wie der optische Telegraf von Claude Chappe (1794) funktionierte: Man bewegt die Hebel, sieht die Flügel auf dem Mast reagieren und kann eigene Nachrichten senden. Sie besteht aus einer einzigen HTML-Datei ohne externe Abhängigkeiten und läuft in jedem aktuellen Browser.

Das TECHNOSEUM Mannheim war der Anlass für das Projekt. Die Simulation ist keine Abbildung eines Exponats, sondern eine eigene Umsetzung auf Grundlage der unten genannten Quellen. Sie wurde mit KI-Unterstützung erstellt und vor der Präsentation vom Autor auf ihre Funktion geprüft. Sie ist ein Lern- und Demonstrationswerkzeug und kein exaktes historisches Modell.

### Funktionsweise des Chappe-Systems

Chappe entwickelte seinen Flügeltelegrafen ab 1790. 1794 ging die erste reguläre Linie zwischen Paris und Lille in Betrieb, mit einer Länge von etwa 240 km (je nach Quelle werden 225 bis 270 km genannt). Ein Signal brauchte von Paris nach Lille nur wenige Minuten.

**Mechanischer Aufbau (wie in der Simulation umgesetzt)**

- Regulator: Mittelbalken, 4,60 m, mit Lamellen gegen die Windlast. Vier Hauptstellungen im 45°-Raster (0°, 45°, 90°, 135°).
- Indikatoren: zwei Signalflügel mit je 2,00 m, an den Enden des Regulators drehbar gelagert. Jeder Flügel lässt sich in 45°-Schritten einstellen.
- Gegengewichte: Eisenstangen mit Kugeln gleichen das Gewicht der Holzflügel aus. Aus großer Entfernung sind sie kaum zu erkennen.
- Manipulator: Ein verkleinertes Hebelwerk in der Kabine, das über Seilzüge und Umlenkrollen im Verhältnis 1:1 mit dem Mast gekoppelt ist.

**Das Zwei-Phasen-Protokoll**

1. Einstellphase: Das Zeichen wird eingestellt, solange der Regulator schräg steht (45° oder 135°). Die Nachbarstation sieht, dass die Flügel noch in Bewegung sind, und liest noch nicht ab.
2. Verriegelung: Erst wenn der Regulator waagerecht (0°) oder senkrecht (90°) steht, gilt das Zeichen als gültig und wird durch das Fernrohr abgelesen.

Mit zwei Lesepositionen des Regulators und je sieben Stellungen der beiden Indikatoren ergeben sich 2 × 7 × 7 = 98 Lesesignale. Zusammen mit Léon Delaunay entwickelte Chappe außerdem ein Codebuch für ganze Wörter, Orte und Redewendungen, das die Übertragung beschleunigte und vor dem Mitlesen schützte.

### Funktionen der Simulation

- Drei Ansichten in einem Fenster: Mast mit Seilzügen und Bewegungsbereich, Fernrohr-Ansicht der Nachbarstation (12 km Distanz) und Hebelwerk der Bedienkabine.
- Telegrammsender für Nachrichten beliebiger Länge im Zwei-Takt-Verfahren (schräg einstellen, dann verriegeln und protokollieren), mit automatischer Umlaut-Umwandlung (Ä zu AE, Ö zu OE, Ü zu UE, ß zu SS).
- Anpassung an unterschiedliche Bildschirmgrößen, vom Smartphone bis zum 4K-Monitor.

### Historischer Kontext in Deutschland

Das französische Netz reichte in napoleonischer Zeit bis an den Rhein. Preußen baute zwischen 1832 und 1852 eine eigene optische Telegrafenlinie von Berlin nach Koblenz. Sie ist ein anderes System als das von Chappe, beruht aber auf demselben Grundgedanken: Nachrichten werden über sichtbare Signale von Station zu Station weitergegeben.

| Merkmal | Preußische Linie Berlin – Koblenz |
|---|---|
| Länge und Stationen | ca. 587 km, 62 Stationen |
| Stationsabstand | ca. 9 bis 14 km |
| Betrieb | ca. 6 Stunden täglich bei klarer Sicht |
| Geheimhaltung | Nur wenige Codebücher; entschlüsselt wurde nur in ausgewählten Stationen, die Zwischenstationen gaben die Stellungen weiter |
| Erhaltene Stationen (Auswahl) | Potsdam (Station 4), Neuwegersleben (18), Oeynhausen (32), Iserlohn (43), Köln-Flittard (50), Straßenhaus (57) |

Ein Beispiel zum Ansehen ist die erhaltene Station in Köln-Flittard.

---

## English

### What this is

An interactive simulation of Claude Chappe's 1794 optical telegraph. You move the levers, watch the arms on the mast respond, and send your own messages. It is a single HTML file with no external dependencies and runs in any current browser.

The project started with a visit to the TECHNOSEUM Mannheim. The simulation does not reproduce an exhibit; it is an independent implementation based on the sources listed below. It was built with AI assistance, and the author checked its behaviour before presenting it. It is meant for learning and demonstration, not as an exact historical model.

### Features

- Three views in one window: the mast with cables and range of motion, a telescope view of the neighbouring station (12 km away), and the lever mechanism in the operator's cabin.
- The two-phase protocol: arms are set while the main beam is oblique (45° or 135°), then locked horizontal (0°) or vertical (90°) so the next station can read the signal.
- A message sender for texts of any length, with a scrolling paper-tape log and automatic umlaut conversion.
- Responsive layout for screens from phones to 4K monitors.

### Running it

Open `index.html` in a browser, or use the live demo linked above. No installation or build step is needed.

---

## Quellen / Sources

1. [Chappes optischer Flügel-Telegraf – kryptografie.de](https://kryptografie.de/kryptografie/chiffre/chappe.htm): Kodierung, Funktionsweise, Übertragungsgeschwindigkeit und Codebücher.
2. [Optische Telegraphie in Preußen – optischertelegraph4.de](https://www.optischertelegraph4.de/): Geschichte und Stationen der Linie Berlin – Koblenz.
3. [Flittard – Wikipedia](https://de.wikipedia.org/wiki/Flittard): Hinweise zur erhaltenen Station in Köln-Flittard.

## Lizenz / License

MIT-Lizenz, siehe [LICENSE](LICENSE).
