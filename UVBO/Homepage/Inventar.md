# Inventar der FKVBO-Website

## 1. Zweck des Inventars

Dieses Dokument inventarisiert die bestehende Website des **Keglerverbandes Oberland (FKVBO)**. Es dient als Grundlage für die spätere Entscheidung, ob die bestehende Website modernisiert, technisch aktualisiert oder vollständig neu aufgebaut werden soll.

Die Inventarisierung betrachtet nicht nur die sichtbare Navigation, sondern unterscheidet zwischen redaktionellen Inhalten, strukturierten Sportdaten, Dokumenten und möglichen Anwendungen.

**Analysierte Website:** https://www.keglerverband-oberland.ch/fkvboweb/index.php?cat=FKVBO%20Start

**Festgestellte technische Basis:** moziloCMS 2.0; im Footer wird die Website als „FKVBO WEB 1.5“ ausgewiesen.

---

## 2. Hauptnavigation

Die bestehende Website weist folgende Hauptbereiche auf:

| Bereich | Inhalt / Funktion | Typ | Bedeutung für Neubau |
|---|---|---|---|
| FKVBO Start | Einstieg, aktuelle Informationen, wichtige Hinweise und Verweise | Redaktionell | hoch |
| ZV | Informationen zum Zentralvorstand | Verband / redaktionell | mittel-hoch |
| UVMW | Bereich des Unterverbandes bzw. dessen Organisation und Sportbetrieb | Verband / Sport | hoch |
| Startheft 2026 | Startheft und damit verbundene Informationen | Anwendung / Sportdaten | sehr hoch |
| Sportliches | Meisterschaften, Programme, Resultate, Ranglisten usw. | Strukturierte Sportdaten | sehr hoch |
| Verband | Allgemeine Verbandsinformationen | Redaktionell | mittel |
| Kegelbahnen | Übersicht der verwendeten Kegelbahnen und Links | Strukturierte Stammdaten | hoch |
| Fotos und Events | Bilder und Veranstaltungen | Medien / redaktionell | mittel |
| Wichtige Links | Externe Links zu relevanten Angeboten | Links | mittel |
| Archiv | Ältere Informationen und Dokumente | Archiv | hoch |
| Zum Gedenken | Informationen über verstorbene Kegler/Funktionäre | Historische Daten | mittel |
| Login | Zugang zu geschützten bzw. administrativen Funktionen | Anwendung | sehr hoch / offen |

---

## 3. FKVBO Start

### Inhalt

Die Startseite dient als zentrale Einstiegs- und Informationsseite. Erkennbar sind unter anderem:

- aktuelle Informationen
- Jahresprogramm 2026
- Resultate Einzel-Cup 2026
- Hinweise zu Bürodiensten, Bahnaufsicht und Service
- Startheft Oberland
- Ranglisten
- Inserate bzw. Hinweise auf externe Meisterschaften
- Verweise auf Berner-Trophy
- Verweis auf Meisterschaftsplaner / Keglerfreund

### Einordnung

**Typ:** redaktioneller Inhalt mit Links und Dokumenten.

### Möglicher Neubau

Ein eigener Bereich „Aktuelles“ bzw. „News“ wäre sinnvoll. Meldungen könnten strukturiert verwaltet werden:

- Titel
- Datum
- Text
- optional Bild
- optional Dokument
- optional externer Link
- Status / Veröffentlichung

Die Startseite könnte daraus automatisch die aktuellen Meldungen und ausgewählte wichtige Informationen anzeigen.

---

## 4. ZV

### Inhalt

Der Bereich dient den Informationen zum Zentralvorstand bzw. zur Verbandsführung.

### Noch zu klären

- vollständige Unterseiten
- Funktionen und Personen
- Kontaktdaten
- Ressorts
- Sitzungen / Versammlungen
- Dokumente
- historische Informationen

### Einordnung

**Typ:** überwiegend redaktionell, teilweise strukturierbare Personendaten.

### Möglicher Neubau

Personen und Funktionen könnten als strukturierte Daten geführt werden:

```text
Person
├── Vorname
├── Name
├── Funktion / Ressort
├── Kontakt
└── Gültigkeit
```

Damit könnten Vorstand und Kontaktinformationen automatisch dargestellt werden.

---

## 5. UVMW

### Inhalt

Der Bereich UVMW gehört zur organisatorischen bzw. sportlichen Struktur des FKVBO.

### Noch zu klären

- genaue Bedeutung und Abgrenzung des Bereichs
- eigene Organisation / Funktionäre
- eigene Meisterschaften
- eigene Resultate
- eigene Dokumente
- eigene Termine

### Einordnung

**Typ:** Verband / Sportbetrieb.

### Neubau-Relevanz

Falls hier sportliche Daten gepflegt werden, sollte geprüft werden, ob diese als gemeinsame Datenbasis mit den übrigen Meisterschafts- und Veranstaltungsdaten geführt werden können.

---

## 6. Startheft 2026

### Bedeutung

Der Bereich „Startheft 2026“ ist einer der wichtigsten Punkte der Inventarisierung. Das Startheft ist nicht lediglich ein statischer Informationsbereich, sondern kann eine Anwendung bzw. eine Darstellung dynamischer Sportdaten darstellen.

### Zu klären

- Herkunft der Startzeiten
- Erfassung und Pflege der Startzeiten
- Anmeldung / Reservation
- Stornierung
- Benutzerrollen
- Login-Abhängigkeit
- verantwortliche Personen
- verwendete Datenquellen
- Zusammenhang mit externen Systemen
- Zusammenhang mit K-Tool

### Einordnung

**Typ:** Anwendung / strukturierte Sportdaten.

### Neubau-Relevanz

Sehr hoch. Vor einem Neubau muss geklärt werden, ob das Startheft künftig weiterhin Bestandteil der FKVBO-Website sein soll oder ob die Funktionalität durch K-Tool bereitgestellt bzw. von dort eingebunden werden kann.

---

## 7. Sportliches

### Inhalt

Der Bereich „Sportliches“ enthält die wesentlichen Informationen zum Sportbetrieb. Dazu gehören insbesondere:

- Jahresmeisterschaften
- Jahresprogramm
- Meisterschaften
- Einzel-Cup
- Resultate
- Ranglisten
- weitere sportliche Veranstaltungen

Das Jahresprogramm enthält strukturierte Angaben wie Datum, Veranstaltung, Kegelbahn, Klub und weitere Angaben zum Sportbetrieb.

### Einordnung

**Typ:** strukturierte Sportdaten plus Dokumente.

### Neubau-Relevanz

Sehr hoch.

Statt Informationen nur in Seiten und PDF-Dateien abzulegen, könnte ein Neubau Veranstaltungen als Datenobjekte führen:

```text
Veranstaltung
├── Bezeichnung
├── Datum von / bis
├── Veranstaltungsart
├── Kegelbahn
├── durchführender Klub
├── Programm
├── Ausschreibung
├── Startzeiten
├── Rangliste
└── Resultate
```

Damit könnten Jahresprogramm, Veranstaltungsübersichten und Archivansichten automatisch aus derselben Datenbasis erzeugt werden.

---

## 8. Verband

### Inhalt

Allgemeine Informationen zum Verband.

### Mögliche Inhalte

- Geschichte
- Organisation
- Reglemente
- Kontakte
- Funktionäre
- Klubs
- Versammlungen
- Dokumente

### Einordnung

**Typ:** überwiegend statischer bzw. selten ändernder redaktioneller Inhalt.

### Neubau-Relevanz

Mittel. Ein klassischer CMS-Bereich reicht grundsätzlich aus.

---

## 9. Kegelbahnen

### Bestehender Inhalt

Die Website führt eine Übersicht von Kegelbahnen bzw. Kegellokalen, unter anderem:

- Kegelsportzentrum Rössli Heimberg
- Gasthof zum Bären Süderen
- Restaurant Bellevue / Rossgagupintli Steffisburg
- Park Goldswil
- Restaurant Glockental Steffisburg
- Alpenrose Innertkirchen

Die Einträge verweisen auf externe Websites.

### Einordnung

**Typ:** Stammdaten / externe Links.

### Möglicher Neubau

Kegelbahnen sollten als eigene Datenobjekte geführt werden:

```text
Kegelbahn
├── Name
├── Adresse
├── Ort
├── Anzahl Bahnen
├── Kontakt
├── Website
└── weitere Informationen
```

Veranstaltungen könnten direkt auf eine Kegelbahn verweisen. Damit würden dieselben Bahndaten nicht mehrfach erfasst.

---

## 10. Fotos und Events

### Inhalt

Bereich für Bilder und Veranstaltungen.

### Noch zu klären

- Anzahl und Umfang der Fotoalben
- historische Bilder
- Zuordnung von Bildern zu Veranstaltungen
- wer Bilder hochlädt und pflegt
- Speicherort und Dateiorganisation

### Einordnung

**Typ:** Medien / redaktioneller Inhalt.

### Möglicher Neubau

Veranstaltungen könnten mit Fotoalben verbunden werden:

```text
Event
├── Titel
├── Datum
├── Beschreibung
└── Fotoalbum
    ├── Bild 1
    ├── Bild 2
    └── ...
```

---

## 11. Wichtige Links

### Inhalt

Sammlung externer Links, unter anderem zu Angeboten rund um den Kegelsport.

### Einordnung

**Typ:** externe Links.

### Möglicher Neubau

Einfache strukturierte Linkverwaltung:

```text
Link
├── Bezeichnung
├── Beschreibung
├── URL
└── Kategorie
```

---

## 12. Archiv

### Bedeutung

Das Archiv enthält ältere Informationen und Dokumente. Bei einem Neubau sollte dieser Bereich nicht einfach als Sammlung einzelner alter Seiten übernommen werden.

### Zu klären

- vorhandene Jahre
- Jahresprogramme
- Resultate
- Ranglisten
- Veranstaltungen
- Versammlungsunterlagen
- Fotos
- historische Informationen

### Möglicher Neubau

Das Archiv sollte möglichst über Jahr und Inhaltstyp erschliessbar sein:

```text
Archiv
├── 2026
├── 2025
├── 2024
└── ...
```

Dabei sollten strukturierte Daten und Dokumente möglichst gemeinsam auffindbar sein.

---

## 13. Zum Gedenken

### Inhalt

Bereich für das Andenken an verstorbene Kegler und Funktionäre.

### Einordnung

**Typ:** historischer / redaktioneller Inhalt.

### Möglicher Neubau

Falls die Daten entsprechend gepflegt werden, könnte ein Gedenkeintrag strukturiert werden:

```text
Person
├── Name
├── Geburtsjahr
├── Todesjahr
├── Foto
├── Klub / Funktion
└── Gedenktext
```

Der Bereich hat eine besondere historische Bedeutung und sollte bei einem Neubau bewusst erhalten werden.

---

## 14. Login

### Bedeutung

Der öffentliche Menüpunkt „Login“ ist für die Beurteilung der technischen Komplexität besonders wichtig.

### Noch zu klären

- Welche Benutzer können sich anmelden?
- Welche Funktionen stehen angemeldeten Benutzern zur Verfügung?
- Gibt es einen geschützten Dokumentenbereich?
- Gibt es administrative Funktionen?
- Wird das Startheft darüber verwaltet?
- Gibt es Resultaterfassung?
- Gibt es Benutzerrollen?
- Welche Daten werden im Login-System gespeichert?

### Einordnung

**Typ:** Anwendung.

### Neubau-Relevanz

Sehr hoch. Erst nach Analyse des Login-Bereichs kann der tatsächliche Funktionsumfang der heutigen Website abschliessend beurteilt werden.

---

## 15. Dokumente

Dokumente spielen auf der Website eine wichtige Rolle. Insbesondere im sportlichen Bereich werden Informationen teilweise als PDF bereitgestellt.

### Typische Dokumente

- Jahresprogramme
- Ausschreibungen
- Ranglisten
- Resultate
- Verbandsunterlagen
- weitere sportliche Dokumente

### Grundsätzliche Frage für den Neubau

Es ist zu entscheiden, welche Informationen weiterhin als PDF veröffentlicht werden sollen und welche künftig direkt aus strukturierten Daten auf der Website dargestellt werden können.

Ein PDF kann weiterhin als offizielles Dokument sinnvoll sein. Die Website sollte jedoch nicht gezwungen sein, Informationen ausschliesslich über PDF-Dateien zugänglich zu machen.

---

## 16. Vorläufige technische Inventarisierung

### Bestehende technische Basis

- moziloCMS 2.0
- Websitebezeichnung im Footer: „FKVBO WEB 1.5“
- PHP-basierte Webanwendung
- überwiegend dateibasierte / CMS-basierte Inhalte
- Dokumente und Bilder als ergänzende Dateien
- Login bzw. geschützte Funktionen vorhanden

### Architektur, soweit öffentlich erkennbar

```text
Browser
   │
   ▼
Webserver / PHP
   │
   ▼
moziloCMS 2.0
   │
   ├── CMS-Seiten
   ├── Dokumente
   ├── Bilder
   ├── externe Links
   └── Login / weitere Funktionen
```

Die genaue technische Umsetzung des Login- und Startheftbereichs muss separat untersucht werden.

---

## 17. Klassifizierung für einen möglichen Neubau

Für die weitere Analyse werden die Inhalte in vier Klassen eingeteilt:

| Klasse | Beschreibung | Beispiele | Geeignete technische Lösung |
|---|---|---|---|
| A | Statische Informationen | Verband, Geschichte, Kontakte | CMS / redaktionelle Seiten |
| B | Redaktionelle Inhalte | News, Events, Fotos, Hinweise | CMS mit Medienverwaltung |
| C | Strukturierte Daten | Veranstaltungen, Termine, Bahnen, Resultate, Ranglisten | Datenbank / Fachanwendung |
| D | Interaktive Anwendungen | Startheft, Login, Reservationen, Administration | Webanwendung |

---

## 18. Besonders untersuchungswürdige Bereiche

Für die nächste Analyse haben folgende Bereiche Priorität:

1. **Login** – tatsächlichen Funktionsumfang ermitteln
2. **Startheft 2026** – Datenquelle und Funktionen ermitteln
3. **Sportliches** – vorhandene Sportdaten und deren Pflege untersuchen
4. **UVMW** – Struktur und eigene Funktionen klären
5. **Archiv** – Umfang und historische Daten erfassen
6. **Fotos und Events** – Umfang der Medienbestände erfassen
7. **ZV / Verband** – Verantwortlichkeiten und redaktionelle Pflege klären

---

## 19. Ziel der weiteren Inventarisierung

Die nächste Stufe soll nicht nur die sichtbaren Menüpunkte erfassen, sondern für jede einzelne Seite bzw. Funktion folgende Angaben dokumentieren:

| Merkmal | Bedeutung |
|---|---|
| URL | aktuelle Adresse |
| Titel | Bezeichnung der Seite |
| Navigation | Position in der Website-Struktur |
| Inhalt | fachlicher Inhalt |
| Inhaltstyp | Text, Dokument, Bild, Daten, Anwendung |
| Datenquelle | Woher stammen die Informationen? |
| Pflege | Wer pflegt den Inhalt? |
| Änderungsfrequenz | Wie häufig wird er verändert? |
| Benutzerrolle | Wer darf ihn sehen bzw. bearbeiten? |
| Abhängigkeiten | Andere Seiten/Systeme/Daten |
| Neubau-Kategorie | A, B, C oder D |
| Übernahme | unverändert / überarbeiten / neu modellieren / ersetzen |
| K-Tool-Bezug | mögliche Integration oder Ablösung durch K-Tool |

---

## 20. Vorläufiges Fazit

Die bestehende FKVBO-Website ist nicht nur eine statische Vereins-Homepage. Sie verbindet:

- redaktionelle Verbandsinformationen,
- aktuelle Meldungen,
- Dokumentenverwaltung,
- Sportprogramme,
- Meisterschaftsinformationen,
- Resultate und Ranglisten,
- Kegelbahn-Stammdaten,
- Fotos und Events,
- ein historisches Archiv,
- einen Gedenkbereich,
- ein Startheft und
- einen Login-Bereich.

Damit besteht eine sinnvolle Grundlage für die Untersuchung eines Neuaufbaus.

**Die zentrale Frage für den Neubau ist nicht, wie die heutige Website technisch nachgebaut werden kann, sondern welche heutigen Inhalte künftig als redaktioneller Inhalt, als strukturierte Daten oder als eigenständige Anwendung behandelt werden sollen.**

Insbesondere ist zu prüfen, ob das Startheft und weitere sportliche Funktionen mit K-Tool verbunden oder teilweise durch K-Tool übernommen werden können. Dadurch könnte die neue FKVBO-Website wesentlich einfacher bleiben als ein vollständiger Ersatz aller heute vorhandenen Funktionen.
