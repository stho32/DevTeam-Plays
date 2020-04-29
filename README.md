# DevTeam-Plays
Unterschiedliche Strategien für Softwarentwicklerteams

In Computerspielen gibt es unterschiedlichste Strategien. Was wäre, wenn man die auf Softwareentwicklerteams denken würde?

Strategien: Rushen, Einigeln, Expansion, Dampfwalze

Taktiken: Scouten, Hinterhalt, Angriff, Guerillia-Angriff

## Entwickler

### Strategien

#### Rushen
  - schnelle Erstellung der notwendigen Funktionalität
  - nicht auf Schönheit oder Langlebigkeit achten
  - "billige, schnelle Lösungen", sie sind vielleicht nicht state-of-the-art oder mit Top-Entwicklungen vergleichbar, aber bringen einen zügig implementierten Brückenkopf zustande
  - z.B. "StackOverflow-Kopieren ohne (viel) Validierung", einfache Anwendungsmodelle (Konsolenanwendung mit geplantem Task statt Dienst)
  - kann beim ersten Anzeichen von Widerstand zusammenbrechen
  - sorgt dafür, dass man viele viele billige Anwendungen hat. Ein technologischer Umschwung (Widerstand) kann einen Haufen Arbeit auslösen, weil man dann viele unabhängige Anpassungen durchführen muss.
  - Wozu Logs?
  - Einfach mal schnell auf der Datenbank machen!
  
### Einigeln
  - Vor allem auf Solidität setzen
  - Dienste als Bus-System oder asynchron aufstellen; Wert auf die Fähigkeit der Systeme zur Selbstheilung legen
  - Transaktionen
  - Solidität vor Performance, der Benutzer braucht vielleicht 5 Minuten für den Mausklick im Browser, aber wenn er dabei keine Fehlermeldung erhält, hat es funktioniert.
  - Logs
  - interne Support-Tools
  - Monitoring
  - Reporting auf Vorgesetztenberuhigung ausrichten
  - Refactoring durchführen um sich und/oder die Software abzusichern
  - Security-Tests

#### Expansion
  - Die Software wird mit Blick auf "weitere Vorteile, die später mal benötigt werden könnten" implementiert
  - Offene Schnittstellen
  - Geteilte Bibliotheken erstellen

#### Dampfwalze
  - Die Änderungen werden schneller in die Produktion gegeben, als diese sich anpassen kann.
  - Die Änderungen werden direkt und kontinuierlich aus der Entwicklung live in die Produktion gegeben, mehrfach am Tag.
  - Die Entwicklung achtet nicht darauf, dass Produktion sich anpassen kann, sondern pumpt einfach Änderungen in die Produktion, bis diese zusammenbricht.
  - Geschwindigkeit der Entwicklungen spielt eine entscheidende Rolle
  - Jedes Update fügt mindestens einen neuen Bug ein. Bugs werden fließend gefixt, tauchen aber andersartig an anderen Stellen auf, so dass sich Produktion ständig auf andere Probleme einstellen muss (könnte auch Guerilla sein)

#### Aufrüsten
  - Einführung neuer Technologien und Hardware zur Problemlösung
  - Führt bei Unbedachtheit zu "Totrüsten"

#### Zentralisieren
  - Funktionalitäten in einer größeren Anwendung zusammenziehen
  - "Single point of failure"

#### Dezentralisieren
  - Funktionalitäten verteilen
  - vielleicht stabiler, aber schwierigere Übersicht
  - weniger zentrale Kontrolle

### Taktiken

#### Scouten
  - sich umhören, was als nächstes kommt
  - Kontakt zu Arbeitskollegen suchen
  - Beobachten, wie die Software verwendet wird
  - Geschäftsführern zuhören, welche Visionen oder Unternehmenswandlungen anstehen

#### Hinterhalt
  - ?? Entwicklung ohne Berücksichtigung des Geschäftszwecks
  - Die Kommunikation findet erst ganz am Ende der Entwicklung statt, wenn die Software letztlich eingesetzt werden soll?
  
#### Angriff
  - Zusammenstellung einer Reihe von abgeschlossenen Aufgaben in unterschiedlichen Projekten
  - Man läuft damit zum Arbeitsplatz des Vorgesetzten und je nach Stimmungs-/Interessenlage Feedback zu den spezifischen Aufgaben einholen, die zur Situation passen. 3-4 Aufgaben besprechen, je nach Widerstand (also der Menge der Einwände oder neuen Ideen). Die restlichen Aufgaben zurückhalten und erst zugeben, dass sie erledigt sind, wenn die Simmungs-/Interessenlage sich gewandelt hat. 
  - Die "verlorenen Aufgaben", die nun abgenommen sind, müssen nach dem Angriff durch neue ersetzt werden. Aber man behält den Rest der Truppen. Was kein Problem ist, denn vermutlich hat sich der Vorgesetzte mit Änderungswünschen geäußert. 
  
#### Guerillia-Angriff
  - Man hat eine Reihe von Dingen, zu denen man Feedback braucht, der Vorgesetzte versteckt sich aber immer in Besprechungen o.ä..
  - Man stellt die Liste zusammen. 
  - Per Scouting findet man z.B. Essenspläne, oder man stellt sich in die Nähe der Kaffeemaschine
  - "Wo ich Dich gerade sehe." (1-2 Punkte besprechen, dann sofort wieder zurückziehen, bevor der Vorgesetzte sich überrannt vorkommt)

## Vorgesetzte

### Rushen
  - Entwickler mit kleinen Aufgaben überhäufen, die alle keinen großen Wert haben
  - so schnell neue kleine Aufgaben ausdenken, dass die Entwickler nicht mit Aufrüsten oder Einigeln reagieren können, sondern selbst ebenfalls kurzfristige Lösungen produzieren müssen

### Micromanagement
  - Den Entwicklern bis ins letzte Detail vorgeben, was sie machen müssen.
  - Stetiges Einmischen in die Lösung
  - Am Besten mit Driften und Statusmeetings kombinieren
  
### Driften
  - Auf jede Frage zu Aufgabendetails mit einer leichten Abweichung zur ursprünglichen Erklärung reagieren, die zunächst unwichtig scheint, aber in der Implementierung einen Unterschied macht
  - Da jede leichte Abweichung eine weitere Verunsicherung und damit weitere Nachfragen verursacht...
  
### Einigeln
  - Aufgabenbeschreibungen in Buchform

### Expansion
  - Aufgaben basieren auf Features, die noch nicht implementiert sind
  
### Dampfwalze
  - Immer wieder neue Aufgaben schicken, schneller, als die Entwicklung die bestehenden Aufgaben abarbeiten kann.
  - Komplexe Aufgaben verwenden, die 1-2 oder mehr Tage halten, während der Aufgabenstrom nicht abreist.
  
#### Aufrüsten
  - Ticketsystem anschaffen oder andere Technologien um große Mengen an Aufgaben zu verwalten

### Taktiken

#### Scouten
  - Statusmeetings
  - Statusmails
  - Umfragen bei Mitarbeitern der Entwicklerabteilung oder anderen Abteilungen bzgl. der Funktionen der Software oder bzgl. Problemen

#### Hinterhalt
  - "Ich habe dem Kunden leider schon versprochen, dass wir das Feature nächste Woche haben." "Ich kann ihn noch maximal x Tage hinhalten."
  - Eine Reihe von Aufgaben bereits fertig haben. Wenn ein Entwickler eine Frage hat oder sonst die Nase aus dem Zimmer steckt, immer eine Aufgabe mehr mitgeben, bis keine Fragen mehr kommen. Dumme Fragen durchaus mit mehr Aufgaben belohnen, um den Lerneffekt zu verstärken.
  
#### Angriff
  - Viele unterschiedliche Aufgaben bereit haben. Dann Meeting einberufen.
  
#### Guerillia-Angriff
  - Durch das Büro schlendern oder Entwickler beim Scouten abfangen und sie dann mit Ideen bombardieren.

  
  
