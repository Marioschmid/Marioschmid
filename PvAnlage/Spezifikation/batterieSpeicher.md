# Batteriespeicher

## 1. Ziel

Der Batteriespeicher dient primär dazu, den Eigenverbrauch der Photovoltaikanlage zu erhöhen und den Bezug elektrischer Energie aus dem öffentlichen Stromnetz möglichst weitgehend zu vermeiden.

Die Batterie soll insbesondere dann Energie an das Haus abgeben, wenn am Netzanschlusspunkt ein Bezug festgestellt wird.

Der Speicher ist damit nicht primär für Arbitragegeschäfte mit dem Stromnetz oder für eine gezielte Einspeisung von Batteriestrom in das öffentliche Netz vorgesehen.

## 2. Grundprinzip

Die Energieversorgung des Hauses soll nach Möglichkeit in folgender Reihenfolge erfolgen:

1. direkte Versorgung des Hausverbrauchs durch die PV-Anlage,
2. Laden der Batterie mit vorhandenem PV-Überschuss,
3. Versorgung des Hausverbrauchs aus der Batterie, sobald die PV-Leistung den aktuellen Verbrauch nicht mehr deckt,
4. Bezug aus dem öffentlichen Stromnetz nur dann, wenn PV-Leistung und verfügbare Batterieleistung den aktuellen Verbrauch nicht decken können.

Soweit technisch möglich, soll am Netzanschlusspunkt ein möglichst geringer beziehungsweise kein Netzbezug entstehen, solange ausreichend Energie in der Batterie vorhanden ist.

## 3. Messung am Netzanschlusspunkt

Die Regelung des Batteriespeichers muss den tatsächlichen Energiefluss zwischen Hausinstallation und öffentlichem Stromnetz erfassen können.

Massgebend für die Lade- und Entladeentscheidung ist der Energiefluss am Netzanschlusspunkt und nicht allein die momentan von der PV-Anlage erzeugte Leistung.

Die Messung muss insbesondere unterscheiden können zwischen:

- Bezug aus dem öffentlichen Stromnetz,
- Einspeisung in das öffentliche Stromnetz,
- Versorgung des Hauses aus PV und Batterie.

## 4. Entladeverhalten

Wird am Netzanschlusspunkt ein Netzbezug festgestellt und steht ausreichend Energie in der Batterie zur Verfügung, soll die Batterie Energie an das Haus abgeben.

Beispiel:

- Hausverbrauch: 2.5 kW
- PV-Leistung: 1.0 kW
- Netzbezug: 1.5 kW
- Batterieabgabe: möglichst ca. 1.5 kW
- verbleibender Netzbezug: möglichst 0 kW

Die Regelung muss dabei berücksichtigen:

- maximale Entladeleistung der Batterie,
- aktuellen Ladezustand (State of Charge, SOC),
- minimale zulässige Batteriereserve,
- technische Grenzen des Wechselrichters,
- Mess- und Regelverzögerungen.

## 5. Vermeidung unnötiger Netzbezüge

Die Regelung soll nicht bei jeder kurzfristigen Schwankung des Energieflusses zwischen Laden und Entladen wechseln.

Dazu sind geeignete Regelparameter vorzusehen, insbesondere:

- Messintervall,
- Reaktionszeit,
- Mindestleistung für eine Lade-/Entladeanforderung,
- Hysterese beziehungsweise Totzone,
- Mindestdauer eines Zustandswechsels.

Ziel ist ein stabiler Betrieb ohne unnötiges Hin- und Herschalten des Batteriespeichers.

## 6. Laden der Batterie

Die Batterie soll im normalen Betriebsmodus ausschliesslich mit überschüssiger Energie der PV-Anlage geladen werden.

Ein Laden der Batterie aus dem öffentlichen Stromnetz soll im normalen Betriebsmodus ausgeschlossen sein.

Beispiel:

- PV-Leistung: 5.0 kW
- Hausverbrauch: 2.0 kW
- verfügbarer PV-Überschuss: 3.0 kW
- Batterie wird mit möglichst bis zu 3.0 kW geladen, soweit Ladeleistung und Ladezustand dies zulassen.

Bei vollständig geladener Batterie wird der verbleibende PV-Überschuss gemäss der vorgesehenen Einspeiseregelung ins öffentliche Netz abgegeben.

## 7. Keine gezielte Einspeisung von Batteriestrom

Batteriestrom soll im normalen Betriebsmodus nicht gezielt in das öffentliche Stromnetz eingespeist werden.

Die Regelung soll deshalb verhindern, dass durch die Batterie bei fehlendem Hausverbrauch eine Einspeisung ins öffentliche Netz entsteht.

Wenn die Batterie entlädt, soll die Leistung grundsätzlich auf den aktuellen Hausverbrauch begrenzt werden.

Beispiel:

- Hausverbrauch: 0.8 kW
- PV-Leistung: 0 kW
- Batterie könnte 5 kW liefern
- zulässige Batterieabgabe: höchstens ungefähr 0.8 kW
- Ziel am Netzanschlusspunkt: kein beziehungsweise möglichst kein Netzbezug und keine gezielte Batterieeinspeisung.

## 8. Mindestreserve

Für die Batterie ist ein konfigurierbarer Mindest-Ladezustand (SOC) vorzusehen.

Unterhalb dieses SOC soll die Batterie den Hausverbrauch nicht mehr vollständig ausgleichen, damit eine definierte Energiereserve erhalten bleibt.

Die Höhe der Reserve ist als Anlagenparameter festzulegen und soll später ohne Änderung der grundlegenden Regelungslogik angepasst werden können.

## 9. Betriebsarten

Die Anlage soll mindestens folgende Betriebszustände unterscheiden können:

### 9.1 PV-Überschuss

PV-Leistung ist grösser als der aktuelle Hausverbrauch.

- Haus wird direkt durch PV versorgt.
- Überschuss lädt die Batterie.
- Nach Erreichen des maximalen SOC wird der verbleibende Überschuss eingespeist.

### 9.2 PV deckt Verbrauch nicht vollständig

PV-Leistung ist kleiner als der aktuelle Hausverbrauch.

- PV versorgt das Haus mit der verfügbaren Leistung.
- Batterie übernimmt den verbleibenden Verbrauch, soweit SOC und maximale Entladeleistung dies zulassen.
- Nur der verbleibende Rest wird aus dem Netz bezogen.

### 9.3 Keine ausreichende PV-Leistung

PV liefert keine beziehungsweise nicht genügend Leistung.

- Batterie versorgt das Haus, soweit möglich.
- Wird der minimale SOC erreicht oder reicht die maximale Entladeleistung nicht aus, erfolgt der verbleibende Bezug aus dem öffentlichen Netz.

### 9.4 Batterie voll

Ist die Batterie vollständig geladen, wird überschüssige PV-Energie gemäss der vorgesehenen Einspeiseregelung ins öffentliche Netz eingespeist.

### 9.5 Batterie leer beziehungsweise Mindest-SOC erreicht

Bei Erreichen des definierten Mindest-SOC wird die Batterieentladung beendet oder auf die konfigurierte Reserve beschränkt. Der verbleibende Hausverbrauch wird aus dem öffentlichen Netz gedeckt.

## 10. Netzbezug und Netznutzungsentgelt

Für die Planung ist zwischen PV-Energie und Netzenergie zu unterscheiden.

PV-Energie, die direkt im Haus verbraucht oder zunächst in der Batterie gespeichert und später im Haus verbraucht wird, soll nicht als Netzbezug behandelt werden.

Netzenergie, die das Haus aus dem öffentlichen Netz bezieht, bleibt dagegen normaler Netzbezug.

Die Anlage ist deshalb so zu konfigurieren, dass die Batterie im normalen Betriebsmodus nicht aus dem öffentlichen Netz geladen wird.

Die konkrete Messung, Abrechnung und allfällige zusätzliche Messeinrichtungen sind mit dem zuständigen Netzbetreiber, insbesondere BKW, vor der Installation zu klären.

## 11. Anforderungen an Wechselrichter und Energiemanagement

Die angebotene Lösung muss mindestens folgende Eigenschaften unterstützen:

- Messung des Energieflusses am Netzanschlusspunkt,
- automatische Regelung der Batterie anhand dieses Energieflusses,
- PV-Überschussladen,
- bedarfsgerechte Batterieentladung,
- Begrenzung der Batterieabgabe auf den tatsächlichen Hausverbrauch,
- konfigurierbarer Mindest-SOC,
- konfigurierbare Regelparameter,
- Verhinderung einer unbeabsichtigten Batterieladung aus dem Netz,
- Verhinderung einer unbeabsichtigten Einspeisung von Batteriestrom,
- Anzeige von PV-Leistung, Hausverbrauch, Batterie-Leistung, SOC, Netzbezug und Netzeinspeisung.

Die Kommunikation zwischen Energiezähler, Energiemanagementsystem und Batterie-/PV-Wechselrichter muss für eine ausreichend schnelle Regelung ausgelegt sein.

## 12. Verhalten bei Kommunikations- oder Messfehlern

Bei Ausfall oder fehlerhaften Werten der Messung am Netzanschlusspunkt muss ein sicherer Betriebszustand gewährleistet sein.

Insbesondere darf ein Mess- oder Kommunikationsfehler nicht dazu führen, dass die Batterie unkontrolliert ins öffentliche Netz einspeist oder unkontrolliert aus dem öffentlichen Netz geladen wird.

Das konkrete Fehlerverhalten ist Bestandteil der Anlagenplanung und mit dem Hersteller beziehungsweise Installateur festzulegen.

## 13. Anforderungen an die Offerte

Der Installateur soll in der Offerte ausdrücklich bestätigen:

1. an welcher Stelle der Energiefluss gemessen wird,
2. welches Messgerät verwendet wird,
3. wie die Batterie bei erkanntem Netzbezug geregelt wird,
4. ob die Batterie aus dem öffentlichen Netz geladen werden kann,
5. wie das Laden aus dem öffentlichen Netz verhindert wird,
6. wie eine Einspeisung von Batteriestrom ins öffentliche Netz verhindert wird,
7. welcher Mindest-SOC vorgesehen ist,
8. welche maximale Lade- und Entladeleistung zur Verfügung steht,
9. welche Regelverzögerung beziehungsweise Regelgenauigkeit am Netzanschlusspunkt erreicht wird,
10. welche zusätzlichen Zähler oder Messeinrichtungen für BKW erforderlich sind,
11. wie die Anlage bei Kommunikations- oder Messfehlern reagiert.

## 14. Abnahmekriterien

Die Funktion ist nach der Installation anhand realer Betriebszustände zu prüfen.

Mindestens folgende Tests sind durchzuführen:

- PV-Leistung grösser als Hausverbrauch: Batterie wird mit Überschuss geladen.
- PV-Leistung kleiner als Hausverbrauch: Batterie übernimmt den fehlenden Anteil.
- Batterie ausreichend geladen: Netzbezug wird auf das technisch mögliche Minimum reduziert.
- Batterie erreicht Mindest-SOC: weiterer Verbrauch wird aus dem Netz gedeckt.
- Kein Hausverbrauch bei nicht ausreichender PV-Leistung: Batterie speist nicht gezielt ins öffentliche Netz ein.
- Batterie darf im normalen Betriebsmodus nicht aus dem öffentlichen Netz geladen werden.
- Kurzzeitige Lastschwankungen führen nicht zu instabilem Lade-/Entladeverhalten.

Die tatsächlich erreichbare Restmenge an Netzbezug ist abhängig von Messgenauigkeit, Regelgeschwindigkeit, Wechselrichterleistung und kurzfristigen Laständerungen. Ein dauerhafter Wert von exakt 0 W Netzbezug ist deshalb nicht als technische Voraussetzung festzulegen; Ziel ist eine möglichst weitgehende Vermeidung des Netzbezugs.
