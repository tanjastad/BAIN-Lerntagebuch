---
title: "Lehreinheit 10"
date: 2023-05-30
---

## Aktuelle Datenmodelle für Metadaten
Es gibt aktuell zwei Datenmodelle für Metadaten, die aufgrund ihrer Aktualität und Wichtigkeit herausragen. Beide Modelle werden nachfolgend kurz vorgestellt. 
### BIBFRAME
BIBFRAME wird seit 2012 entwickelt und gilt als Nachfolger von MARC21. Es basiert auf dem bekannten FRBR-Modell (Functional Requirements for Bibliographic Records) und dem Regelwerk RDA (Resource Description and Access). Darüber hinaus folgt es dem Linked Data Paradigma. BIBFRAME unterteilt die Daten in Werk, Instanz und Exemplar und definiert drei verschiedene Entitäten (ähnlich aber einfacher als das FRBR-Modell). BIBFRAME ist ein richtiges Datenmodell, was eine Suche darin interessanter macht (entdeckende Suche). 

#### Vor- und Nachteile

| BIBFRAME | MARC(XML/21) | 
| -------- | -------- |
| **Vorteile** | **Vorteile** |
| Katalogisierung von grossen Beständen in guter Qualität | flexibel und leicht erweiterbar |
| keine Kostensteigerung | dient als Validierungsinstrument |
| ermöglicht eine Vernetzung der Datensätze | verlustfreie Umwandlung innnerhalb des MARC-Standards
| Identifikation von Entitäten und Anlegen von Beziehungen 
| (Quelle: https://blog.fhgr.ch/dis/von-marc-zu-bibframe-die-bibliographic-framework-transition-initiative-der-library-of-congress/)* | *(Quelle: https://wiki.deutsche-digitale-bibliothek.de/pages/viewpage.action?pageId=78513053)* |
| **Nachteile** | **Nachteile** |
| FRBR wird noch nicht vollständig abgedeckt | MARCXML ist für den Menschen nicht gut lesbar
| andere Verwendung der Vokabulare (FRBR und RDA)
| *(Quelle: http://www.payer.de/dbaufbau/dbauf07.html)* | *(Quelle: https://silo.tips/download/datenaustauschprozesse-zwischen-bibliotheken-im-deutschsprachigen-raum-vor-dem-u)*
   

### Records in Contexts (RiC)
RiC basiert ebenfalls auf den Linked-Data-Prinzipien und ermöglicht neue und mehrfache Beziehungen zwischen den Entitäten. Aktuell ist man an einer Ausarbeitung einer Schweizer Version des Standards dran. RiC wäre ein neuer archivischer Verzeichnungsstandard, der die vier bisherigen Standards ICA-Standards ISAD(G), ISAAR(CPF), ISDF und ISDIAH ablösen soll. 


| RiC | ICA-Standard | 
| -------- | -------- |
| **Vorteile** | **Vorteile** |
| ermöglicht flexible Beziehungsnetze | Verwaltung und Recherche von Informationen zu den logischen Einheiten von Archivgut über Verzeichnungselemente |
| verknüpfbare Metadaten | garantieren die Zuverlässigkeit und Authentizität der Unterlagen gegenüber dem Nutzer |
| plurale Verknüpfung zwischen Entitäten | garantiert die Zuverlässigkeit und Authentizität gegenüber dem Urheber/Aktenbildner selbst |
| Metadaten verknüpfen und abbilden | flexibel einsetzbare archivische Instrumentarien |
| (Quelle: https://arbido.ch/de/ausgaben-artikel/2017/metadaten-datenqualit%C3%A4t/records-in-contexts-vom-baum-zum-netz* | *(Quelle: https://de.wikipedia.org/wiki/ISAD(G))* |
| **Nachteile** | **Nachteile** |
| Vor allem bei den externen Verlinkungen und der Metadaten-Provenienz stehen die Anwendungen eher am Anfang | ermöglicht nur eine Zuteilung der Ressource |
| fehlenden Tiefe der Verzeichniselemente | 26 Verzeichnungselemente reichen meist nicht aus |
|keine Möglichkeit für Benutzung bereits bestehender Ontologien| nicht maschinenlesbar |
| *(Quelle: https://bop.unibe.ch/iw/article/view/7083/9936)* | *(Quelle: https://bop.unibe.ch/iw/article/view/7083/9936* |
   

### Metadaten anreichern mit Open Refine und Wikidata
In dieser spannenden Übung wurde wieder mit dem Tool Open Refine gearbeitet. Dabei ging es darum, Daten in Open Refine einzuspeisen und den Abgleich (Reconcile) zu machen. Dies ist über den Namen möglich (sinnvoll, da dieser in Wikidata als erstes gesucht wird) oder aber auch über das Geburtsjahr. Dies kann beispielsweise hinzugezogen werden, wenn der Name allein nicht für eine automatische Zuordnung reicht (lediglich 53% konnten nur durch den Namen zugeordnet werden). Mit dem zusätzlichen Geburtsjahr funktioniert es zu 100%. Die eingespeisten Daten konnten durch Wikidata angereichert werden. So haben wir eine neue Spalte mit dem Namen wikidata eingefügt und darin die „Award received“ eingespeist und aufgeführt. 
