# K-Tool – Benutzeranleitung

## 1. K-Tool

### 1.1 Was ist K-Tool?

K-Tool ist eine Sammlung von Werkzeugen für den Kegelsport der **SFKV**.

Die einzelnen Tools unterstützen unterschiedliche Aufgaben rund um den Kegelsport. Je nach Aufgabe und Berechtigung stehen einem Benutzer unterschiedliche Funktionen zur Verfügung.

### 1.2 Die verfügbaren Tools

| Tool | Aufgabe |
|---|---|
| **Auth** | Benutzerkonto, Anmeldung und Benutzerverwaltung |
| **Starthefte** | Verwaltung von Veranstaltungen, Startheften und Startzeiten |

Weitere Tools können künftig ergänzt werden.

---

## 2. Auth

Das Tool **Auth** verwaltet die Benutzerkonten und den persönlichen Zugang zu K-Tool.

### 2.1 Anmelden

**Anmeldung:** nicht erforderlich  
**Erforderliche Rolle:** keine

Mit der Anmeldung erhält der Benutzer Zugriff auf die für ihn freigegebenen Funktionen.

Zur Anmeldung werden E-Mail-Adresse und Passwort eingegeben.

Nach erfolgreicher Anmeldung stehen abhängig von den persönlichen Berechtigungen weitere Funktionen zur Verfügung.

---

### 2.2 Abmelden

**Anmeldung:** nicht erforderlich  
**Erforderliche Rolle:** keine

Mit der Funktion **Abmelden** wird die aktuelle Sitzung beendet.

Nach dem Abmelden müssen Sie sich erneut anmelden, wenn Sie Funktionen verwenden möchten, für die eine Anmeldung erforderlich ist.

---

### 2.3 Registrieren

**Anmeldung:** nicht erforderlich  
**Erforderliche Rolle:** keine

Benutzer, die noch kein K-Tool-Konto besitzen, können eine Registrierungsanfrage stellen.

Dazu werden die erforderlichen persönlichen Angaben eingegeben.

Die Anfrage wird anschließend von der zuständigen Stelle bearbeitet.

---

### 2.4 Eigenes Profil bearbeiten

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine besondere Rolle

Angemeldete Benutzer können ihre persönlichen Angaben bearbeiten.

Dazu gehören insbesondere:

- E-Mail-Adresse
- Name
- Vorname
- MAP-Mitgliedernummer

Nach der Änderung werden die neuen Angaben gespeichert.

---

### 2.5 Passwort ändern

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine besondere Rolle

Über die Funktion **Passwort ändern** kann das persönliche Passwort geändert werden.

> **Hinweis:** Diese Funktion ist derzeit noch nicht verfügbar.

---

### 2.6 Benutzer anlegen

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Administrator**

Administratoren können neue Benutzer für K-Tool anlegen.

Bei der Anlage eines Benutzers können unter anderem folgende Angaben erfasst werden:

- E-Mail-Adresse
- Passwort
- Name
- Vorname
- MAP-Mitgliedernummer

Nach dem Anlegen kann der Benutzer mit den erforderlichen Rollen und Berechtigungen ausgestattet werden.

---

### 2.7 Benutzerrollen verwalten

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Administrator**

Administratoren können die Rollen eines Benutzers verwalten.

Dabei kann festgelegt werden, welche Aufgaben ein Benutzer innerhalb der einzelnen K-Tool-Tools übernehmen darf.

Zu den verfügbaren Rollen gehören:

- **Administrator**
- **Veranstalter**
- **Gast**

Zusätzlich können einem Benutzer Veranstaltungen zugeordnet werden.

---

# 3. Starthefte

Das Tool **Starthefte** unterstützt die Vorbereitung und Durchführung von Kegelveranstaltungen.

Der typische Ablauf einer Veranstaltung ist:

1. Veranstaltung anlegen
2. Veranstalter zuordnen
3. Programme definieren
4. Spielzeiten definieren
5. Startzeiten erzeugen
6. Startheft anzeigen
7. Startzeiten buchen
8. Startzeiten gegebenenfalls stornieren

---

## 3.1 Veranstaltung anlegen

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Administrator**

Mit dieser Funktion wird eine neue Veranstaltung angelegt.

Für eine Veranstaltung werden folgende Angaben erfasst:

- Verband
- Veranstaltungsname
- Startdatum
- Enddatum
- Kegelbahn

### Vorgehen

1. Öffnen Sie **Starthefte → Veranstaltung anlegen**.
2. Wählen Sie den zuständigen Verband.
3. Geben Sie den Namen der Veranstaltung ein.
4. Geben Sie das Startdatum ein.
5. Geben Sie das Enddatum ein.
6. Wählen Sie bei Bedarf eine Kegelbahn.
7. Speichern Sie die Veranstaltung.

Nach dem Speichern kann die Veranstaltung weiter bearbeitet werden.

---

## 3.2 Veranstalter zuordnen

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Administrator**

Mit dieser Funktion wird festgelegt, welcher Veranstalter für eine Veranstaltung zuständig ist.

### Vorgehen

1. Öffnen Sie **Starthefte → Veranstalter zuordnen**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Wählen Sie einen Veranstalter aus.
4. Speichern Sie die Zuordnung.

Bereits bestehende Zuordnungen werden angezeigt.

Eine Zuordnung kann bei Bedarf wieder entfernt werden.

> **Hinweis:** Als Veranstalter können Benutzer ausgewählt werden, die im Bereich Starthefte über die entsprechende Veranstalter-Berechtigung verfügen.

---

## 3.3 Programme bearbeiten

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Veranstalter**

Mit dieser Funktion werden die Programme einer Veranstaltung festgelegt.

Ein Programm beschreibt unter anderem:

- den Namen des Programms
- das Startintervall
- die Kegelbahn
- die verwendeten Bahnen

### Vorgehen

1. Öffnen Sie **Starthefte → Programme bearbeiten**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Prüfen Sie die bereits vorhandenen Programme.
4. Erfassen Sie bei Bedarf ein neues Programm.
5. Geben Sie den Namen des Programms ein.
6. Legen Sie das Startintervall fest.
7. Ergänzen Sie bei Bedarf Kegelbahn und Bahnen.
8. Speichern Sie das Programm.

Ein nicht mehr benötigtes Programm kann gelöscht werden.

### Startintervall

Das Startintervall bestimmt den zeitlichen Abstand zwischen den erzeugten Startzeiten.

Beispiel:

> Bei einem Startintervall von **15 Minuten** werden innerhalb einer Spielzeit Startzeiten im Abstand von 15 Minuten erzeugt.

---

## 3.4 Spielzeiten bearbeiten

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Veranstalter**

Mit dieser Funktion werden die Zeitfenster festgelegt, innerhalb derer eine Veranstaltung durchgeführt wird.

Eine Spielzeit besteht aus:

- Datum
- Startzeit
- Endzeit
- optionaler Bemerkung

### Vorgehen

1. Öffnen Sie **Starthefte → Spielzeiten bearbeiten**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Geben Sie das Datum ein.
4. Geben Sie die Startzeit ein.
5. Geben Sie die Endzeit ein.
6. Ergänzen Sie bei Bedarf eine Bemerkung.
7. Speichern Sie die Spielzeit.

Eine bestehende Spielzeit kann gelöscht werden.

### Mehrere Spieltage

Bei Veranstaltungen mit mehreren Spieltagen können die Spielzeiten nacheinander erfasst werden.

Die Anwendung unterstützt dabei die wiederholte Eingabe ähnlicher Spielzeiten.

---

## 3.5 Startzeiten erzeugen

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Veranstalter**

Mit dieser Funktion werden aus den definierten Programmen und Spielzeiten die konkreten Startzeiten erzeugt.

### Voraussetzungen

Vor dem Erzeugen der Startzeiten sollten:

- die Veranstaltung angelegt sein
- die Programme vollständig erfasst sein
- die Spielzeiten vollständig erfasst sein

### Vorgehen

1. Öffnen Sie **Starthefte → Startzeiten erzeugen**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Kontrollieren Sie die vorhandenen Programme und Spielzeiten.
4. Starten Sie die Erzeugung der Startzeiten.

Die Startzeiten werden entsprechend den definierten Programmen und Spielzeiten erzeugt.

### Beispiel

Ein Programm hat ein Startintervall von:

> **20 Minuten**

Für eine Spielzeit von:

> **09:00 bis 11:00 Uhr**

werden entsprechend Startzeiten in diesem Zeitabstand erzeugt.

---

## 3.6 Startheft anzeigen

**Anmeldung:** nicht erforderlich  
**Erforderliche Rolle:** keine

Mit dieser Funktion kann das Startheft einer Veranstaltung angezeigt werden.

Das Startheft kann auch von Personen aufgerufen werden, die nicht bei K-Tool angemeldet sind.

### Vorgehen

1. Öffnen Sie **Starthefte → Starthefte**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Das Startheft wird angezeigt.

Diese Funktion eignet sich insbesondere für die öffentliche Anzeige eines Starthefts.

---

## 3.7 Startzeiten buchen

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine besondere Rolle

Mit dieser Funktion können Startzeiten für Teilnehmer gebucht werden.

### Vorgehen

1. Öffnen Sie **Starthefte → Buchen**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Suchen Sie die gewünschte Startzeit.
4. Wählen Sie einen freien Startplatz.
5. Erfassen Sie die erforderlichen Angaben zum Teilnehmer.
6. Speichern Sie die Buchung.

Die gebuchte Startzeit wird anschließend als belegt angezeigt.

### Mehrere Buchungen

Bei mehreren Buchungen hintereinander können bereits eingegebene Angaben erneut verwendet werden. Dies erleichtert die Erfassung mehrerer Startzeiten.

---

## 3.8 Startzeiten stornieren

**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine besondere Rolle

Mit dieser Funktion kann eine bestehende Buchung wieder aufgehoben werden.

### Vorgehen

1. Öffnen Sie **Starthefte → Stornieren**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Suchen Sie die betreffende Startzeit.
4. Wählen Sie die bestehende Buchung.
5. Führen Sie die Stornierung aus.

Die Buchung wird entfernt.

Die Startzeit steht anschließend wieder für eine neue Buchung zur Verfügung.

---

# 4. Rollen und Berechtigungen

Die folgenden Rollen werden in K-Tool verwendet:

| Rolle | Bedeutung |
|---|---|
| **Administrator** | Verwaltet Benutzer und übernimmt übergeordnete Aufgaben innerhalb der Tools. |
| **Veranstalter** | Verwaltet Veranstaltungen und deren Vorbereitung im Rahmen der vorgesehenen Aufgaben. |
| **Gast** | Verfügt über eingeschränkte Berechtigungen. |

Nicht jede Funktion benötigt eine bestimmte Rolle.

Einige Funktionen:

- sind öffentlich zugänglich,
- benötigen lediglich eine Anmeldung,
- oder setzen eine bestimmte Rolle voraus.

---

# 5. Berechtigungsübersicht

| Funktion | Anmeldung | Erforderliche Rolle |
|---|---|---|
| Anmelden | Nein | Keine |
| Abmelden | Nein | Keine |
| Registrieren | Nein | Keine |
| Eigenes Profil bearbeiten | Ja | Keine besondere Rolle |
| Passwort ändern | Ja | Keine besondere Rolle* |
| Benutzer anlegen | Ja | **Administrator** |
| Benutzerrollen verwalten | Ja | **Administrator** |
| Veranstaltung anlegen | Ja | **Administrator** |
| Veranstalter zuordnen | Ja | **Administrator** |
| Programme bearbeiten | Ja | **Veranstalter** |
| Spielzeiten bearbeiten | Ja | **Veranstalter** |
| Startzeiten erzeugen | Ja | **Veranstalter** |
| Startheft anzeigen | Nein | Keine |
| Startzeiten buchen | Ja | Keine besondere Rolle |
| Startzeiten stornieren | Ja | Keine besondere Rolle |

\* Die Funktion „Passwort ändern“ ist vorgesehen, aber derzeit noch nicht verfügbar.

---

# 6. Typischer Ablauf einer Veranstaltung

Die Vorbereitung einer Veranstaltung erfolgt normalerweise in dieser Reihenfolge:

### 1. Veranstaltung anlegen

**Administrator**

Die grundlegenden Daten der Veranstaltung werden erfasst.

↓

### 2. Veranstalter zuordnen

**Administrator**

Der zuständige Veranstalter wird der Veranstaltung zugeordnet.

↓

### 3. Programme bearbeiten

**Veranstalter**

Die Programme und Startintervalle werden festgelegt.

↓

### 4. Spielzeiten bearbeiten

**Veranstalter**

Die Spieltage sowie Beginn und Ende der Spielzeiten werden festgelegt.

↓

### 5. Startzeiten erzeugen

**Veranstalter**

Aus Programmen und Spielzeiten werden die konkreten Startzeiten erzeugt.

↓

### 6. Startheft anzeigen

**Alle**

Das fertige Startheft kann angezeigt werden.

↓

### 7. Startzeiten buchen

**Angemeldete Benutzer**

Freie Startzeiten können gebucht werden.

↓

### 8. Startzeiten stornieren

**Angemeldete Benutzer**

Bestehende Buchungen können bei Bedarf wieder aufgehoben werden.

---

# 7. Kurzüberblick für Benutzer

## Administrator

Ein Administrator kann insbesondere:

- Benutzer anlegen
- Benutzerrollen verwalten
- Veranstaltungen anlegen
- Veranstalter Veranstaltungen zuordnen

## Veranstalter

Ein Veranstalter kann insbesondere:

- Programme bearbeiten
- Spielzeiten bearbeiten
- Startzeiten erzeugen

## Angemeldete Benutzer

Angemeldete Benutzer können:

- ihr eigenes Profil bearbeiten
- Startzeiten buchen
- Startzeiten stornieren

## Öffentliche Benutzer

Auch ohne Anmeldung kann:

- das Startheft angezeigt werden.

---

# 8. Hinweise zur Arbeit mit Startheften

Für eine reibungslose Vorbereitung empfiehlt sich folgende Reihenfolge:

1. Veranstaltung vollständig anlegen
2. Veranstalter zuordnen
3. Programme definieren
4. Spielzeiten definieren
5. Angaben kontrollieren
6. Startzeiten erzeugen
7. Startheft kontrollieren
8. Startzeiten zur Buchung freigeben

Je sorgfältiger die Veranstaltung vor der Erzeugung der Startzeiten eingerichtet wird, desto weniger nachträgliche Korrekturen sind erforderlich.
