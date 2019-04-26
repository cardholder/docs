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

| Funktion      | Name                     | Kontakt                         | Verfügbarkeit | Wissen                                       | Interesse & Ziele                               | Relevanz    |
|:--------------|:-------------------------|:--------------------------------|:--------------|:---------------------------------------------|:------------------------------------------------|:------------|
| Spieler       | -                        | -                               | -             | Kennt die Regeln der jeweiligen Kartenspiele | Möchte mit Freunden online Kartenspiele spielen | Endnutzer   |
| Product-Owner | Prof. Dr. Jörg Brunsmann | joerg.brunsmann@fh-bielefeld.de | 24/7          | Vertraut mit Fullstack-Anwendungen           | Koordination                                    | Entscheider |

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

### User Stories

| **Als**  | **möchte ich**              | **so dass**                                                                                           | **Akzeptanz**                |
|:---------|:----------------------------|:------------------------------------------------------------------------------------------------------|:-----------------------------|
| Benutzer | Kartenspiele online spielen | ich in meiner Freizeit mit Freunden Kartenspiele spielen kann                                         | Spiel ist spielbar           |
| Benutzer | eine Lobby erstellen        | ich mit anderen Spieler spielen kann                                                                  | Andere können beitreten      |
| Benutzer | einer Lobby beitreten       | ich in meiner Freizeit mit Freunden und Fremden Kartenspiele spielen kann                             | Spiel ist spielbar           |
| Benutzer | meine Lobby einstellen      | ich die Spieleranzahl, Kartenspiel und ob es eine öffentliche oder private Lobby ist, einstellen kann | Lobby erstellen              |
| Benutzer | Freunde einladen            | ich mit meinen Freunden zusammen spiele können                                                        | Freund kann beitreten        |
| Benutzer | Andere Spieler entfernen    | ich als Lobby Leiter andere Spieler entfernen kann                                                    | Anderer Spieler ist entfernt |

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

