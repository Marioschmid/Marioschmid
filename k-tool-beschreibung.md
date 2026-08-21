# K-Tool – Benutzeranleitung

## 1. K-Tool

### 1.1 Was ist K-Tool?

K-Tool ist eine Sammlung von Werkzeugen für den **Kegelsport der SFKV**.

Die einzelnen Tools unterstützen unterschiedliche Aufgaben rund um den Kegelsport. Je nach Aufgabe und Berechtigung stehen einem Benutzer unterschiedliche Funktionen zur Verfügung.

### 1.2 Die verfügbaren Tools

| Tool | Aufgabe |
|---|---|
| **Auth** | Benutzerkonto, Anmeldung und Benutzerverwaltung |
| **Starthefte** | Verwaltung von Veranstaltungen, Startheften und Startzeiten |

Weitere Tools können künftig ergänzt werden.

---

# 2. Auth

Das Tool **Auth** verwaltet die Benutzerkonten und den persönlichen Zugang zu K-Tool.

## 2.1 Anmeldung

**Tool:** Auth  
**Menü:** Login  
**Anmeldung:** nicht erforderlich  
**Erforderliche Rolle:** keine

Mit der Anmeldung erhalten Sie Zugriff auf die für Sie freigegebenen Funktionen.

Geben Sie dazu Ihre E-Mail-Adresse und Ihr Passwort ein.

Nach erfolgreicher Anmeldung stehen abhängig von Ihren Berechtigungen weitere Funktionen zur Verfügung.

---

## 2.2 Registrierung

**Tool:** Auth  
**Menü:** Registrieren  
**Anmeldung:** nicht erforderlich  
**Erforderliche Rolle:** keine

Wenn Sie noch kein Benutzerkonto besitzen, können Sie sich bei K-Tool registrieren.

Geben Sie die erforderlichen persönlichen Angaben ein und senden Sie die Registrierungsanfrage ab.

---

## 2.3 Abmelden

**Tool:** Auth  
**Menü:** Abmelden  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine

Mit **Abmelden** beenden Sie Ihre aktuelle Sitzung.

Wenn Sie anschließend wieder auf Funktionen zugreifen möchten, für die eine Anmeldung erforderlich ist, müssen Sie sich erneut anmelden.

---

## 2.4 Profil bearbeiten

**Tool:** Auth  
**Menü:** Profil  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine besondere Rolle

Sie können Ihre persönlichen Angaben bearbeiten.

Dazu gehören insbesondere:

- E-Mail-Adresse
- Name
- Vorname
- MAP-Mitgliedernummer

Nach der Änderung werden die neuen Angaben gespeichert.

---

## 2.5 Passwort ändern

**Tool:** Auth  
**Menü:** Passwort ändern  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine besondere Rolle

Mit dieser Funktion können Sie Ihr persönliches Passwort ändern.

> **Hinweis:** Die Funktion ist derzeit noch nicht verfügbar.

---

## 2.6 Benutzer anlegen

**Tool:** Auth  
**Menü:** Benutzer → Benutzer anlegen  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Administrator**

Administratoren können neue Benutzer für K-Tool anlegen.

Bei der Anlage eines Benutzers werden unter anderem folgende Angaben erfasst:

- E-Mail-Adresse
- Passwort
- Name
- Vorname
- MAP-Mitgliedernummer

Nach dem Anlegen können dem Benutzer die erforderlichen Berechtigungen zugewiesen werden.

---

## 2.7 Benutzerrollen verwalten

**Tool:** Auth  
**Menü:** Benutzer → Benutzer Rollen  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Administrator**

Administratoren können die Rollen eines Benutzers verwalten.

Dabei wird festgelegt, welche Aufgaben ein Benutzer innerhalb der einzelnen K-Tool-Tools übernehmen darf.

Zur Verfügung stehen insbesondere die Rollen:

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

## 3.1 Home

**Tool:** Starthefte  
**Menü:** Home  
**Anmeldung:** nicht erforderlich  
**Erforderliche Rolle:** keine

Die Startseite des Tools **Starthefte** bietet den Einstieg in die Funktionen des Tools.

Von hier aus können Sie die verfügbaren Funktionen aufrufen.

---

# 4. Veranstaltung

Die Menügruppe **Veranstaltung** enthält alle Funktionen, die für die Vorbereitung einer Veranstaltung benötigt werden.

---

## 4.1 Veranstaltung anlegen

**Tool:** Starthefte  
**Menü:** Veranstaltung → Veranstaltung anlegen  
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

1. Öffnen Sie **Veranstaltung → Veranstaltung anlegen**.
2. Wählen Sie den zuständigen Verband.
3. Geben Sie den Namen der Veranstaltung ein.
4. Geben Sie das Startdatum ein.
5. Geben Sie das Enddatum ein.
6. Wählen Sie die Kegelbahn.
7. Speichern Sie die Veranstaltung.

Nach dem Speichern kann die Veranstaltung weiter bearbeitet werden.

---

## 4.2 Veranstalter zuordnen

**Tool:** Starthefte  
**Menü:** Veranstaltung → Veranstalter zuordnen  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Administrator**

Mit dieser Funktion wird festgelegt, welcher Veranstalter für eine Veranstaltung zuständig ist.

### Vorgehen

1. Öffnen Sie **Veranstaltung → Veranstalter zuordnen**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Wählen Sie einen Veranstalter aus.
4. Speichern Sie die Zuordnung.

Bereits bestehende Zuordnungen werden angezeigt.

Eine Zuordnung kann bei Bedarf wieder entfernt werden.

> **Hinweis:** Als Veranstalter können Benutzer ausgewählt werden, die über die entsprechende Veranstalter-Berechtigung für das Tool Starthefte verfügen.

---

## 4.3 Programme bearbeiten

**Tool:** Starthefte  
**Menü:** Veranstaltung → Programme bearbeiten  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Veranstalter**

Mit dieser Funktion werden die Programme einer Veranstaltung festgelegt.

Ein Programm beschreibt unter anderem:

- den Namen des Programms
- das Startintervall
- die Kegelbahn
- die verwendeten Bahnen

### Vorgehen

1. Öffnen Sie **Veranstaltung → Programme bearbeiten**.
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

## 4.4 Spielzeiten bearbeiten

**Tool:** Starthefte  
**Menü:** Veranstaltung → Spielzeiten bearbeiten  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Veranstalter**

Mit dieser Funktion werden die Zeitfenster festgelegt, innerhalb derer eine Veranstaltung durchgeführt wird.

Eine Spielzeit besteht aus:

- Datum
- Startzeit
- Endzeit
- optionaler Bemerkung

### Vorgehen

1. Öffnen Sie **Veranstaltung → Spielzeiten bearbeiten**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Geben Sie das Datum ein.
4. Geben Sie die Startzeit ein.
5. Geben Sie die Endzeit ein.
6. Ergänzen Sie bei Bedarf eine Bemerkung.
7. Speichern Sie die Spielzeit.

Eine bestehende Spielzeit kann gelöscht werden.

### Mehrere Spieltage

Bei Veranstaltungen mit mehreren Spieltagen können die Spielzeiten nacheinander erfasst werden.

---

## 4.5 Startzeiten erzeugen

**Tool:** Starthefte  
**Menü:** Veranstaltung → Startzeiten erzeugen  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** **Veranstalter**

Mit dieser Funktion werden aus den definierten Programmen und Spielzeiten die konkreten Startzeiten erzeugt.

### Voraussetzungen

Vor dem Erzeugen der Startzeiten sollten:

- die Veranstaltung angelegt sein
- die Programme vollständig erfasst sein
- die Spielzeiten vollständig erfasst sein

### Vorgehen

1. Öffnen Sie **Veranstaltung → Startzeiten erzeugen**.
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

# 5. Starthefte

## 5.1 Startheft anzeigen

**Tool:** Starthefte  
**Menü:** Starthefte  
**Anmeldung:** nicht erforderlich  
**Erforderliche Rolle:** keine

Mit dieser Funktion kann das Startheft einer Veranstaltung angezeigt werden.

Das Startheft kann auch von Personen aufgerufen werden, die nicht bei K-Tool angemeldet sind.

### Vorgehen

1. Öffnen Sie **Starthefte**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Das Startheft wird angezeigt.

Diese Funktion eignet sich insbesondere für die öffentliche Anzeige eines Starthefts.

---

# 6. Buchen

## 6.1 Startzeiten buchen

**Tool:** Starthefte  
**Menü:** Buchen  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine besondere Rolle

Mit dieser Funktion können Startzeiten für Teilnehmer gebucht werden.

### Vorgehen

1. Öffnen Sie **Buchen**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Suchen Sie die gewünschte Startzeit.
4. Wählen Sie einen freien Startplatz.
5. Erfassen Sie die erforderlichen Angaben zum Teilnehmer.
6. Speichern Sie die Buchung.

Die gebuchte Startzeit wird anschließend als belegt angezeigt.

### Mehrere Buchungen

Bei mehreren Buchungen hintereinander können bereits eingegebene Angaben erneut verwendet werden.

Dies erleichtert die Erfassung mehrerer Startzeiten.

---

# 7. Stornieren

## 7.1 Startzeiten stornieren

**Tool:** Starthefte  
**Menü:** Stornieren  
**Anmeldung:** erforderlich  
**Erforderliche Rolle:** keine besondere Rolle

Mit dieser Funktion kann eine bestehende Buchung wieder aufgehoben werden.

### Vorgehen

1. Öffnen Sie **Stornieren**.
2. Wählen Sie die gewünschte Veranstaltung.
3. Suchen Sie die betreffende Startzeit.
4. Wählen Sie die bestehende Buchung.
5. Führen Sie die Stornierung aus.

Die Buchung wird entfernt.

Die Startzeit steht anschließend wieder für eine neue Buchung zur Verfügung.

---

# 8. Rollen und Berechtigungen

K-Tool verwendet verschiedene Rollen. Die Rolle bestimmt, welche Aufgaben ein Benutzer übernehmen darf.

| Rolle | Bedeutung |
|---|---|
| **Administrator** | Darf administrative Aufgaben und übergeordnete Funktionen ausführen. |
| **Veranstalter** | Darf Veranstaltungen im Rahmen seiner Aufgaben vorbereiten und bearbeiten. |
| **Gast** | Verfügt über eingeschränkte Berechtigungen. |

Nicht jede Funktion benötigt eine bestimmte Rolle.

Einige Funktionen:

- sind öffentlich zugänglich,
- benötigen lediglich eine Anmeldung,
- oder setzen eine bestimmte Rolle voraus.

---

# 9. Berechtigungsübersicht

| Tool | Menü | Funktion | Anmeldung | Erforderliche Rolle |
|---|---|---|---|---|
| Auth | Login | Anmeldung | Nein | Keine |
| Auth | Registrieren | Registrierung | Nein | Keine |
| Auth | Abmelden | Abmelden | Ja | Keine |
| Auth | Profil | Profil bearbeiten | Ja | Keine besondere Rolle |
| Auth | Passwort ändern | Passwort ändern | Ja | Keine besondere Rolle* |
| Auth | Benutzer → Benutzer anlegen | Benutzer anlegen | Ja | **Administrator** |
| Auth | Benutzer → Benutzer Rollen | Benutzerrollen verwalten | Ja | **Administrator** |
| Starthefte | Home | Startseite | Nein | Keine |
| Starthefte | Veranstaltung → Veranstaltung anlegen | Veranstaltung anlegen | Ja | **Administrator** |
| Starthefte | Veranstaltung → Veranstalter zuordnen | Veranstalter zuordnen | Ja | **Administrator** |
| Starthefte | Veranstaltung → Programme bearbeiten | Programme bearbeiten | Ja | **Veranstalter** |
| Starthefte | Veranstaltung → Spielzeiten bearbeiten | Spielzeiten bearbeiten | Ja | **Veranstalter** |
| Starthefte | Veranstaltung → Startzeiten erzeugen | Startzeiten erzeugen | Ja | **Veranstalter** |
| Starthefte | Starthefte | Startheft anzeigen | Nein | Keine |
| Starthefte | Buchen | Startzeiten buchen | Ja | Keine besondere Rolle |
| Starthefte | Stornieren | Startzeiten stornieren | Ja | Keine besondere Rolle |

\* Die Funktion „Passwort ändern“ ist vorgesehen, aber derzeit noch nicht verfügbar.

---

# 10. Typischer Ablauf einer Veranstaltung

Die Vorbereitung einer Veranstaltung erfolgt normalerweise in dieser Reihenfolge:

### 1. Veranstaltung anlegen

**Administrator**

**Tool:** Starthefte  
**Menü:** Veranstaltung → Veranstaltung anlegen

Die grundlegenden Daten der Veranstaltung werden erfasst.

↓

### 2. Veranstalter zuordnen

**Administrator**

**Tool:** Starthefte  
**Menü:** Veranstaltung → Veranstalter zuordnen

Der zuständige Veranstalter wird der Veranstaltung zugeordnet.

↓

### 3. Programme bearbeiten

**Veranstalter**

**Tool:** Starthefte  
**Menü:** Veranstaltung → Programme bearbeiten

Die Programme und Startintervalle werden festgelegt.

↓

### 4. Spielzeiten bearbeiten

**Veranstalter**

**Tool:** Starthefte  
**Menü:** Veranstaltung → Spielzeiten bearbeiten

Die Spieltage sowie Beginn und Ende der Spielzeiten werden festgelegt.

↓

### 5. Startzeiten erzeugen

**Veranstalter**

**Tool:** Starthefte  
**Menü:** Veranstaltung → Startzeiten erzeugen

Aus Programmen und Spielzeiten werden die konkreten Startzeiten erzeugt.

↓

### 6. Startheft anzeigen

**Alle**

**Tool:** Starthefte  
**Menü:** Starthefte

Das fertige Startheft kann angezeigt werden.

↓

### 7. Startzeiten buchen

**Angemeldete Benutzer**

**Tool:** Starthefte  
**Menü:** Buchen

Freie Startzeiten können gebucht werden.

↓

### 8. Startzeiten stornieren

**Angemeldete Benutzer**

**Tool:** Starthefte  
**Menü:** Stornieren

Bestehende Buchungen können bei Bedarf wieder aufgehoben werden.

---

# 11. Kurzüberblick für Benutzer

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

# 12. Hinweise zur Arbeit mit Startheften

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
