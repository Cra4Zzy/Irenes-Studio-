# Elektro Freitag – Website-Entwurf

Individueller statischer Website-Auftritt in Rot (#d5312b), Anthrazit und warmem Weiß. Original-Logo, großzügige Typografie, asymmetrische Bildflächen und klare Leistungslisten statt einer austauschbaren Kartenoberfläche.

## Vorschau

`python -m http.server 8000 --directory .`

Die Startseite ist `index.html`. Alle Pfade sind relativ; die fertigen Dateien können auch im Hauptverzeichnis eines GitHub-Pages-Repositories bereitgestellt werden. Kein Build-Service und kein Framework erforderlich.

## Bearbeiten

Inhalte und Seitentemplates: `build.py`. Neu erzeugen: `python build.py`.
Styles: `assets/style.css`. Interaktionen: `assets/main.js`.
Die Asset-Dateien bleiben beim Neugenerieren erhalten.

## Seiten

Startseite, Leistungsübersicht, Elektroinstallation, Photovoltaik, KNX/Gebäudesteuerung, Hausgeräte, Netzwerk/Kommunikation, Service/Reparatur, Über uns, Verkaufsbereich, Stellenangebote/Ausbildung, Kontakt, Impressum, Datenschutz, 404.
Die bisherigen Routen `kontakt.html`, `stellenangebote.html`, `footer/impressum.html` und `footer/datenschutz.html` bleiben erhalten. Die frühere Über-uns-Navigation führte auf die Startseite; sie erhält jetzt eine eigene Seite.

## Funktionen

Responsive Navigation mit Tastatur- und Escape-Bedienung, aufklappbare Stellenangebote, dezente Einblendeeffekte mit Rücksicht auf reduzierte Bewegung, Telefon- und E-Mail-Verknüpfungen, externe Anfahrt erst nach Klick.
Das Kontaktformular erstellt einen E-Mail-Link. Es sendet und speichert keine Nachrichten auf einem Server. Vor dem tatsächlichen Versand öffnet der Besucher sein E-Mail-Programm.
Kein Tracking, keine eingebetteten Karten, keine extern geladenen Schriften. Die Präsentationsversion bleibt `noindex,nofollow`.

## Quellen und Freigabe

Unternehmensinformationen und bisherige Seiten: https://www.elektro-freitag.net/ (Abruf 08.10.2026).
Seit 1947, Archshofen 5, Kontaktdaten und 70-m²-Verkaufsbereich sind dem bestehenden Auftritt entnommen. Die Karriereangaben orientieren sich an dessen Stellenangeboten. Der dort genannte Ausbildungsstart September 2026 liegt bereits in der Vergangenheit und wird als historische Angabe mit Rückfrage zum nächsten Start behandelt.

Original-Logo und drei Verkaufsbereichsfotos wurden von der vorhandenen Website lokal übernommen. Die Eigentums-/Nutzungsfreigabe erfolgt mit dem Unternehmen vor offizieller Veröffentlichung.
Die beiden ergänzenden Bilder sind illustrative generierte Motive, keine behaupteten Mitarbeiter-, Projekt- oder Referenzaufnahmen. Hinweise hierzu stehen im Datenschutz des Entwurfs.

Impressum und Datenschutz sind ein gekennzeichneter Präsentationsstand. Vor dem offiziellen Livegang Unternehmensdaten, Stellenverfügbarkeit, Bilderfreigabe, Hosting, Kontaktzustellung und rechtliche Texte mit dem Betreiber abstimmen.

## Bildbriefings

Integrierter Bildgenerator, photorealistic-natural:
1. `assets/hero.webp`: glaubwürdiges fränkisches Wohnhaus mit Satteldach und Photovoltaik zur blauen Stunde, warme integrierte Beleuchtung, natürliche Architekturaufnahme, ohne Personen oder Marken.
2. `assets/detail.webp`: anthrazitfarbenes KNX-Bedienelement auf warmer mineralischer Wand neben einer Eichenholztür, dezente Innenraumfotografie, ohne Texte oder Marken.

## Prüfung

JavaScript-Syntax, HTML-Struktur, Seitenverweise und lokale Assets werden geprüft. Eine visuelle Browserprüfung steht aus, da das zulässige Browser-QA-Werkzeug in dieser Umgebung nicht verfügbar ist.
