# Spezifikation Gesamtanlage Photovoltaik und Energiemanagement

## 1. Zweck und Geltungsbereich

Diese Spezifikation beschreibt das geplante Gesamtsystem zur Erzeugung, Speicherung und Nutzung elektrischer Energie im Gebäude. Sie bildet den übergeordneten Rahmen für die Photovoltaikanlage, den Batteriespeicher, die bestehende Wärmepumpe, den elektrischen Boiler sowie das Energiemanagement.

Die technischen Einzelanforderungen an die PV-Energiegewinnung und den Batteriespeicher sind in separaten Dokumenten festgehalten:

- [Spezifikation Energiegewinnung](energiegewinnung.md)
- [Spezifikation Batteriespeicher](batterieSpeicher.md)

Diese Systemübersicht ergänzt die beiden Spezifikationen. Bei Detailfragen gelten die Anforderungen der jeweils zuständigen Teilspezifikation; die Komponenten müssen als Gesamtsystem aufeinander abgestimmt werden.

## 2. Ziele des Gesamtsystems

Das Gesamtsystem soll den Eigenverbrauch der lokal erzeugten Solarenergie erhöhen, den Bezug elektrischer Energie aus dem öffentlichen Netz reduzieren und eine schrittweise Erweiterung ermöglichen.

Dabei gelten folgende Grundsätze:

- PV-Strom soll nach Möglichkeit zuerst direkt im Gebäude genutzt werden.
- Vorhandener PV-Überschuss soll – abhängig von Betriebszustand und technischen Grenzen – zum Laden der Batterie und für geeignete steuerbare Verbraucher genutzt werden.
- Die Batterie soll den Hausverbrauch bei ungenügender PV-Leistung unterstützen, damit der Netzbezug möglichst gering bleibt.
- Die Batterie soll im normalen Betriebsmodus nicht aus dem öffentlichen Netz geladen werden und nicht gezielt Batteriestrom ins öffentliche Netz einspeisen.
- Die bestehende Wärmepumpe und der elektrische Boiler sollen bei der Planung und, soweit technisch sinnvoll möglich, bei der Nutzung von PV-Überschuss berücksichtigt werden.
- Eine selbst aufgebaute Homeautomation auf Basis von Home Assistant soll Energieflüsse und geeignete Verbraucher koordinieren können. Die PV-Anlage darf dafür keine unnötige Bindung an eine bestimmte Cloud oder proprietäre Steuerungsplattform voraussetzen.
- Haushaltsgeräte wie Geschirrspüler, Waschmaschine und Wäschetrockner sollen abhängig von der Energiesituation betrieben werden können: teils mit automatischem Start nach ausdrücklicher Freigabe, teils über Startvorschläge.
- Vorrangiges Optimierungsziel ist, möglichst viel selbst erzeugten PV-Strom direkt im Gebäude zu nutzen. Dabei sollen Komfort, Gerätesicherheit und sinnvolle Nutzung der Batterie berücksichtigt werden.
- Der bevorstehende Küchenumbau soll genutzt werden, um erforderliche Stromkreise, Anschlüsse, Netzwerkverbindungen und mögliche Steuerungs- oder Messpunkte rechtzeitig vorzubereiten.
- Die Anlage soll modular aufgebaut sein: Die Erstinstallation bleibt begrenzt, spätere Erweiterungen sollen ohne unnötigen Austausch bereits installierter Komponenten möglich sein.
- Die Betriebsweise muss stabil, sicher und für den Betreiber nachvollziehbar sein.

## 3. Bestand und erste Ausbaustufe

### 3.1 Bestehende Verbraucher

Im Gebäude sind bereits folgende elektrische Verbraucher vorhanden:

- **Wärmepumpe:** bestehende CTA-Luft/Wasser-Wärmepumpe mit einer angegebenen elektrischen Leistung von ca. 3,7 kW. Die Wärmepumpe ist vorhanden und soll im Rahmen dieses Projekts nicht vorsorglich ersetzt werden. Zu prüfen ist, welche Steuerungs- und Kommunikationsschnittstellen verfügbar sind und wie sich der Betrieb sinnvoll mit PV-Erzeugung und Energiemanagement abstimmen lässt.
- **Elektrischer Boiler:** bestehender elektrisch betriebener Boiler. Seine genaue Funktion, sein Speichervolumen, seine elektrische Anschlussleistung und seine vorhandenen Steuerungsmöglichkeiten sind bei der Bestandsaufnahme zu erfassen.
- **Übriger Hausverbrauch:** Beleuchtung, Geräte und weitere elektrische Verbraucher werden als Teil des gesamten Hausverbrauchs durch die Anlage mitversorgt.

Die Angabe von 3,7 kW bei der Wärmepumpe ist als elektrische Leistungsangabe zu verstehen. Der tatsächliche momentane Verbrauch hängt vom Betriebszustand und den Betriebsbedingungen ab.

### 3.2 Erste Ausbaustufe der PV-Anlage

Gemäss der Spezifikation [Energiegewinnung](energiegewinnung.md) umfasst die erste Ausbaustufe:

- Rückbau des oberhalb der Ost-Dachfläche herausragenden Teils des stillgelegten Kamins und Vorbereitung des verbleibenden Kaminzugs als Kabelschacht;
- Installation von PV-Modulen auf der unteren West-Dachfläche C mit ca. 41 m² und ca. 15° Dachneigung.

Die Ost-Dachfläche A, die obere West-Dachfläche B und weitere nutzbare Flächen rund um das Gebäude bleiben zunächst ohne PV-Module. Die technische Planung soll spätere optionale Erweiterungen berücksichtigen.

Der Batteriespeicher wird gemäss [Spezifikation Batteriespeicher](batterieSpeicher.md) ausgelegt. Seine anfängliche Kapazität und eine mögliche spätere Erweiterung sind in der Offerte separat auszuweisen.

## 4. Systemkomponenten und Zusammenspiel

Das Gesamtsystem besteht funktional mindestens aus folgenden Komponenten:

1. **PV-Module:** Erzeugen elektrische Energie auf den jeweils belegten Dach- oder späteren Erweiterungsflächen.
2. **PV-/Batteriewechselrichter und gegebenenfalls weitere Wechselrichter:** Wandeln und steuern die Energieflüsse entsprechend der gewählten Systemarchitektur. Die Eignung für die erste Ausbaustufe und spätere Erweiterungen ist nachzuweisen.
3. **Energiemessung am Netzanschlusspunkt:** Erfasst Bezug und Einspeisung, damit das Energiemanagement den tatsächlichen Energiefluss des Gebäudes kennt.
4. **Batteriespeicher:** Nimmt PV-Überschuss auf und versorgt bei Bedarf die Verbraucher des Gebäudes. Die Einzelanforderungen stehen in der Batteriespeicher-Spezifikation.
5. **Energiemanagement und Home Assistant:** Home Assistant ist als geplante zentrale Homeautomation vorgesehen. Es soll Energieinformationen zusammenführen und Automationen für geeignete Verbraucher ermöglichen. Es ist zu klären, welche Funktionen durch das PV-/Batteriesystem selbst und welche durch Home Assistant übernommen werden.
6. **Bestehende Wärmepumpe und elektrischer Boiler:** Können bei geeigneter technischer Schnittstelle als steuerbare Verbraucher genutzt werden, um PV-Überschüsse sinnvoll einzusetzen.
7. **Haushaltsgeräte:** Geschirrspüler, Waschmaschine und Wäschetrockner sind erste Kandidaten für eine energieabhängige Betriebsplanung. Weitere geeignete Geräte können später ergänzt werden.
8. **Netzanschluss und erforderliche Schutz- und Messeinrichtungen:** Müssen für die gewählte Anlagenleistung, die geltenden Anschlussbedingungen und spätere Ausbaustufen geeignet sein.

Der Anbieter hat die vorgesehene Systemarchitektur in einem übersichtlichen Schema darzustellen und die Kommunikation zwischen Zähler, Wechselrichter, Batterie und steuerbaren Verbrauchern zu erläutern. Die geplante Homeautomation mit Home Assistant ist dabei als eigenständige, später umsetzbare Komponente zu berücksichtigen. Verfügbare lokale Schnittstellen, Protokolle, Messwerte und Steuerungsmöglichkeiten sind offenzulegen.

## 5. Energiemanagement und Energieprioritäten

Das Energiemanagement soll die Energieflüsse unter Berücksichtigung des aktuellen Verbrauchs, der PV-Leistung, des Batterieladezustands und der Betriebsbedingungen der Wärmepumpe und des Boilers koordinieren.

Als grundlegendes Zielbild gilt:

1. PV-Leistung versorgt zuerst den aktuellen Hausverbrauch.
2. Verfügbarer PV-Überschuss wird entsprechend der konfigurierten Betriebsstrategie für das Laden der Batterie und für geeignete steuerbare Verbraucher genutzt.
3. Wenn PV-Leistung und direkte Nutzung nicht ausreichen, versorgt die Batterie die Verbraucher gemäss ihrer verfügbaren Leistung und dem festgelegten Mindest-Ladezustand.
4. Der verbleibende Bedarf wird aus dem öffentlichen Netz gedeckt.
5. Überschüssige PV-Energie, die weder im Haus verbraucht noch gespeichert oder sinnvoll thermisch genutzt werden kann, darf gemäss den geltenden Anschluss- und Einspeiseregeln ins Netz abgegeben werden.

Die konkrete Priorisierung zwischen Batterieladung, Wärmepumpe, Boiler und weiteren steuerbaren Verbrauchern ist im Rahmen der Anlagen- und Homeautomation-Planung festzulegen. Das vorrangige Optimierungsziel ist, möglichst viel selbst erzeugten PV-Strom direkt im Gebäude zu nutzen und unnötige Einspeisung zu vermeiden. Dabei ist zu berücksichtigen, dass die Batterie späteren Hausverbrauch abdecken kann; ein Verbraucher soll nicht allein aufgrund eines kurzen Überschusses gestartet werden, wenn dies insgesamt zu einem ungünstigeren Betrieb führt.

Die Steuerungslogik soll mindestens den aktuellen Netzbezug bzw. die Netzeinspeisung, die PV-Leistung, den Batterieladezustand, den übrigen Hausverbrauch sowie bekannte zeitliche Anforderungen der Verbraucher berücksichtigen. Schwellenwerte, Verzögerungen und Prioritäten sollen konfigurierbar sein, damit die Steuerung nicht bei jeder kurzfristigen Leistungsschwankung reagiert.

Die Anforderungen an Batterieentladung, Mindest-SOC, Vermeidung von Netzladung und Vermeidung gezielter Einspeisung von Batteriestrom richten sich nach der [Spezifikation Batteriespeicher](batterieSpeicher.md).

## 6. Einbindung der bestehenden Wärmepumpe

Die vorhandene CTA-Luft/Wasser-Wärmepumpe hat eine angegebene elektrische Leistung von ca. 3,7 kW. Sie ist als wesentlicher elektrischer Verbraucher in der Planung zu berücksichtigen.

Der Anbieter hat festzustellen und zu dokumentieren:

- Hersteller, genaue Modellbezeichnung und verfügbare technische Dokumentation;
- welche Schnittstellen für eine externe Steuerung vorhanden sind, zum Beispiel ein PV-/SG-Ready-Eingang, ein Freigabekontakt oder eine geeignete digitale Kommunikationsschnittstelle;
- ob und wie Betriebszustände oder Leistungsaufnahme an das Energiemanagement übermittelt werden können;
- welche Betriebsgrenzen, Sperrzeiten und Mindestlaufzeiten einzuhalten sind;
- ob die Wärmepumpe so angesteuert werden kann, dass geeignete Wärmebedarfe bevorzugt bei PV-Überschuss gedeckt werden, ohne Komfort, Effizienz oder sicheren Betrieb zu beeinträchtigen.

Eine konkrete Steuerungsmethode darf erst festgelegt werden, nachdem die vorhandenen Schnittstellen und die Herstellervorgaben geprüft wurden. Die Wärmepumpe soll nicht allein aufgrund einer angenommenen Schnittstelle als steuerbar vorausgesetzt werden.

## 7. Einbindung des elektrischen Boilers

Der bestehende elektrische Boiler soll bei der Planung als möglicher thermischer Speicher für PV-Überschüsse berücksichtigt werden.

Der Anbieter hat bei der Bestandsaufnahme zu klären:

- Speichervolumen und vorhandene elektrische Anschlussleistung;
- vorhandene Regelung, Temperaturfühler und Schaltmöglichkeiten;
- ob eine externe, sichere und mit den Herstellervorgaben vereinbare Ansteuerung möglich ist;
- welche Temperaturgrenzen und Schutzfunktionen einzuhalten sind;
- ob der Boiler unabhängig von oder in Abstimmung mit der Wärmepumpe betrieben wird.

Wenn eine geeignete Steuerung möglich ist, soll das Energiemanagement den Boiler bevorzugt dann betreiben, wenn PV-Überschuss verfügbar ist und Wärmebedarf besteht. Dabei sind unnötiges Aufheizen, Komfortanforderungen, die vorgesehenen Temperaturgrenzen und alle erforderlichen Schutzfunktionen zu berücksichtigen.

Eine Steuerung des Boilers darf vorhandene Sicherheits- oder Temperaturregelungen nicht umgehen. Falls keine geeignete Schnittstelle vorhanden ist, soll der Anbieter die technisch und wirtschaftlich sinnvollen Alternativen ausweisen.

## 8. Home Assistant und energieabhängiger Betrieb von Haushaltsgeräten

Für die Homeautomation ist ein selbst aufgebautes System auf Basis von Home Assistant vorgesehen. Es soll die Energieinformationen der PV-Anlage, des Batteriespeichers und des Netzanschlusspunkts nutzen und bei geeigneten Geräten energieabhängige Betriebsabläufe ermöglichen. Die genaue Umsetzung wird in einer separaten Spezifikation der Homeautomation festgelegt; diese Systemübersicht definiert die Anforderungen an die Schnittstellen und die Abstimmung mit der Energieanlage.

### 8.1 Vorgesehene Geräte

Als erste Kandidaten sind vorgesehen:

- Geschirrspüler;
- Waschmaschine;
- Wäschetrockner.

Weitere geeignete Verbraucher können später ergänzt werden. Auch bei der Küchenplanung sollen mögliche zusätzliche Geräte und Automationen berücksichtigt werden, ohne bereits jetzt eine abschliessende Geräteliste vorauszusetzen.

### 8.2 Kombination aus automatischem Start und Startvorschlägen

Die Steuerung soll zwei Betriebsarten ermöglichen:

- **Automatischer Start:** Ein Gerät darf automatisch gestartet werden, wenn der Betreiber diesen Automatikbetrieb für das Gerät ausdrücklich freigegeben hat, die Geräteschnittstelle den Start zuverlässig unterstützt und die definierten Energie- und Zeitbedingungen erfüllt sind.
- **Startvorschlag:** Wenn ein sicherer automatischer Start nicht möglich oder nicht freigegeben ist, soll Home Assistant einen geeigneten Startzeitpunkt vorschlagen bzw. den Betreiber informieren, dass genügend selbst erzeugte Energie verfügbar ist.

Ein Gerät darf nicht allein durch das Unterbrechen und Wiederherstellen seiner Stromversorgung gestartet werden, sofern dies nicht ausdrücklich vom Hersteller vorgesehen und für das Gerät sicher ist. Bevorzugt werden dokumentierte Geräteschnittstellen oder vom Hersteller vorgesehene Funktionen verwendet.

### 8.3 Entscheidungsgrundlagen

Die Automatisierung soll – soweit die erforderlichen Messwerte verfügbar sind – berücksichtigen:

- aktuelle PV-Erzeugung und den tatsächlichen Energiefluss am Netzanschlusspunkt;
- aktuellen Hausverbrauch und laufende grössere Verbraucher, insbesondere Wärmepumpe und Boiler;
- Batterieladezustand und Lade-/Entladeleistung;
- erwartete bzw. verfügbare PV-Leistung, sofern eine geeignete Prognose vorhanden ist;
- manuelle Freigabe, gewünschte Fertigstellungszeit und weitere vom Betreiber gesetzte Zeitvorgaben;
- Prioritäten zwischen den Geräten sowie die zulässige Gesamtlast.

Die erste Zielsetzung ist, möglichst viel selbst erzeugten PV-Strom direkt zu verbrauchen. Die Steuerung soll aber keine unnötigen Wasch- oder Trocknungsvorgänge auslösen und keine wichtigen Zeitvorgaben oder Sicherheitsbedingungen verletzen. Bei fehlenden oder unplausiblen Messwerten muss die Automatik in einen definierten sicheren Zustand wechseln und darf keine unkontrollierten Starts auslösen.

### 8.4 Koordination und Bedienung

Die Steuerung soll mehrere Geräte koordinieren können. Beispielsweise kann die Waschmaschine zuerst und der Trockner anschliessend betrieben werden, sofern Energieangebot, Zeitvorgaben und Geräteeigenschaften dies zulassen. Gleichzeitige hohe Lasten sollen bei Bedarf vermieden werden.

Der Betreiber muss erkennen können, ob ein Gerät auf Automatik freigegeben ist, auf einen Start wartet, einen Startvorschlag erhalten hat oder gerade läuft. Ein manueller Start muss weiterhin möglich sein; manuelle Eingriffe sollen von der Automatik respektiert werden.

### 8.5 Schnittstellen und Zuständigkeiten

Der PV-Anbieter soll dokumentieren, welche Energie- und Gerätemesswerte lokal über geeignete Schnittstellen verfügbar sind und ob bzw. wie ein externes Energiemanagement darauf zugreifen kann. Die Anlage soll nach Möglichkeit offene, dokumentierte und lokal nutzbare Schnittstellen unterstützen. Eine vollständige Home-Assistant-Installation ist nicht zwingend Bestandteil der PV-Erstinstallation; notwendige Zähler, Kommunikationsschnittstellen und sinnvolle Vorbereitungen sind jedoch in der Offerte auszuweisen.

Die sicherheitsrelevante Regelung von Wärmepumpe, Boiler und Haushaltsgeräten verbleibt bei den jeweiligen Geräten bzw. ihren dafür vorgesehenen Schutz- und Regelungssystemen. Home Assistant darf diese Funktionen nicht umgehen.

## 9. Küchenumbau und bauliche Vorbereitung

Der bevorstehende Küchenumbau soll frühzeitig mit der PV- und Homeautomation-Planung abgestimmt werden. Ziel ist, spätere Automationen und Messungen zu ermöglichen, ohne dafür erneut Wände, Möbel oder Installationen öffnen zu müssen.

Bei der Küchenplanung sind – in Abstimmung mit einer Elektrofachperson – insbesondere zu prüfen:

- passende und ausreichend dimensionierte Stromkreise für Geschirrspüler, Backofen, Kochfeld, Kühlschrank und weitere vorgesehene Geräte;
- sichere und normgerechte Möglichkeiten zur Messung des Energieverbrauchs einzelner Geräte oder Stromkreise, falls dies für die Automationen erforderlich ist;
- Netzwerk- und Funkabdeckung am vorgesehenen Standort von Geräten und Steuerungskomponenten;
- Platz und Zugänglichkeit für zusätzliche Messgeräte, Aktoren oder Kommunikationsmodule;
- Leitungswege und Reservekapazitäten für spätere Ergänzungen;
- Beleuchtung, Präsenz- oder Türsensoren sowie weitere gewünschte Homeautomation-Funktionen.

Es sind nicht vorsorglich alle Geräte intelligent zu schalten. Vorbereitungen sollen auf den geplanten Bedarf und auf wirtschaftlich sinnvolle Erweiterungsmöglichkeiten abgestimmt werden. Arbeiten an festen elektrischen Installationen sind durch qualifizierte Fachpersonen auszuführen.

## 10. Messung, Überwachung und Bedienung

Das Gesamtsystem soll die wesentlichen Energieflüsse nachvollziehbar anzeigen. Mindestens folgende Messwerte bzw. Zustände sollen – soweit die jeweilige Komponente sie bereitstellt – verfügbar sein:

- aktuelle PV-Erzeugungsleistung;
- aktueller Hausverbrauch;
- Netzbezug und Netzeinspeisung am Netzanschlusspunkt;
- Lade- bzw. Entladeleistung und Ladezustand der Batterie;
- Betriebszustand und elektrische Leistungsaufnahme der Wärmepumpe;
- Betriebszustand und Leistungsaufnahme des Boilers, sofern mess- oder auslesbar;
- Fehlermeldungen und Kommunikationsstatus der wesentlichen Systemkomponenten.

Die Offerte soll beschreiben, welche Werte direkt gemessen und welche aus Geräteinformationen übernommen werden. Mess- und Steuerfunktionen dürfen nicht allein aufgrund einer grafischen Anzeige als vorhanden gelten.

## 11. Modularität und spätere Erweiterbarkeit

Das System ist für einen stufenweisen Ausbau vorzusehen. Neben den in der Energiegewinnungs-Spezifikation beschriebenen optionalen PV-Flächen ist auch die Erweiterbarkeit des Batteriespeichers gemäss der Batteriespeicher-Spezifikation zu berücksichtigen.

Der Anbieter soll darstellen, welche Komponenten bei der Erstinstallation bereits endgültig dimensioniert werden müssen und welche später ergänzt oder erweitert werden können. Dabei sind insbesondere zu betrachten:

- Wechselrichterleistung, zusätzliche Wechselrichter und MPP-Tracker;
- String-Anschlüsse und Leitungswege zu den zunächst ungenutzten Flächen;
- Leistungsgrenzen des Netzanschlusses und erforderliche Meldungen oder Bewilligungen;
- Erweiterbarkeit der Batteriekapazität;
- verfügbare EMS-Ein- und Ausgänge sowie unterstützte Kommunikationsprotokolle;
- lokale Schnittstellen und verfügbare Messwerte für Home Assistant;
- Schnittstellen zur Wärmepumpe, zum Boiler und zu den vorgesehenen Haushaltsgeräten;
- erforderliche bauliche und elektrische Vorbereitungen beim Küchenumbau;
- Kosten für sinnvolle Vorbereitungen bei der Erstinstallation gegenüber nachträglichen Umbauten.

Die Offerte muss die Kosten der ersten Ausbaustufe von optionalen Vorbereitungen und späteren Erweiterungen trennen. Erweiterbarkeit ist anhand konkreter technischer Angaben und nicht nur mit einer allgemeinen Herstellerzusage zu belegen.

## 12. Anforderungen an die Offerte

Der Anbieter soll mindestens folgende Unterlagen und Angaben liefern:

1. Systemübersicht bzw. Schema mit allen wesentlichen Komponenten und Energieflüssen.
2. Beschreibung der ersten Ausbaustufe und der möglichen späteren Erweiterungen.
3. Separate Ausweisung der PV-Leistung und des erwarteten Ertrags je geplanter Ausbaustufe.
4. Angaben zu Wechselrichter, MPP-Trackern, Strings und den Erweiterungsmöglichkeiten.
5. Angaben zu Batteriespeicher, nutzbarer Kapazität, Lade-/Entladeleistung und späterer Kapazitätserweiterung.
6. Beschreibung der Messung am Netzanschlusspunkt und der Regelung gegen unnötigen Netzbezug.
7. Ergebnis der Schnittstellenprüfung für die bestehende Wärmepumpe und den elektrischen Boiler.
8. Beschreibung der vorgesehenen Nutzung von PV-Überschüssen für Batterie und steuerbare Verbraucher.
9. Auflistung benötigter zusätzlicher Zähler, Sensoren, Kommunikationsmodule und Steuergeräte.
10. Getrennte Kosten für die erste Ausbaustufe, sinnvolle vorbereitende Massnahmen und optionale spätere Erweiterungen.
11. Benennung technischer Einschränkungen, Annahmen und noch offener Abklärungen.
12. Angaben zu lokal verfügbaren Schnittstellen für Home Assistant, einschliesslich allfälliger Lizenz-, Cloud- oder Zusatzhardware-Anforderungen.
13. Auflistung der sinnvollen elektrischen, Netzwerk- und Messvorbereitungen, die im Rahmen der PV-Erstinstallation bzw. des Küchenumbaus berücksichtigt werden sollten.

## 13. Inbetriebnahme und Abnahme

Bei der Inbetriebnahme sind die wesentlichen Funktionen des Gesamtsystems zu prüfen und zu dokumentieren. Die Prüfungen ergänzen die spezifischen Abnahmekriterien in den Dokumenten [Energiegewinnung](energiegewinnung.md) und [Batteriespeicher](batterieSpeicher.md).

Mindestens zu prüfen sind:

- PV-Erzeugung und korrekte Anzeige der wesentlichen Energieflüsse;
- korrektes Messen von Netzbezug und Netzeinspeisung am Netzanschlusspunkt;
- Laden der Batterie bei PV-Überschuss und bedarfsgerechte Entladung gemäss Batteriespeicher-Spezifikation;
- Vermeidung einer Batterieladung aus dem öffentlichen Netz im normalen Betriebsmodus;
- Vermeidung einer gezielten Einspeisung von Batteriestrom ins öffentliche Netz;
- Funktion der freigegebenen Steuerung von Wärmepumpe und Boiler, sofern diese technisch eingebunden werden;
- Verhalten bei Kommunikationsausfall oder fehlerhaften Messwerten;
- Dokumentation der für spätere Erweiterungen vorgesehenen Anschlüsse, Reserven und technischen Grenzen.

Die Inbetriebnahme soll mit einer verständlichen Anlagendokumentation und einer Einführung für den Betreiber abgeschlossen werden.

## 14. Noch offene Grundlagen

Folgende Angaben sind bei der Detailplanung zu erheben oder zu bestätigen:

- genaue Modellbezeichnung und Schnittstellen der bestehenden CTA-Wärmepumpe;
- elektrische Anschlussleistung, Speichervolumen und Steuerungsmöglichkeiten des Boilers;
- tatsächlicher Haushaltsstromverbrauch und zeitliches Verbrauchsprofil;
- konkrete Modulbelegung, Leistung und Ertragsprognose der ersten PV-Ausbaustufe;
- anfängliche Batteriekapazität und mögliche spätere Erweiterung;
- technische Architektur und Betriebsstrategie des Energiemanagements;
- Schnittstellenstrategie zwischen Home Assistant, PV-/Batteriesystem, Wärmepumpe, Boiler und Haushaltsgeräten;
- gewünschte Automatikfreigaben, Startvorschläge und Zeitvorgaben für Haushaltsgeräte;
- Umfang der beim Küchenumbau vorzusehenden elektrischen, Netzwerk- und Messvorbereitungen;
- Anforderungen des zuständigen Netzbetreibers an Netzanschluss, Messung und Einspeisung.
