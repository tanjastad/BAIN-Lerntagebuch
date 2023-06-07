---
title: "Lehreinheit 5"
date: 2023-04-04
---

## Funktion und Aufbau von Bibliothekssystemen, Teil 2

In der Woche vor der BAIN-Vorlesung besuchte ich einen Sketchnote-Kurs der Fachhochschule Graubünden. Um das Gelernte gleich praktisch anzuwenden, verfasste ich die Notizen während der Einheit auf diese Weise. Hier ist das Resultat:

![Sketchnote](https://user-images.githubusercontent.com/125452743/232825282-01599de4-e684-4270-b893-907d96a3e970.png)

Zu Beginn der Einheit befassten wir uns gleich wieder praktisch mit dem Bibliothekssystem Koha. In der bibliothekarischen Praxis wird mit RDA kaum noch selbständig katalogisiert. Man importiert die Daten von einer Institution und passt lediglich gravierende Fehler und bibliotheksinterne Eintragungen an. Die Vorteile sind die Arbeitserleichterung, eine geringere Fehleranfälligkeit und man kann das Katalogisat einmal in aller Ruhe machen, ohne gestresst zu sein. Copy Cataloging ist auch mit Koha möglich. Dafür muss der Server Z39.50/SRU eingerichtet werden. SRU steht für Search/Retrieve via URL und ist der Nachfolger vom Z39.50-Protokoll. 
Ist diese Einstellung vorgenommen, kann unter der Katalogisierungsfunktion einen Import (copy cataloging) über die Funktion Z39.50/SRU vorgenommen werden. Der gesuchte Titel kann über verschiedene Suchfelder gefunden werden, danach überprüft man die Felder und muss den Medientyp und einen Barcode vergeben. 

Neben dem Import kann aber auch der Export für eine Bibliothek interessant und wichtig sein. Beispielsweise wenn die Daten für die Weiterverarbeitung gebraucht werden, wenn man Aggregationen ermöglichen möchte (Verbundrecherchen) oder eine Datenbereitstellung (beispielsweise für die Digitalisierung). Der Datenexport aus Koha ist über die OAI-PMH-Schnittstelle möglich. Ausgeschrieben bedeutet das "Open Archives Initiative Protocol for Metadata Harvesting". Das OAI-PMH wird uns auch noch in einer späteren Einheit beschäftigen. Während einer Übung war das Ziel, Testdatensätze zu katalogisieren oder zu importieren und danach die Schnittstelle nach dem entsprechenden Eintrag zu prüfen. Diese Übung war sehr tricky, ohne die Auflösung in der gemeinsamen Besprechung hätte ich den angelegten Eintrag nicht gefunden. Der Schlüssel zum Eintrag ist die Record Number in Koha. In der OAI-PMH-Schnittstelle muss die URL unter Record Details mit der Record Number ersetzt werden. Diese Übung bereitete mir doch ein wenig Kopfzerbrechen. In der Praxis sehe ich bis jetzt noch keinen konkreten Nutzen - trotz der genannten Beispiele. 

Sehr interessant fand ich den Marktüberblick der Bibliothessysteme. Dank den jährlichen Statistiken und Artikeln von Marshall Breeding zu den Library Technology Sales Statistics ist eine gute Marktübersicht der USA möglich. Marktführer ist Ex Libris mit seinem Bibliothekssystem Alma. Alma ist der Nachfolger von Aleph und hat den grossen Vorteil, dass das ERM (Electronic Resource Management) integriert ist. Bei Koha beispielsweise ist dies nicht möglich. Alma hat im Bereich der wissenschaftlichen Bibliotheken Konkurrenz von Folio (Open Resource) und WMS. Bei den öffentlichen Bibliotheken ist Axiell am "Durchstarten". 

Alma entwickelt sich leider mehr und mehr zu einer Marktmacht wie Elsevier (eBook-Pakete im Bereich der wissenschaftlichen Bibliotheken). Das Bibliothekssystem hat zwar viele Vorteile (vorbildliche Programmschnittstellen, regelmässige Updates sind nur einige wenige), trotzdem besteht die Gefahr, dass sie aufgrund ihrer Grösse und Macht das Interesse an Innovation verlieren und die Preise unfair gestalten könnte. Entscheidet man sich einmal für ein Bibliothekssystem, bleibt es meist bei dem. Wechsel im Nachhinein sind schwierig und teuer. Diesen Rat nehme ich gerne mit auf den Weg.  
