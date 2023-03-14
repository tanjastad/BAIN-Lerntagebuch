---
title: "Lehreinheit 4"
date: 2023-03-07
---

#### Funktion und Aufbau von Bibliothekssystemen, Teil 1

##### Metadatenstandards in Bibliotheken (MARC21)
Damit wir die Funktion und den Aufbau von Bibliothekssystemen verstehen, braucht es zuerst eine Einführung in den Metadatenstandard. In Bibliotheken ist der Standard MARC21 (Machine Readable Cataloging) in Gebrauch. Die Zahl 21 steht dabei für das 21. Jahrhundert. Der Metadatenstandard sollte nicht mit dem Dateiformat verwechselt werden. Mit Metadatenstandard ist eine getroffene Verabredung gemeint, während das Dateiformat die technische Ausprägung beschreibt, die die Daten Computer-lesbar machen. 
Um MARC21-Dateien zu lesen, braucht es eine spezielle Software wegen des eigenen Binärformats. Als Alternative ist aber auch ein XML-Format möglich, so können die Daten mit einem beliebigen Editor oder einer Programmiersprache bearbeitet werden. In MARC21 gibt es verschiedene Datenfelder mit der genauen Feldbezeichnung (numerisch). Die meisten Bibliothekssysteme unterstützen MARC21 als Austauschformat. Voraussichtlich wird das Format aber in naher Zukunft (ca. 20 Jahre) von BIBFRAME abgelöst. Dieses Format basiert auf RDF und die Zukunft soll ein semantisches System/eine Ontologie ermöglichen.
![Modell Bibframe](https://www.loc.gov/bibframe/docs/images/bf2-model.jpg)
Obenstehendes Modell zeigt die in RDF erfassten Ebenen. Auf der obersten Ebene das Werk, das eigentlich nur die Idee eines Verfassers darstellt (intellektueller Oberbegriff). Diese Ebene kann mit Subjekten, Vertretern und Veranstaltungen verknüpft werden. Das Werk hat verschiedene Instanzen oder Manifestationen. Das können verschiedene Formate oder Herausgeber sein. Schlussendlich auf der untersten Ebene steht das Exemplar. Das kann gehalten werden durch eine Bibliothek (3 Exemplare) und mit einem Barcode versehen. 
Durch Bibframe erhofft man sich gute Normierungschancen, die mit MARC21 verloren gehen. Personeninformation sollen durch Datenmodelle besser erfasst werden. 
Als Übung verglichen wir MARC21 mit Dublin Core. Für Laien oder Personen ohne Vorkenntnisse ist Dublin Core viel verständlicher und einfacher in der Handhabung. MARC21 ist ohne das Wissen über die Felderbezeichnung schwierig zu verstehen. Hingegen gibt es mit diesem Metadatenstandard mehr Angaben als mit Dublin Core. 


##### Koha
Koha ist eine Open Source Software für den Bibliotheksbereich. Sie ist weit verbreitet und gibt es bereits seit 1999. Regelmässig werden grössere Updates geschalten und sie zeichnet sich durch eine sehr aktive Community aus. Die Open Source Software ist durch eine GPL Lizenz vor kommerzieller Weitergabe durch einen indirekten Rechtstrick geschützt. 
Im Internet gibt es ein gutes Tutorial für den ersten Einstieg in Koha. Dieses wurde von Herrn Lohmeier vorgestellt. Danach konnte eine Übung zur manuellen Bedienung gemacht werden. Ziel war es untenstehende Aufgaben in Koha zu lösen:
* Buch erfassen
* Benutzer anlegen
* Buch an Theke ausleihen
* Buch an Theke zurücknehmen

Ich war erstaunt, wie gut und durchdacht Koha war. Ich arbeite seit einigen Jahren mit der Software winMedio von Predata. Die Qualität von Koha schätzte ich auf den ersten Blick sehr hoch ein und kommt den kommerziellen Produkten, die ich kenne, sehr nahe. In winMedio sind die MARC21-Felder hinter den "Beschreibungsfeldern" versteckt. Deshalb kenne ich noch nicht alle Felder auswendig. Trotzdem hat man sich sehr schnell in den verschiedenen Modulen zurechtgefunden. Ich bin gespannt auf die nächste Lehreinheit mit Koha. 
