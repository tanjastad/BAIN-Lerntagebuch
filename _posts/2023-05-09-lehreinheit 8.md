---
title: "Lehreinheit 8"
date: 2023-05-09
---

## Metadaten modellieren und Schnittstellen nutzen

Orientiert man sich am Schaubild der ersten Unterrichtseinheit, befinden wir uns in der heutigen Lehreinheit im gelb markierten Bereich: 

![Schaubild Zwischenstand](https://github.com/tanjastad/BAIN-Lerntagebuch/assets/125452743/3ab949ff-d851-4353-955e-ae7c12b7b219)

Für das Verfassen des Lerntagebuchs musste ich mich zuerst nochmals genauer in die Thematik einlesen und mir eine kurze Definitionsübersicht der verschiedenen teilweise sehr ähnlichen Begriffen rund um Metadaten und Schnittstellen. Dafür habe ich mich am Handbuch IT in Bibliotheken orientiert. 
Datenformat: wie werden Daten strukturiert und dargestellt (Bedeutung durch Datenmodell)
2 Kategorien von Datenformaten:
* Strukturierungssprache: Daten in kleinere Pakete packen und so Beziehungen erstellen. Beispiele: JSON, CSV, XML, RDF
* Anwendungsformate: strukturiert Daten für spezifische Inhalte. Sind letzten Endes auch mit einer Strukturierungssprache codiert. Beispiel: Metadatenformate
Weitere Formate: 
* Schemasprachen: formale Beschreibung der Syntax (Struktur der Daten)
* Abfragesprachen: für Verweise innerhalb der Datensätze
* Modellierungssprachen: beschreiben die Datenmodelle, meist mit ERM-Modellen (Entity Relationship-Modell)
Metadatenformat: Gehört zur Unterklasse Anwendungsformat. Ermöglicht es, Dokumente zu beschreiben. Für digitale Objekte und Forschungsdaten gibt es spezifischere Formate. 
* Bibliothekarische Metadatenformate
  *  Machine-Readable Cataloging (MARC). Die aktuellste Version ist MARC21 und dient zum Austausch von Daten zwischen Bibliotheken. 
  *  PICA. Datenformat von zwei spezifischen Bibliothekssystemen
  *  MAB und allgero: werden nur noch sporadisch verwendet. 
* Datenmodelle und RDF-Formate
  * Dublin Core: Metadatenstandard mit einer der grössten Verbreitungen
  * FRBR: abstraktes Metadatenmodell
  * BIBFRAME: soll in Zukunft MARC ablösen und wird auf der Grundlage von RDF aufgebaut

Um Daten von einem System in ein anderes zu übertragen, kommt meist ein ETL-Prozess zum Einsatz. Der Prozess besteht aus drei zentralen Schritten: Extract., Transform und Load
1)	Extraktion (extract): Daten werden ausgewählt und abgezogen. Dieser Vorgang nennt man auch Harvesting. Die Qualität der Harvesting-Daten ist unterschiedlich und ist abhängig von der Datenquelle. Es braucht lediglich ein strukturiertes Datenformat und eine Schnittstelle. Bei Bedarf kann dieser Extraktionsvorgang regelmässig gemacht werden. 
Beispiel aus der Lehreinheit: wir haben Metadaten über die OAI-PMH-Schnittstelle mit VuFindHarvest geharvestet. Sowohl Koha, ArchivesSpace als auch DSpace verfügen über diese Möglichkeit. 
2)	Transformation (transform): hat man die Daten erstmals abgezogen, liegen diese in unterschiedlichen Datenformaten mit verschiedenen Datenmodellen vor. Damit die Daten in ein gemeinsames Datenmodell überführt werden können, braucht es eine Vereinheitlichung der Formate (auch Schema genannt). Die Formatanpassung (Mapping) kann durch die Verwendung von gleichen Austauschformaten minimiert werden.
Mit einem Crosswalk können Daten von einem Metadatenformat in ein anderes konvertiert werden. Dabei gibt es gewisse Regeln für die Zuordnung von Elementen und Werten (Mapping). 
3)	Laden (load): die Daten werden ins Zielsystem überführt. Es dürfen nur Datensätze überführt werden, die zuvor transformiert wurden. 

OpenRefine ist ein Open-Source-ETL-Werkzeug und führt durch obengenannte Schritte. Es kann den Prozess ein Stück weit vereinfachen. 



