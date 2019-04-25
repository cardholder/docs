# Anforderungs- und Entwurfsspezifikation

__Autoren:__
* Marti Stuwe
* Patrick Reinke
* Stefan Kröker

__Inhaltsverzeichnis__
1. Einführung  
   1.1 Beschreibung  
   1.2 Ziele
2. Anforderung  
   2.1 Stakeholder  
   2.2 Funktionale Anforderungen  
   2.3 Nicht-funktionale Anforderungen  
   2.4 Graphische Benutzerschnittstelle  
   2.5 Anforderungen im Detail
3. Technische Beschreibung  
   3.1 Systemübersicht  
   3.2 Softwarearchitektur  
   3.3 Schnittstellen  
   3.4 Datenmodell  
   3.5 Abläufe  
   3.6 Entwurf
4. Projektorganisation  
   4.1 Annahmen  
   4.2 Verantwortlichkeiten  
   4.3 Grober Projektplan
5. Anhänge  
   5.1 Glossar  
   5.2 Referenzen  
   5.3 Index
  
 

# 1 Einführung

## 1.1 Beschreibung

__Projektname:__ Cardholder 
  
Cardholder ist eine Applikation, die es ermöglicht online Kartenspiele zu spielen. Dabei kann man mit Freunden und Menschen aus aller Welt spielen. Es gibt eine Auswahl von verschiedenen Kartenspielen. Die Nutzer können die Kartenspiele ohne Anmeldung spielen. Spieler sollen andere Nutzer zu einem Spiel einladen können. Cardholder ist als App und als Webseite verfügbar.

## 1.2 Ziele

Das Ziel von Cardholder ist es, dass Familie, Freunde und Kartenspiel-Begeisterte zusammen Kartenspiele spielen können. Die Motivation ist eine freie und für jeden zugängliche Software bereitzustellen. Es werden verschiedene Kartenspiele zur Verfügung gestellt. 

Cardholder setzt vorraus, dass die Nutzer die entsprechenden Regeln der jeweiligen Kartenspiele kennen. Weitere Vorkenntnisse sind nicht erforderlich.  

Bei Cardholder ist es nicht möglich eigene Kartenspiele hinzuzufügen. Des Weiteren ist es nicht möglich seinen Spielstand zu speichern.

# 2 Anforderungen

## 2.1 Stakeholder

| Funktion | Name | Kontakt | Verfügbarkeit | Wissen  | Interesse & Ziele  | Relevanz  |
|---|---|---|---|---|---|---|
|  |   |   |   |   |   |   |


### Beispiel

| Funktion | Name | Kontakt | Verfügbarkeit | Wissen  | Interesse & Ziele  | Relevanz  |
|---|---|---|---|---|---|---|
| Leiter der Bibliothek  |  Herr Bauer | Tel. 409000  | Von 9-19 Uhr telefonisch erreichbar, Mitarbeit zu 30% möglich, Nürnberg  | Kennt das Altsystem aus der Anwendersicht, soll mit dem System arbeiten  | Vereinfachung der Ausleihprozesse  | Fachlicher Entscheider  |
| Administrator  | Herr Heiner  | Heiner@gmx.net  | Per E-Mail, immer erreichbar, Verfügbarkeit 50%, Nürnberg  | Vertraut mit vergleichbarer Verwaltungssoftware   |  Stabiles System, geringer Wartungsaufwand | Informationslieferant bzgl. Wartungsanforderungen  |
| Product-Owner  | Paul Ottmer  |  po@ottmer.de | Per E-Mail und tel. tagsüber, Verfügbarkeit 100%, Nürnberg  | Koordinator für die Inputs der Stakeholder  | ROI des Systems sicherstellen  | Entscheider - als Koordinator der Stakeholderanforderungen  |

## 2.2 Funktionale Anforderungen
    - Use-Case Diagramme
    - Strukturierung der Diagramme in funktionale Gruppen

## 2.3 Nicht-funktionale Anforderungen 

### 2.3.1 Rahmenbedingungen
    - Normen, Standards, Protokolle, Hardware, externe Vorgaben

### 2.3.2 Betriebsbedingungen
    - Vorgaben des Kunden (z.B. Web Browser / Betriebssystem Versionen, Programmiersprache)

### 2.3.3 Qualitätsmerkmale
    - Externe Qualitätsanforderungen (z.B. Performance, Sicherheit, Zuverlässigkeit, Benutzerfreundlichkeit)

Qualitätsmerkmal | sehr gut | gut | normal | nicht relevant
---|---|---|---|---
**Zuverlüssigkeit** | | | | |
Fehlertoleranz |X|-|-|-|
Wiederherstellbarkeit |X|-|-|-|
Ordnungsmäßigkeit |X|-|-|-|
Richtigkeit |X|-|-|-|
Konformität |-|X|-|-|
**Benutzerfreundlichkeit** | | | | |
Installierbarkeit |-|-|X|-|
Verständlichkeit |X|-|-|-|
Erlernbarkeit |-|X|-|-|
Bedienbarkeit |-|X|-|-|
**Performance** | | | | |
Zeitverhalten |-|-|X|-|
Effizienz|-|-|-|X|
**Sicherheit** | | | | |
Analysierbarkeit |X|-|-|-|
Modifizierbarkeit |-|-|-|X|
Stabilität |X|-|-|-|
Prüfbarkeit |X|-|-|-|

## 2.4 Graphische Benutzerschnittstelle
    - GUI-Mockups passend zu User Stories
    - Screens mit Überschrift kennzeichnen, die im Inhaltsverzeichnis zu sehen ist
    - Unter den Screens darstellen (bzw. verlinken), welche User Stories mit dem Screen abgehandelt werden
    - Modellierung der Navigation zwischen den Screens der GUI-Mockups als Zustandsdiagramm

## 2.5 Anforderungen im Detail
    - User Stories mit Akzeptanzkritierien 
    - Optional: Name (oder ID) und Priorität ("Must", "Should", "Could", "Won't")
    - Strukturierung der User Stories in funktionale Gruppen

### Schablone für User Stories

| **Als** | **möchte ich** | **so dass** | **Akzeptanz** |
| :------ | :----- | :------ | :-------- |
| Wer | Was | Warum | Wann akzeptiert |

### Beispiel 1

| **Als** | **möchte ich** | **so dass** | **Akzeptanz** |
| :------ | :----- | :------ | :-------- |
| Benutzer | bei Fehleingabe die Lösung angezeigt bekommen | ich lernen kann | Lösung wird angezeigt |

### Beispiel 2

| **Name**| **In meiner Rolle als**...|   ...**möchte ich**...   | ..., **so dass**... | **Erf�llt, wenn**... | **Priorit�t**   |
|:-----|:----------:|:-------------------|:-------------|:---------|:----------------|
| Lernen  |Benutzer| bei Fehleingabe die Lösung angezeigt bekommen|ich lernen kann| Lösung wird angezeigt | Muss |


# 3 Technische Beschreibung

## 3.1 Systemübersicht
    - Systemarchitekturdiagramm ("Box-And-Arrow" Diagramm)
    - Kommunikationsprotokolle, Datenformate

## 3.2 Softwarearchitektur
    - Darstellung von Softwarebausteinen (Module, Schichten, Komponenten)

## 3.3 Schnittstellen
    - Schnittstellenbeschreibung
    - Auflistung der nach außen sichtbaren Schnittstelle der Softwarebausteine

## 3.4 Datenmodell 
    - Konzeptionelles Analyseklassendiagramm (logische Darstellung der Konzepte der Anwendungsdom�ne)
    - Modellierung des physikalischen Datenmodells 
      - RDBMS: ER-Diagramm bzw. Dokumentenorientiert: JSON-Schema

## 3.5 Abläufe
    - Aktivitätsdiagramme für relevante Use Cases
    - Aktivitätsdiagramm für den Ablauf sämtlicher Use Cases

## 3.6 Entwurf
    - Detaillierte UML-Diagramme für relevante Softwarebausteine

# 4 Projektorganisation

## 4.1 Annahmen
    - Nicht durch den Kunden definierte spezifische Annahmen, Anforderungen und Abhängigkeiten
    - Verwendete Technologien (Programmiersprache, Frameworks, etc.)
    - Aufteilung in Git-Repositories gemäß Software- und Systemarchitektur und Softwarebbausteinen 
    - Einschränkungen, Betriebsbedingungen und Faktoren, die die Entwicklung beeinflussen (Betriebssysteme, Entwicklungsumgebung)
    - Interne Qualitätsanforderungen (z.B. Softwarequalitätsmerkmale wie z.B. Erweiterbarkeit)

## 4.2 Verantwortlichkeiten
    - Zuordnung von Personen zu Softwarebausteinen aus Kapitel 3.1 und 3.2
    - Rollendefinition und Zuordnung

| Softwarebaustein | Person(en) |
|----------|-----------|
| Komponente A | Thomas Mustermann |

### Rollen

#### Softwarearchitekt
Entwirft den Aufbau von Softwaresystemen und trifft Entscheidungen über das Zusammenspiel der Softwarebausteine.

#### Frontend-Entwickler
Entwickelt graphische oder andere Benutzerschnittstellen, insbesondere das Layout einer Anwendung.

#### Backend-Entwickler
Implementiert die funktionale Logik der Anwendung. Hierbei werden zudem diverse Datenquellen und externe Dienste integriert und für die Anwendung bereitgestellt.

### Rollenzuordnung

| Name     | Rolle     |
|----------|-----------|
| Thomas Mustermann | Softwarearchitekt |


## 4.3 Grober Projektplan
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

# 5 Anhänge

## 5.1 Glossar 
    - Definitionen, Abkärzungen, Begriffe

## 5.2 Referenzen
    - Handbücher, Gesetze

## 5.3 Index



