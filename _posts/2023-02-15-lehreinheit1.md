---
title: "Lehreinheit 1"
date: 2023-02-15
---

#### Teil 1, Vormittag
Die Blockwoche in unser letztes Semester an der Fachhochschule Graubünden startete mit dem Modul Bibliotheks- und Archivinformatik. Zuerst wurden alle organisatorischen Fragen geklärt. Dies umfasste vor allem die Durchführung und Form des Leistungsnachweises. Der Leistungsnachweis wird in Form eines Lerntagebuchs abgelegt. Für dieses Tagebuch schreibt man nach jeder Unterrichtseinheit einen Bericht. Zudem wird ein separater Artikel mit dem Wissensstand vor und nach dem Modul geschrieben sowie zu spezifischen Übungen. Mit dieser Form des Leistungsnachweises kann ich mich sehr gut anfreunden. So kann man regelmässig und im bereits im Voraus an der Prüfungsleistung arbeiten und muss nicht alles während der Prüfungs- und Abgabezeit erledigen. Der Abgabetermin für die Lerntagebücher wird am 30. Juni sein, was ich als sehr fair betrachte. 

Die Lehrmaterialien sind in diesem Kurs etwas anders, als ich dies bis anhin im Studium erlebt habe. Meist wurden uns PowerPoint-Folien per PDF zur Verfügung gestellt. In BAIN gab es auf Moodle einen Link zum „Gemeinsamen Dokument“. Dieses Internetdokument HedgeDoc kann von allen Studierenden bearbeitet werden und bildet nun die Grundlage für die Lehrveranstaltung. Bis anhin hatte ich noch nie mit einem HedgeDoc zu tun, es war für mich Neuland. Die Bedienung scheint mir aber sehr logisch zu sein. Als nächsten Programmpunkt fand die Vorstellung der Dozenten statt. Felix Lohmeier als Hauptdozent und seine allfällige Stellvertretung Sebastian Meyer. Auch die Studierenden durften sich vorstellen. Dabei standen die Fragen nach bisherigen Erfahrungen mit Bibliotheks- und Archivsoftware sowie die Motivation und allfällige Erwartungen im Vordergrund. 

Nach der Vorstellungsrunde fing nun die eigentliche Einführung ins Thema an. Das untenstehende Schaubild zeigte die Lehrinhalte des Moduls auf. 
![Schaubild zu Lehrinhalten](https://pad.gwdg.de/uploads/c8d2a2dc-b427-4330-a665-b355a2a85f50.png)
Folgende Dinge wurde uns zum Schaubild erklärt:
-	Koha: ist die Open Source Software im Bereich Bibliothekswesen
-	ArchiveSpace: ist die Open Source Software für den Bereich Archiv
-	DSpace: ist das Repository für Onlinedokumente (Publikationsdaten)
  -  OAI-PMH: nutzen wir als Schnittstelle (wie zieht man die Daten aus der Software)
    -  VuFindHarvest (OAI Harvester): Software, um die Daten über OAI-PMH zu beziehen (Harvesting = Ernten)
    - Software VuFindHarvest via Schnittstelle OAI Harvester aus einer Software beziehen
    - VuFind: gemeinsame Nutzung in einem Suchindex
      - 3 verschiedene XML-Dateien (MARC21-XML, EAD, Dublin Core) = Metadatenformate für die verschiedenen Teilgebiete
        - Crosswalks:
        - marcEdit (XSLT): vorhandene Crosswalks verwenden mit dieser Software
        - Vereinheitlichung in MARC-21-XML
-	Tabellendaten bearbeiten und einspeisen (OpenRefine)

Damit wir das HedgeDoc und auch allenfalls GitHub für unser Lerntagebuch bearbeiten können, lernten wir die wichtigsten Formatierungsmöglichkeiten von Markdown in einem spielerischen Tutorial mit entsprechenden Übungen. Die Funktionen wendeten wir gleich im HedgeDoc an, in dem wir unsere Namen/Synonyme in eine vorgefertigte Liste eintrugen. Herr Lohmeier bat uns ausserdem, ein Konto bei GitHub zu eröffnen. Zuerst dachte ich, ich hätte bereits ein Konto aus einem anderen Kurs. Es stellte sich jedoch heraus, dass dies GitLab war, weshalb ich dies nachholte. Damit wir zukünftige Übungen auf der gleichen Grundlage für alle lösen können, eignet sich die GitHub Codespace. Die Einrichtung dieser wollte zuerst nicht klappen, mit dem Verwenden eines anderen Browsers konnte das Problem dann aber behoben werden. Die Eingaben im GitHub Codespace erfolgen durch die Unix Shell. Mit dieser hatten wir zuletzt im Modul ARIS zu tun (siehe auch [Einführungsartikel](<https://tanjastad.github.io/BAIN-Lerntagebuch/2023/02/15/einfuehrung.html>)). Deshalb war das Kapitel 2 und 3 im Library Carpentry zur Unix Shell eine sehr gute Wiederholung und Auffrischung. Gewisse Befehle kamen einem durch die Lesson schnell wieder in den Sinn. Nach Abschluss dieser Kapitel gab es eine wohlverdiente Mittagspause. 

---

#### Teil 2, Nachmittag

Nach der Pause trug der Dozent noch einige Tipps zur Unix Shell vor. Ausserdem wurde auf die Wichtigkeit der Unix Shell aufmerksam gemacht. Wenn man Open Source Programme in Bibliotheken und Archiven nutzen möchte, kommt man um diese Eingabemöglichkeit nicht drum herum. Die Textbasierte Suche ist zudem extrem schnell. 
Gewisse Befehle habe ich mir während der Vorlesung notiert: 
-	clear = Bildschirm löschen
-	ctrl + C = stopp
-	head + Dateiname = die ersten 10 Zeilen einer Datei anzeigen
-	wc + Dateiname = word count
    - 1. Anzahl: Zeilen
    - 2. Anzahl: Wörter
    - 3. Anzahl: Zeichen
-	wc + -l + *.tsv = Anzahl Wörter ausgeben, von allen Dateien mit Endung
-	grep 1999 *.tsv = alle Dateien nach der Zeichenkette 1999 durchsuchen
-	grep -c revolution *.tsv = Zählung mit allen Treffern der Zeichenkette Revolution

Die Philosophie von Linux ist, dass jedes kleine Programm (beispielsweise wc (word count)) eine Sache sehr gut kann. Möchte man mehrere Dinge erreichen, können alle diese Programme miteinander kombiniert werden. 

Nachdem wir die Shell fürs Erste ruhen liessen, kam Git zur Sprache. Was ich nicht wusste, ist, dass Git eine Software ist und GitHub (sowie auch GitLab) diese Software „nur“ brauchen. Die Zusammenarbeit an einer gemeinsamen Textdatei auf mehreren Rechnern wird dadurch ermöglicht. Jede/r kann bei GitHub Änderungen und Bearbeitungen an Code vornehmen. Diese Änderungen kann man „nur“ lokal abspeichern und weiternutzen oder dem Ersteller als pull request zukommen lassen. Darin sind die entsprechenden Änderungen aufgeführt und Kommentare können angeführt werden. Der ursprüngliche Ersteller des Codes kann selber entscheiden, ob er die Änderungen akzeptiert und annimmt oder diese ignoriert. Der grosse Vorteil des Programms ist die Nachvollziehbarkeit, die durch dieses pull-request-System entsteht. GitHub ist die bekannteste Plattform in diesem Bereich. 2018 wurde sie von Microsoft aufgekauft, trotzdem blieben die meisten Dienstleistungen kostenlos. Meist werden Open-Source-Projekte auf dieser Plattform abgelegt. Die bekannteste Alternative ist wohl GitLab. Erstaunt hat mich, dass sehr viele Bibliotheken auch selber Code anlegen und diese auf GitHub oder GitLab veröffentlichen. Es gibt gewisse Listen mit Repositorien, wo was von wem abgelegt wurde. 

Um die grundlegenden Funktionen von Git kennenzulernen, führten wir eine gemeinsame Übung durch. Dabei musste ein Repository angelegt werden und darin etwas platzieren. Auch ein Fork musste erstellt werden, damit danach eine Änderung vorgenommen werden konnte. Diese Änderung kommentierte man und stellte es via Pull-Request zu. 

Die Unterrichtseinheit war 1.5h früher fertig als geplant. Das war aber nicht so schlimm, da wir uns so bereits Gedanken über das Lerntagebuch machen konnten. Dies war nämlich die Aufgabe aufs nächste Mal. Ein Lerntagebuch erstellen und die ersten drei Berichte dazu schreiben. Die freie Zeit nutzte ich, um mich bei den Mitstudierenden über die Programmwahl für das Lerntagebuch zu erkunden. Eine Kollegin aus dem gleichen Semester, welche den Kurs aber bereits vorgeholt hat, meinte GitHub sei sehr gut machbar. Einzig die Einrichtung sei etwas schwierig. Dies stimmte mich zuversichtlich, dass die vom Dozenten vorgeschlagene Programmwahl eine gute ist. 
