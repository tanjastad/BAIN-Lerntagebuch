---
title: "Lehreinheit 9"
date: 2023-05-16
---

## Suchmaschinen und Discovery Systeme
Um einen praktischen Einblick in Suchmaschinen und Discovery Systeme zu erhalten, arbeiteten wir in der Lehreinheit mit VuFind, einer reifen Software aus dem Bibliotheksbereich mit viel Dokumentation und Anleitungen. Dafür mussten zuerst gewisse Installationen und Konfigurationen vorgenommen werden. Zuletzt füllten wir diesem modernen Online Katalog noch Beispieldatensätze hinzu. 

### Funktion von Suchmaschinen am Beispiel von Solr
Solr ist die Basis für gewisse Systeme. VuFind beispielsweise basiert auf Solr und ist sozusagen die „Einstellung im Hintergrund“. Auch Ex Libris Primo (Discovery Systeme von Alma) basiert auf Solr. Schaut man sich nun noch den Unterschied von Solr zu MySQL an, fallen gewisse Unterschiede auf. Solr ist nicht als Datenspeicher gedacht, sondern als Suchmaschine. Die Daten sind statisch, wohingegen sie bei MySQL verändert werden können. Die Funktion Retrieval (Solr) gegen die Funktion Storage (MySQL). 

Spricht man von Suchmaschinen müssen wir auch die Unterscheidung zwischen horizontaler und vertikaler Suchmaschine machen. Bei der horizontalen Suchmaschine geschieht die Suche unspezifisch über ungleichartige Bestände. Dafür braucht es kein Schema und Feldsuchen sind meist nicht möglich. Beispiele hierfür sind Internet- oder Volltextsuchen. Bei der vertikalen Suchmaschine hingegen sind die Daten zwar einheitlicher und die Suche geschieht datenmodell-orientiert. Auch braucht es ein Datenschema und Beispiele dafür können Bibliothekskataloge und Online Shops sein.
In einer praktischen Gruppenübung ergründeten wir die Unterschiede der Suche in VuFind und der von Solr. Solr hat in dem Sinne keine grafische Benutzeroberfläche, weshalb es für Laiensucherinnen und -sucher eher ungeeignet ist. Trotzdem gibt Solr in der Ergebnisliste eigentlich mehr Information her als VuFind. 

### VuFind Ranking und Autovervollständigung
Das Rankingprinzip von VuFind fand ich persönlich sehr interessant. In einem Modul am Anfang unseres Studiums schauten wir bereits einmal das komplizierte Ranking von Google an. Nun wurden uns die Gewichtungsfaktoren einer weiteren Suchmaschine vorgestellt. 

![grafik](https://github.com/tanjastad/BAIN-Lerntagebuch/assets/125452743/f983eba0-f0f3-40a3-a53f-06f34d746e05)

In der Abbildung sieht man die verschiedenen Bezeichnungen und der jeweilige Gewichtungsfaktor dazu. Beispielsweise hat der volle Titel ohne Feldbezug den Gewichtungsfaktor 600 oder ein ganzer Titel 400. Diese Gewichtungsfaktoren entscheiden schlussendlich über die Positionierung im Trefferfeld. VuFind hat dieses Ranking nach 15 Jahren Entwicklungsarbeit veröffentlicht. 
Wenn man beim VuFind eine Suchanfrage eintippt, wird diese Suchanfrage im Hintergrund abgeschickt und gewisse Treffer bereits angezeigt. So entsteht ein Live-Erlebnis für die Autovervollständigung. Damit der Server nicht überlastet wird, baut man im Hintergrund jeweils einen Verzögerungszeitpunkt für die Suchanfrage ein. 

### Schaubild
Zum Schluss möchte ich das heutige Thema im Schaubild Revue passieren lassen. Wir befinden uns ganz am Ende des Prozesses. Auf dem Testserver läuft in der Regel VuFind und im Hintergrund davon ein Solr. Wenn man Daten in VuFind ausgeben möchte, müssen diese Daten zuvor in Solr eingespeist werden. MARC Daten werden mit einem Skript an Solr geschickt. 
