# __Einführung__

## Beschreibung

Cardholder ist eine Applikation, die es ermöglicht online Kartenspiele
zu spielen. Dabei kann man mit Freunden und Menschen aus aller Welt
spielen. Es gibt eine Auswahl von verschiedenen Kartenspielen. Die
Nutzer können die Kartenspiele ohne Anmeldung spielen. Spieler sollen
andere Nutzer zu einem Spiel einladen können. Cardholder ist als App und
als Webseite verfügbar.

## Ziele

Das Ziel von Cardholder ist es, dass Familie, Freunde und
Kartenspiel-Begeisterte zusammen Kartenspiele spielen können. Die
Motivation ist eine freie und für jeden zugängliche Software
bereitzustellen. Es werden verschiedene Kartenspiele zur Verfügung
gestellt.

Cardholder setzt vorraus, dass die Nutzer die entsprechenden Regeln der
jeweiligen Kartenspiele kennen. Weitere Vorkenntnisse sind nicht
erforderlich.

Bei Cardholder ist es nicht möglich eigene Kartenspiele hinzuzufügen.
Des Weiteren ist es nicht möglich seinen Spielstand zu speichern.

# __Anforderungen__

## Stakeholder

| Funktion | Name | Kontakt | Verfügbarkeit | Wissen | Interesse & Ziele | Relevanz |
|:---------|:-----|:--------|:--------------|:-------|:------------------|:---------|
|          |      |         |               |        |                   |          |


Beispiel

| Funktion              | Name        | Kontakt        | Verfügbarkeit                                                           | Wissen                                                                  | Interesse & Ziele                         | Relevanz                                                   |
|:----------------------|:------------|:---------------|:------------------------------------------------------------------------|:------------------------------------------------------------------------|:------------------------------------------|:-----------------------------------------------------------|
| Leiter der Bibliothek | Herr Bauer  | Tel. 409000    | Von 9-19 Uhr telefonisch erreichbar, Mitarbeit zu 30% möglich, Nürnberg | Kennt das Altsystem aus der Anwendersicht, soll mit dem System arbeiten | Vereinfachung der Ausleihprozesse         | Fachlicher Entscheider                                     |
| Administrator         | Herr Heiner | Heiner@gmx.net | Per E-Mail, immer erreichbar, Verfügbarkeit 50%, Nürnberg               | Vertraut mit vergleichbarer Verwaltungssoftware                         | Stabiles System, geringer Wartungsaufwand | Informationslieferant bzgl. Wartungsanforderungen          |
| Product-Owner         | Paul Ottmer | po@ottmer.de   | Per E-Mail und tel. tagsüber, Verfügbarkeit 100%, Nürnberg              | Koordinator für die Inputs der Stakeholder                              | ROI des Systems sicherstellen             | Entscheider - als Koordinator der Stakeholderanforderungen |

## Funktionale Anforderungen

    - Use-Case Diagramme
    - Strukturierung der Diagramme in funktionale Gruppen

## Nicht-funktionale Anforderungen

### Rahmenbedingungen

    - Normen, Standards, Protokolle, Hardware, externe Vorgaben

### Betriebsbedingungen

__Mindestanforderungen an den Web Browser für die Web Anwendung__

| Browser           | Version |
|:------------------|:--------|
| Internet Explorer | 11      |
| Edge              | 15      |
| Firefox           | 54      |
| Chrome            | 51      |
| Safari            | 10      |
| Opera             | 38      |

__Mindestanforderungen an das mobile Endgerät für die App__

| Betriebssystem | Version |
|:---------------|:--------|
| iOS            | 8       |
| Android (ARM)  | 4.1     |

__Mindestanforderungen an den Server für das Backend__

| Programmiersprache | Version |
|:-------------------|:--------|
| Python             | 3.5     |

### Qualitätsmerkmale

| Qualitätsmerkmal           |      sehr gut      |        gut         |       normal       |   nicht relevant   |
|:---------------------------|:------------------:|:------------------:|:------------------:|:------------------:|
| **Zuverlüssigkeit**        |                    |                    |                    |                    |
| Fehlertoleranz             |         -          |         -          | :heavy_check_mark: |         -          |
| Wiederherstellbarkeit      |         -          |         -          |         -          | :heavy_check_mark: |
| Ordnungsmäßigkeit          |         -          |         -          |         -          | :heavy_check_mark: |
| Richtigkeit                |         -          | :heavy_check_mark: |         -          |         -          |
| Konformität                |         -          |         -          |         -          | :heavy_check_mark: |
| **Benutzerfreundlichkeit** |                    |                    |                    |                    |
| Installierbarkeit          | :heavy_check_mark: |         -          |         -          |         -          |
| Verständlichkeit           | :heavy_check_mark: |         -          |         -          |         -          |
| Erlernbarkeit              | :heavy_check_mark: |         -          |         -          |         -          |
| Bedienbarkeit              | :heavy_check_mark: |         -          |         -          |         -          |
| **Performance**            |                    |                    |                    |                    |
| Zeitverhalten              |         -          | :heavy_check_mark: |         -          |         -          |
| Effizienz                  | :heavy_check_mark: |         -          |         -          |         -          |
| **Sicherheit**             |                    |                    |                    |                    |
| Analysierbarkeit           |         -          |         -          |         -          | :heavy_check_mark: |
| Modifizierbarkeit          |         -          |         -          | :heavy_check_mark: |         -          |
| Stabilität                 |         -          | :heavy_check_mark: |         -          |         -          |
| Prüfbarkeit                |         -          |         -          |         -          | :heavy_check_mark: |

## Graphische Benutzerschnittstelle

    - GUI-Mockups passend zu User Stories
    - Screens mit Überschrift kennzeichnen, die im Inhaltsverzeichnis zu sehen ist
    - Unter den Screens darstellen (bzw. verlinken), welche User Stories mit dem Screen abgehandelt werden
    - Modellierung der Navigation zwischen den Screens der GUI-Mockups als Zustandsdiagramm

## Anforderungen im Detail

    - User Stories mit Akzeptanzkritierien 
    - Optional: Name (oder ID) und Priorität ("Must", "Should", "Could", "Won't")
    - Strukturierung der User Stories in funktionale Gruppen

### Schablone für User Stories

| **Als** | **möchte ich** | **so dass** | **Akzeptanz**   |
|:--------|:---------------|:------------|:----------------|
| Wer     | Was            | Warum       | Wann akzeptiert |

Beispiel 1

| **Als**  | **möchte ich**                                | **so dass**     | **Akzeptanz**         |
|:---------|:----------------------------------------------|:----------------|:----------------------|
| Benutzer | bei Fehleingabe die Lösung angezeigt bekommen | ich lernen kann | Lösung wird angezeigt |

Beispiel 2

| **Name** | **In meiner Rolle als**... | ...**möchte ich**...                          | ..., **so dass**... | **Erf�llt, wenn**...  | **Priorit�t** |
|:---------|:--------------------------:|:----------------------------------------------|:--------------------|:----------------------|:--------------|
| Lernen   |          Benutzer          | bei Fehleingabe die Lösung angezeigt bekommen | ich lernen kann     | Lösung wird angezeigt | Muss          |


# __Technische Beschreibung__

## Systemübersicht

    - Systemarchitekturdiagramm ("Box-And-Arrow" Diagramm)
    - Kommunikationsprotokolle, Datenformate

## Softwarearchitektur

    - Darstellung von Softwarebausteinen (Module, Schichten, Komponenten)

## Schnittstellen

    - Schnittstellenbeschreibung
    - Auflistung der nach außen sichtbaren Schnittstelle der Softwarebausteine

## Datenmodell

    - Konzeptionelles Analyseklassendiagramm (logische Darstellung der Konzepte der Anwendungsdom�ne)
    - Modellierung des physikalischen Datenmodells 
      - RDBMS: ER-Diagramm bzw. Dokumentenorientiert: JSON-Schema

## Abläufe

    - Aktivitätsdiagramme für relevante Use Cases
    - Aktivitätsdiagramm für den Ablauf sämtlicher Use Cases

## Entwurf

    - Detaillierte UML-Diagramme für relevante Softwarebausteine

# __Projektorganisation__

## Annahmen

    - Nicht durch den Kunden definierte spezifische Annahmen, Anforderungen und Abhängigkeiten
    - Verwendete Technologien (Programmiersprache, Frameworks, etc.)
    - Aufteilung in Git-Repositories gemäß Software- und Systemarchitektur und Softwarebbausteinen 
    - Einschränkungen, Betriebsbedingungen und Faktoren, die die Entwicklung beeinflussen (Betriebssysteme, Entwicklungsumgebung)
    - Interne Qualitätsanforderungen (z.B. Softwarequalitätsmerkmale wie z.B. Erweiterbarkeit)

## Verantwortlichkeiten

    - Zuordnung von Personen zu Softwarebausteinen aus Kapitel 3.1 und 3.2
    - Rollendefinition und Zuordnung

| Softwarebaustein | Person(en)        |
|:-----------------|:------------------|
| Komponente A     | Thomas Mustermann |

### Rollen

#### Softwarearchitekt

Entwirft den Aufbau von Softwaresystemen und trifft Entscheidungen über
das Zusammenspiel der Softwarebausteine.

#### Frontend-Entwickler

Entwickelt graphische oder andere Benutzerschnittstellen, insbesondere
das Layout einer Anwendung.

#### Backend-Entwickler

Implementiert die funktionale Logik der Anwendung. Hierbei werden zudem
diverse Datenquellen und externe Dienste integriert und für die
Anwendung bereitgestellt.

### Rollenzuordnung

| Name              | Rolle             |
|:------------------|:------------------|
| Thomas Mustermann | Softwarearchitekt |


## Grober Projektplan

    - Meilensteine

### Meilensteine

* KW 43 (21.10)
  * Abgabe Pflichtenheft
* KW 44 (28.10) / Projekt aufsetzen
  * Repository Struktur
* KW 45 (4.11) / Implementierung
  * Implementierung #3 (Final)
* KW 48 (18.12) / Abnahmetests
  * manuelle Abnahmetestss
  * Pr�sentation / Software-Demo

# __Anhänge__

## Glossar

    - Definitionen, Abkärzungen, Begriffe

## Referenzen

    - Handbücher, Gesetze

## Index

