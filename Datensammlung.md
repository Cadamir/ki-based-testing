# Datensammlung

* Möglichst schnelle Auslieferung von Produkten [1/1]
* Optimierung durch DevOps Bausteinen [1/1]
* Testautomatisierung soll [1/1]
   * Zeit reduzieren
   * Arbeit reduzieren
* Testautomatisierung macht [1/1]
   * Wartung (oft Kleinarbeit)
   * End-To-End-Tests sehr anfällig
   * Langwierige Analysen
   * Registrierungsaufwand von GUI-Objekten
* Was ist künstliche Intelligenz [1/1]
   * "die Lehre der Automatisierung intelligenten Verahltens, sowie des maschinellens Lernens" ([1/1] - "Künstliche Intelligenz - was bedeutete das eigentlich?")
   * stark vs schwach
   * starke noch nicht ernsthaft vorhanden
   * schwach imitiert Intelligenz basierend auf Regeln
   * Muster/Gesetzmäßigkeiten erkennen/verallgemeinern
   * Arbeitet mit Wahrscheinlickeiten [1/3]
   * KI macht aus Daten Informationen und aus Informationen Wissen [1/3]
* Testen mit KI
   * GUI analysieren
   * Testfälle abschätzen, 
   * Automatische Wartung einiger Skripte
   * Optische Veränderungen aufzeigen
   * Testberichte
   * Auswahl und Priorisierung von Regressionstestfällen
* Einsatz KI bisher [1/2] (notwendig?)
   * große Datenmengen auswerten
   * Situationen mit statistischenr Analyse bewerten
   * Vorhersagen treffen
   * Spachbot, Chatbot, Werbung, Big Data
* Spidering AI [1/3]
   * Automatisierte Generierung von Testfällen durch "Spidering"
   * Crawled Anwendungsdaten
      * Screenshots
      * HTML-Code-Download
      * Ladezeitenmessung
   * Wiederholung um KI zu trainieren
   * bei signifikaten Änderungen (zB. Ladezeit) Error/potentielles Problem
   * Mensch muss Probleme betrachten
* Visual Validation Automation Testing [1/3]
   * Richtige Daten am Frontend 
   * Erscheinungsbild gesamt und einzelnelemente werden validiert
   * vergleicht aktuelle Screenshots mit originalen Screenshotes
* API-Test [1/3]
   * hohe Testabdeckung
   * geringe Komplexität
   * Testgenerierung 
* Qualitätssicherung [11]
  * "Aufgabe der Qualitätssicherung, jedwede Art von Fehlern vor der Auslieferung einer Software zu finden und das Auftreten von Fehlern beim Kunden zu vermeiden." ([11], 2.2 Konstruktive und analytische Qualitätssicherung, S. 19)
  * Fehler kann nicht beobachtet werden -> nur Fehlverhalten -> daraus Fehler ableiten
  * Fehler:
    * Programmfehler
    * Zusammenspielfehler
    * Anforderungsfehler
  * Fehlerbehebung kann sehr teuer werden
* analytische Qualitätssicherung: Code bereits fertig entwickelt und wird abschließend aus Fehler untersucht ([11], 2 Grundbegriffe der Qualitätssicherung, S 20)
* konstruktive Qualitätssicherung: "Der Ansatz, bereits vor der Ausführung der eigentlichen Arbeit Qualitätsrichtlinien auszugeben" ([11], 2 Grundbegriffe der Qualitätssicherung, S 20)
* "komplexer werdende Softwaresysteme in kürzerer Zeit zu verifizieren." ([10], 30.1 Künstliche Intelligenz, S 243)
* Überwachung der produktiven Software in Echtzeit und Prognosen über zukünftige Veränderungen und Abweichungen ([10], 30.1 Künstliche Intelligenz, S. 243)
* Testabdeckung steigern ([10], S. 243)
* Nach risikobasiertem und agilem Testen bedeutet KI erneut ein Umdenken für Softwaretester ([10], S. 244)
* "mit sinnvollen Daten [...] trainiert werden" ([10]. S. 244)
* "KI wird nicht dazu führen, dass Tester überflüssig werden" ([10], S. 244)
* Autonomiegrad in KI-gestützten Testen noch niedriger als bei anderen KI-Themen ([10] S 244)
* Frage angebracht, ob Testautomatisierungstools das nicht bereits tun ([10] S 245)
  * Automatisierung zu helfen 
  * Aufwand an mühseligen Routinearbeiten beim Entwickeln und Testen zu verringern
  * Tests für Entwickler durchzuführen und Ergebnisse zu liefern tun Tool schon
  * aber dummes ausführen der tests
  * Auf Codeänderung und anderen Metriken könnte KI nur notwendige Tests starten
  * "Der Nutzen der KI resultiert daraus, dass die direkte Einbeziehung der Entwickler oder Tester in die besonders profanen Aufgaben reduziert wird." ([10], 30.2 Anwendungsbereiche künstlicher Intelligenz S. 245)
* Softwaretest mehrere Phasen [18 S 1]
* Testmanagement "erstreckt sich von der Testplanung über die Erstellung der Testspezifikation und Durchführung der Tests bis hin zur Protokollierung der Testergebnisse und der Auswertung der Tests" ([18], Der Testprozess, S. 1)
  * Incident Management
    * Reaktion auf erkannte/vermutete Störungen und vorbereitende Maßnahmen (ist organisatorischer/technischer Prozess) 
  * Problem Management
    * Ermitteln, Bewerten, Korrektur aufgetretener Fehler
  * Change Management
    * Bearbeitung zusätzlicher/geänderter Anforderungen während des Projektes
  * Release Management
    * Planung/Konfiguration einzelner Software-Releases
* ISTQB-Testprozess ([18] S. 2) 
  * ISTQB = International Software Test Qualifikation Board
  * Planung/Steuerung
  * Analyse/Design
  * Realisierung/Durchführung
  * Auswertung/Bericht
  * Abschluss
  * überlappungen möglich 
* Testprozess ([18] S. 2/3)
  * Säulen ABC
  * A. Fachliches KnowHow
  * B. Methodik 
  * C. Testwerkzeuge
    * Testwerkzeuge = Hauptaugenmerk
    * Testautomatisierung
    * Tools für Testmanagement/Fehlermanagement
  * Phasen (aus V-Modell)
    * Planung
      * Konzept
      * Plan
      * Beschreibung von 
        * Testobjekt
        * Testumgebung
        * Konfiguration
        * Testressourcen
        * welche Tools
        * Testumfang
    * Design
      * Verfeinerung des Planes
      * Dokumentation von
        * Anforderungen
        * Szenarien
        * Testkritierien
      * (mgl. mit Planung zusammen)
    * Spezifikation
      * Beschreibung Testfälle im Detail
        * Testvoraussetzungen
        * erforderliche Eingaben
        * erwartete Ausgaben
        * Abhängigkeiten zwischen Testschritten
      * funtionale und nicht funktionale Anforderungen
    * Durchführung
      * manuell und/oder automatisiert
      * meist iterativ mit der Software-Entwicklung
      * Regressionstests bei behobenen Fehlern
      * Umfang wird meist im Laufe der Zeit größer
    * Protokollierung
      * Ergebnisse aufzeigen
      * manuell: Checklisten, Berichte
      * automatisiert: Log
    * Auswertung
      * Analyse dieser Ergebnisse
      * teilweise Rückkehr zu älteren Phasen
* Warum tests? ([18] S. 7)
  * komplexere Produkte
    * viele Features
    * viele Komponenten
    * Verändungen haben viele Abhängigkeiten
  * schnellere Produktzyklen
    * mehr Produkte in weniger Zeit
  * stärkerer Wettbewerb
    * Globalisierung -> Vergleichbarkeit/Austauschbarkeit einfacher
  * verteilte Entwicklung
* Test-reviewing [18] S. 13
  * Neue Anforderungen
  * erweiterte  Szenarien
  * Tests kritisch betrachten, ergänzen, aktualisieren
* Normen:  [18] S. 22
  * IEEE 829 (S. 22)
    * Übersicht -> Testkonzept
    * Spezifikation
      * Testentwurfspezifikation -> verfeinerte Beschreibung der Vorgehensweise
      * Testfallspezifikation -> Eingabewerte, Ausgabewerte, ist vom Testdesign getrennt
      * Testablaufspezifikation -> Beschreibung aller Schritte zur Durchführung von Testfällen, Implementierung des Testdesigns
    * Bericht
      * Objektübergabebericht -> Beschreibung Übergabe Testfälle, bei getrennter entwicklung
      * Testprotokoll -> Aufzeichnung
      * Testabweichungsbericht -> Aufzeichnung nachprüfungswürdiger Ereignisse
      * Abschlussbericht -> fasst Testaktivitäten zusammen
  * ISO 9126 (S. 22-25)
    * Qualitätsziele: Zuverlässigkeit, Performance und Sicherheit -> durch Tests bestätigen
    * Funktionalität -> "Vorhandensein der Funktionen mit festgelegten Eigenschaften" (S. 23)
      * Angemessenheit -> Eignung für spezifizierte Aufgabe
      * Korrektheit -> Richtige Rückgabewerte und Wirkungen
      * Interoperabilität 
      * Sicherheit
      * Ordnungsmäßigkeit -> Merkmale zur Erfüllung von Vereinbarungen, gesetzl. Richtlinien, anwendungsspezifische Normen
      * Konformität -> Einhalten von Standarts, Konventionen, gestzl. Bestimmungen u.ä.  
    * Zuverlässigkeit -> Leistungsniveau unter festgelegten Bedingungen über einen festgelegten Zeitraum zu bewahren
      * Reife -> seltenes Vesagen
      * Fehlertoleranz -> Leistungsniveau halten trozt Software-Fehler/Schnittstellen-Nicht-Einhaltung
      * Wiederherstellbarkeit -> Leistungsniveau wiederherstellen + Daten wiedergewinnen, Zeit und Aufwand berücksichtigen
      * Konformität -> Grad, Normen oder Vereinbarungen zur Zuverlässigkeit einzuhalten
    * Benutzbarkeit
      * Verständlichkeit
      * Erlernbarkeit
      * Bedienbarkeit
      * Attraktivität
      * Konformität
    * Effizints
      * Zeitverhalten -> Antwort-/Verarbeitungszeit und Durchsatz
      * Verbrauchsverhalten -> Ressourcenverbrauch, Anzahl/Dauer benötigter Betriebsmittel
      * Konformität
    * Änderbarkeit/Wartbarkeit
      * Analysierbarkeit
      * Modifizierbarkeit -> Aufwand von Verbesserungen, ...
      * Stabilität -> Wahrscheinlichkeit des Auftretens unerwartert Abhängigkeiten
      * Testbarkeit -> Aufwand für Testen nach Änderungen
      * Konformität
    * Übertragbarkeit
      * Anpassbarkeit
      * Installierbarkeit
      * Koexistenz
      * Austauschbarkeit
      * Konformität
  * ISO IEC-29119 (S. 25-26)
    * "definiert Testbegriffe, Testprozesse, Testdokumentation und einzelne Testtechniken" ([18] S. 25)
    * ISO/IEC 29119-1: Concepts & Definitions
    * ISO/IEC 29119-2: Test Processes
    * ISO/IEC 29119-3: Test Documentation
    * ISO/IEC 29119-4: Test Techniques
    * ISO/IEC 29119-5: Keyword Driven Testing
* 

