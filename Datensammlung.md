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
* Alte QA-Welt [1/4]
  * Bestandteile
    * UI
    * Peripherie (Bildschrim, Tastatur, Schreibpad, ...)
    * Core-Software
    * Schnittstellen zu "Umsoftware"
    * Speicher
  * Tests
    * Unit-Tests
    * System-Tests (ST)
    * System-Integration-Tests (SST)
  * funktionale Tests -> korrektes Ergebnis
  * nicht-funktionale Tests -> Werte im Rahmen (Ladezeit, ...)
  * User Akzeptanztests (UAT) -> Verwendbares Design/System für Nutzer
  * Bei KI ändert sich nur Steuerung (Core-Software Steuerungskomponente)
* Qualitätssicherung [11]
  * "Aufgabe der Qualitätssicherung, jedwede Art von Fehlern vor der Auslieferung einer Software zu finden und das Auftreten von Fehlern beim Kunden zu vermeiden." ([11], 2.2 Konstruktive und analytische Qualitätssicherung, S. 19)
  * Fehler kann nicht beobachtet werden -> nur Fehlverhalten -> daraus Fehler ableiten
  * Fehler:
    * Programmfehler
    * Zusammenspielfehler
    * Anforderungsfehler
  * Fehlerbehebung kann sehr teuer werden
* [1/4][1/5] -> es geht darum, wie eine KI gestestet werden kann und nicht, wie eine KI testet
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
* KI [5]
* Machine Learnig (ML) Teilgebiet KI [5] S. 18
* Deep Learning (DL) Teilgebiet ML [5] S. 18
* ML -> Strukturen erkennen aus dem Lösen vorgegebener Probleme, um diese Strukturen auf Anwendungen zu übertragen
* Trainig: supervised Learning (SL), unsupvised Learning (UL), reinforcement Learining (RL) [5] S. 18
* Traditionelle ML: Datenvorverarbeitung -> Merkmalextraktion -> Merkmalreduktion -> Modellentwicklung [5] S. 19
* Daten: normalisiert, fehlerfrei, keine Verzerrung [5] S. 19
* DL: End-to-End [5] S. 19
  * keine Merkmalsextrakiton
  * keine Problemdekomposition 
  * orientierung an der Funktionsweise des menschlichen Gehirns [5] S. 67
* KI Beispiele [5] S. 18 (Fußnote)
  * ML
  * Wissensrepräsentation
  * logisches Schließen
  * Planungsalgorithmen
  * Suchalgorithmen
  * regelbasierte Systeme
  * fallbasiertes, nicht monotones Schließen
  * Contrain-basierte Programmierung
  * Optimierung
* ML-Beispiele [5] S. 18
  * DL
  * Entscheidungsbäume
  * Random Forest
  * Support Vector Machines
  * genetische Algorithmen
* KI-Ziel: >= Performance wie menschlicher Experte, Arbeitet mit Wissen und Verstand [5] S. 33
* Klassifiezierung von Programmen [5] S. 33-35
  * Wissenbasierte Syteme: [5] S. 33
    * hoher Entwicklungsaufwand
    * leicht erklärbar
    * Trennung Wissen und maschine
    * menschlicher Entwickler braucht hohes Wissen
  * regelbasierte Systeme: [5] S. 34
    * Wissensbasis + Interfenzmaschine
    * Wissenbasis enthält: Daten, Fakten, Regeln
    * Interferenzmaschine wendet Regeln an, um neue Fakten zu generieren
    * Manueller Aufbau/Wartung der Wissensbasis
    * Regel: Prämisse (Wenn) und Konklusion (Dann)
    * Regeln = Flaschenhals (ungenaue Definition, mehrere gleichzeitig anwendbar, ...)
  * fallbasierte Systeme: [5] S. 34-35
    * Lösen durch Erfahrungswerte
    * ähnliche Probleme -> ähnliche Lösungen
    * _retrieve_ -> Lösen mit vorhandenen Lösungen
    * _reuse_ -> Lösungsansätze wiederverwenden
    * _revise_ -> gefundene Lösungen anpassen
    * _retain_ -> beste Lösung speichern
* Lernen 2D kategorisierbar [5] S. 39
  * Lernmodus
    * SL
    * UL
    * Semi-SL
    * RL
    * Active Learning (AL)
  * Problem
    * Regression -> Kontinuierlichen Wert vorhersagen
    * Klassifizierung -> Objekt in Gruppe einsortieren
    * Clustering -> ähnliche Objekte zusammenfassen
  * Matrix zur Einordnung entsteht
* Supervised Learning [5] S. 39-41
  * vorgeben, was gelernt werden soll
  * Trainigspaar: Eingabe + erwartete Ausgabe
  * erstellen eines Modells -> mit Trainingsdaten lernen -> mit neuen Daten arbeiten
  * Beim lernen -> Rückgabe, wie korrekt eine Antwort war -> Anpassung des Modells
  * Anpassung = Lernen
  * Wiederholung der Anpassung bis Ergebnisse akzeptable sind oder sich nicht mehr ändern
  * _Regression_ 
    * kontinuierliche Daten vorhersagen
    * mgl. statistische Methoden (lineare Regression, polynomiale Regression, multivariate Regression, ...)
    * Einfluss von Variablen aufs Endergebnis
    * Variablen sind unabhängig -> Features, Einflussgrößen
    * Endergebnis -> Zielgröße
    * Spezialfall: logisitische Regression (binäre Klassifikation) -> Ergebniss 1 oder 0
  * _Klassifikation_
    * Klassenzugehörigkeit zuordnen
    * Abbildung von Merkmalen auf Diskrete Werte (Label)
    * Klassen schon in der Trainingsphase bekannt
  * _Zeitreihen_
    * künftige Werte vorhersagen auf Basis von alten Werten
    * zeitlich geordnete Werte
    * Strukturen inhärent in einer Zeitreihe
    * eine Art der Regression
* Unsupervised Learning [5] S. 4
  * vorhandene Daten explorieren und strukturelle Ähnlichkeiten identifizieren
  * keine Beispiele vorhanden
  * für große, unstrukturierte Datenmengen
  * Ähnlichkeit innerhalb einer Gruppe maximieren
  * typisch ist Clustering
  * Regelsuche
  * Zusammenhänge (wer das kaufte, kaufte zu X% auch dies)
* Semi-supervised Learning [5] S. 42
  * Mischform SL und UL
  * Mischung gelabelter und ungelabelter Daten
  * meist mehr ungelabelt als gelabelt
  * Anfang training mit gelabelten Daten
  * Lernperformanz erhöhen durch ungelabelte Daten
* Reinforcement Learning [5] S. 42-44
  * richtige Aktionen belohnen
  * schlechte Aktionen bestrafen
  * gut, wenn man Ergebnis gut einordnen kann, ohne den Weg vorzugeben
  * sehr Ressourcen aufwendig -> Trial-and-Error -> sehr viele Wiederholungen
* Aktives Lernen [5] S. 44
  * aktivies semi-SL
  * Entwickler klassifizerien ebenfalls Daten (unlabelt to labelt)
* Daten zentrale Rolle [5] S. 46
  * Ohne Daten kein Training
* Neuronale Netze [5] S. 67-106
  * Aus künstlichen Neuronen aufgebaut (wie Gehirn)
  * mehrere Neuronen-Schichten
  * 1943 Warren McCulloch und Walter Pitts -> erste Modellierung neuronaler Netze -> Neuron kann 0 und 1 oder kontinuierliche Werte mit Schwellenwerte
  * künstliches Neuron = Perzeptron
  * Dendrite/Eingabe = Eingabewerte
  * Zellkörper = Berechnungsformel
  * Axiom = Ausgabe
  * inhibitorische/exzitatorische Eigenschaften = Gewichtungen
  * Überschreiten eines Schwellenwertes durch Aktivierungsfunktion gesteuert
  * Bias als Grundgewicht
  * Bias + Eingabevektor = Gesamte eingabe für ein Perzeptron
  * Eingaben -> Übertragungsfunktion -> Aktivierungsfunktion -> Ausgabe
  * Übertragungsfunktion fasst die gesamte Eingabe zusammen
  * Eingabewerte = n-dimensionale Vektor X mit Werten x_i
  * zu jedem x_i -> w_i (Gewichtung)
  * Übertragungsfunktion: a = \sum_{i=1}^{n} w_{i} * x_{i} + b [5] S. 69
    * a = Ergebniss der Übertragungsfunktion
    * n = Dimension des Eingabevektors
    * w = Gewichtung
    * x = Eingabewert
    * b = Bias
  * Aktivierungsfunktion: [5] S. 70
    * Bekommt a von Übertragungsfunktion als Parameter
    * Ergebniss = Ausgabe des Neurons
    * verschiedene Funktionen mgl
      * Identiätsfunktion x=y
      * Heaviside-Funktion y = 0 -> x<0: 1 -> x >=0
      * sigmoid = y = \frac{1}{1+e^{-x}}
      * tanh()
      * ReLU
      * SoftsSign
      * SoftMax
  * Gewichtungsanpassung: [5] S. 70-71
    * bei elemtaren Neuronen (Indentiätsfunktion)
    * w_{i,new} = w_{i,old} + mykro * \frac{delta E}{delta w_{i}}
    * w_{i,new} = w_{i,old} + mykro * (y_{i,soll} * y_{i,ist}) * x_{i}
    * kann beliebig wiederholt werden
    * mykro = Lernrate
    * E = Fehlerfunktion
  * mehrschichtige neuronale Netze [5] S. 71
    * Eingabeschicht (Input Layer) -> stellen numerische Merkmalsvektoren dar, ein Neuron = ein Merkmal
    * versteckte Schichten (Hidden Layers) -> Weiterverarbeitung, zB. Filteroperationen, mehr als 1 = tiefes Neuronales Netz
    * Ausgabeschicht (output Layer) -> Zielwert
  * vorwärtsgekoppelte Netze (feedforward)
    * unidirektionale Verbindungen 
    * von Input nach Output
    * gerichteter, azyklischer Graph
    * von einer Schicht zur nächsten
    * niemals zurück
  * rückgekoppelte Netze (feedback)
    * Rückkopplungen zum direkten Vorgänger (direkte Rückkopplung)
    * Rückkopplungen zu vorhergehenden Schichten (indirekte Rückkopplung)
    * oft bei temporalen Aspekten oder bei Sequenzen
  * Abbildung eines gegebenen Eingabevektors auf einen Ausgabevektor = Modell
  * Lernprozess [5] S. 75/76
    * Struktur des künstlichen neuronalen Netzwerkes (KNN) (nach Gefühl, nach bekannten Ansätzen)
    * Hyperparameter festlegen (zB. Anzahl Trainingszüglen)
    * zufällige Bestimmung der Gewichtungen und der Bias
    * Trainigsdaten den Netzwerk geben
    * Feed Forward der Daten
    * Fehlerevaluation (zB. RMSE)
    * Wenn kein Fehlerminimum und noch nicht die Maximale Trainingsrundenanzahl erreicht wurde, werden die Gewichtungen und der Bias angepasst, die Anzahl der trainierten Runden wird erhöht
    * Wenn die Fehler minimiert oder die Maxtrainingsanzahl erreicht wurde -> Modell evaluierren -> Testdaten verwenden
    * Fehlerbestimmung mit Testdaten -> Fehler ok = Modell nutzbbar, Fehler zu viele = Begin von vorn mit neuer Struktur
  * = SL
  * Fehlerfunktion [5] S. 76-77
    * engl. loss function
    * verschiedene Möglich
      * Klassifikation: Categorical Crossentropy, Log Loss, Relative Entropy, Exponential loss
      * Regression: Mean Absolute Error, Mean Squared Error
      * Mean Squared Error (MSE): E = \frac{1}{n} * \sum_{i=1}^{n} (y_{i, soll} - y_{i,ist})^2
      * n = Anzahl (Trainings-)(Test-)beispiele  
  * Anpassung der Gewichtung von hinten nach vorn (Backpropagation) [5] S. 78
  * online-Anpassung: nach jedem Trainingsbeispiel
  * Batch-Anpassung: nach einer Gewissen Menge an Beispielen (Batch-Size)
  * Mini-Batch-Anpassung: Batch-Size < Anzahl Trainingsdaten
  * Epoche = kompletter Trainingsdurchlauf
  * Gradientverfahren [5] S. 79
    * durch kleine Korrekturen Fehlerfunktion minimieren
    * in Richtung des steilsten Abstiegs (Gradient)
    * bei Iterationsschritt -> minimum überspringen
    * multidimensionaler Raum
    * verschiedene Algorithmen:
      * SGD (Stachatic Gradient Descent)
      * Momentum
      * AdaGrad (Adaptive Gradient)
      * AdaDelta
      * Adam (Adaptie Movememnt Estimation)
      * RMSprop (Root Mean Square Propagation)
  * Datenaufbereitung
    * Trainingsset
      * Lernbeispiele
      * interative Einspeisung
      * Training
      * ca. 80% aller Daten
    * Validierungsset
      * Schutz vor Overfitting
      * zur Justierung von Hyperparameter (az. Schichten, az. Neuronone in Schicht, 
      * wenn Fehler im Validierungsset nicht abnimmt -> Abbruch Training -> Early Stopping
      * statt Validierungsset -> Kreuzvalidierung
    * Testset
      * für fertiges Modell
      * zur Präzesionsberechnung des fertigen Modells
      * ca. 20%
  * Netzarchitekturen
    * Full Connected Layer -> Jedes Neuron ist mit allen Neuronen er folgenden Schicht verbunden
    * Convolutional Neural Network (CNN) [5] S. 91ff
      * feedforward
      * Klassifikation
      * Bild/Video
      * Input Layer 
      * Convolution Layer -> Filter/Convolution -> Feature Map
      * Activation Layer -> Aktivierungsfunkiton auf Feature Map
      * Pooling Layer -> Dimension der Feature Map verringern (weniger Graustufen)
      * Full Connected Layer -> auch mehrere Möglich
      * Output Layer
      * Eingabe -> (Feature Extraktion)* -> Klassenzuordnung -> Ausgabe (* beliebig oft wiederholbar)
    * Rekurrente neuronale Netze (RNN) [5] S. 96ff
      * für zeitlich abhängige Aufgaben
      * für Aufgaben mit Gedächtnis/Kontex
      * Spracherkennung, Textvervollständigugn, ...
      * LSTMs (Long Short Term Memory) = spezialfall -> haben Zustandszellen
      * feedback
    * Gernerative Adversarial Networks (GAN) [5] S. 97
      * neue Daten aus Trainingsdaten
      * zwei Netze treten gegeneinander an (Generator vs. Diskriminator)
      * Generator erzeugt neue Daten auf Basis des vorliegenden Datensets
      * Diskriminator prüft in Echtzeit, ob neue Daten zum trainingsset passen
    * weiter hier: https://www.asimovinstitute.org/neural-network-zoo/
* test.ai [19]
  * Tool erforscht selbst die Anwendung
  * interagiert automatisch mit der Anwendung
  * erkennt Zustände, Elemente und Wege
  * Benennung von Zuständen und Elementen
  * überprüft alle Features
  * generierung von KI-baiserten Modellen zur Erkennung von Zuständen u. Elementen u. automatischer Navigation
  * erforscht die Anwendung im Test, um neue Bereiche zu finden
  * Test-Creation
    * ML
    * visuelles Wiederfinden von Elementen
    * Test-Composer -> Test-Bot beaufsichtigen und steuern
    * Test in Echtzeit erstellen
  * hochskalierbar
  * Optische Ergebnis-Aufbereitung
* test.ai
  * Elemente müssen nicht mehr explizit angegeben werden, sondern werden überr ML erkannt
  * kein XPath, CSS, ...
  * Screenshots bei jedem Schritt
  * Schritte sind auf dem Screenshot hervorgehoben
  * reinforcement learning
  * Python-Skripte mgl.
  * Human-Interface
    * Bot Training -> Interfaces benennen
    * Test Spezifikation
    * Bot Configuration
    * Analytics
    * Knowledge Base
  * Application Interaktion
    * Exploration
    * Test-Ausführung
  * Cortex: ML Brain
    * Objekt Lokalisierung
    * Objekt Klassifizierung
    * Lernen
  * Device Interaktion
    * Sensoren -> Objekt Modell, Bildaufnahme, Videoaufnahme
    * Aktoren -> Maus, Tastatur, Touch, Gamepad
  * Supportet Plattforms
    * Laptop, Computer, Mobile, Apple, Android, PS4, XBox, Switch
* test.ai [21]
  * Workflow
    * Collect Data
    * Classify Data
    * Train AI
    * Create Tests
    * Run Tests
    * Review Results
  * AI-Usage
    * Crawl UI -> UI durchsuchen/Browsen
      * Q-Learning
      * Lernen zu navigieren von Seite zu Seite
      * Erstellen eines App-Graphen -> Finden des besten Weges oder eines Ersatzweges
    * sehende Roboter
      * keine Element-Pfade/-Locators
      * Visual Detection um Elemente zu erkennen
      * erkannte Elemente müssen dann benannt werden (vom Tester)
      * Neuronales Netz wird dann darauf trainiert
      * Bots können menschliche Interaktionen nachstellen
      * desto größer die Unterschiede beim Training, desto allgemeiner wird die KI
    * Objektklassifizierung
      * Nutzen von bekannten Icons/Buttons allgemein
      * Nutzen von speziell für die eine App trainierte Buttons
* download von test.ai zurzeit scheinbar nicht mgl. 
* mabl [22]
  * Workspace
    * Oberfläche des Testers
    * vereint alle weiteren Punkte in sich
    * jeder Entwickler hat eigenen Workspace
    * ein Workspace mit vielen Enviorments
    * Dashboard
      * 'status-check'
      * aktuelle Nutzungszahlen
      * Navigation zu anderen Komponenten
  * Enviroment
    * Umgebungen
    * Test, Abnahme, Produktion, ...
    * kann Umgebungsvariablen nutzen
    * Umgebungsvariablen von allen Tests der Umgebung nutzbar
  * Application
    * dargestellt mit ihren URLs
    * Eine Applikation kann merheren Umgebungen zugeordnet werden
    * in Configuration erstellbar
  * Plan
    * mehrere Tests für einen Bereich der App
    * gibt an, wie automatisiert werden soll
    * ein Plan hat nur eine App
    * eine App hat mehrere Pläne
  * Test
    * Menge von Schritten um eine Funktionalität zu definieren
    * für kleine Bereiche/einzelne Features
    * Ein Test kann zu mehreren Plänen gehören
    * Im Test-Bereich
      * Details: Einzelschritte
      * Verlauf
      * zugeordnete Plänge
      * Testveränderung im Laufe der Zeit
  * Test Result -> viele Informationen
  * Elemtsuche
    * Standart
      * Element auswählen
      * Informationen darüber sammeln
      * Beim Test Element mit bester Übereinstimmung
    * Konfigurierte
      * einstellbar, welche Attribute am wichtigsten sind
      * Suchstrategie veränderlich
    * warten und warten
      * Es kann gewartet werden 
      * statische Zeitspanne gewartet
      * warten bis ein Element ein gewisses Attribut hat
    * Pfad-Selektoren
      * CSS, XPath
      * zusätzliche Kontrolle
      * keine Selbstheilung
    * Vorteile: 
      * Selbstheilung
      * Änderungsrobust
      * Vielseitig
  * Selbstheilung
    * Bei jeder Interaktion mit Element -> Speichern der Attribute fürs nächste Finden
    * über 30 Attribute
    * Finden: suche das ähnlichste Element
    * Suche: 1. Kandidaten raussuche -> bester Kandidat
    * Erstmal warten wenn nichts gefunden wurde
    * Wenn kein eindeutiger Kandidat gefunden wurde -> Ausprobieren -> Erfolg: Test pass, überschreiben der Infos <-> Misserfolg: Test error, Autoheal versuch in Log, Fehlerzeigen
    * Ad-hocs tests verändern keine gespeicherten Informationen
* ML [2] S. 201
  * kein Rule-Set programmieren
  * Regeln lernen von Beispielen
  * zB. kein Hand-erstellter Decision-Tree
  * Modell macht vorhersagen
  * Grundlage sind "Beobachtungen" und Vorhersagewert
  * Merkmalsextraktion ist wichtig
    * Handerlesene Merkmale  
      * Daten von Experten in Merkmale aufgeteilt
      * Wichtige Merkmale erhalten lassen
      * Unwichtige/Störende Merkmale entfernen
      * Wenn ein bekannter/starker Zusammenhang zwischen einen Merkmal und Ergebnis besteht: Nutze das Merkmal
    * Algorithmische Merkmalsextraktion
      * Algorithmus unterscheidet wichtige von unwichtigen Merkmalen
      * unvariante Merkmalsextraktion -> Merkmale einzeln betrachten
      * multivariante Merkmalsextraktion -> Merkmale im Zusammenhang
    * Algorithmische generierung von Merkmalen
      * Extraktor durch Trainingsdaten trainiert
      * keine Beschränkung auf bestimmtes Merkmalsvokabular
  * Nearest Neighbor -> sehr Empfindlich bei unnötigen Merkmalen
  * Support Vektor Machine -> sehr Empfindlich
  * Verbesserung -> robust gegen uninformative Merkmale
    * boosting Models (zB. AdaBoost)
    * bagging Models (zB. RandomForest)
  * schwache Lerner (weak learners) genutzt -> Zusammenschluss der schwachen erstellt Vorhersage
  * verschiedene Teilmengen der Trainingsdaten werden für verschiedene schwache Lerner genutzt
  * schwache Lerner die keine Ahnung von Problem haben -> gleichmäßig verteilte unterschiedliche Ergebnisse -> gleichen sich aus
  * schwache Lerner mit Ahnung -> stimmen fürs selbe -> leichte Erhöhung an der richtigen Stelle
  * Klassifizierungsmodelle: [2] S. 206f
    * k-Nearest Neighbors -> Merkmale eines Objektes zu Vektor/Punkt -> Abstand zu allen anderen Punkten/Objekten -> k kürzeste Abstände Punkte werden die Klassen gezählt -> häufigste Klasse = eigene Klasse
    * Suport Vector Machine:
      * ermittelt relative Dichte
      * Support Vektoren werden ermittelt
      * Vectoren sind ähnlich zu den Grenzen (Borders) im Merkmals-Raum
      * Vektoren haben den maximalen Abstand zueinander
      * Hyperplane wird zwischen den Vektoren erstellt
      * Hyperplane hat eine Dimension weniger als der eigentliche Merkmalsraum
    * Entscheidungsbäume
      * Klassifikation
      * Reihe von Entscheidungen
      * Jede Verzweigung = ein Merkmal
      * Schlussendlich -> Blatt = Klasse
      * kein kontinuierlicher Vektorraum notwendig/mgl
      * Alle Merkmale werden als diskrete Werte betrachtet
      * Kategorische Merkmale gehen je nach Kategorie in andere Äste
      * Skalare Werte -> Schwellenwert(e) zur Unterscheidung
      * sehr anfällig für Overfitting/Overtraining
  * Ensemble Modelle [2] S. 209ff
    * -> durch viele einfache Modelle
    * -> einzelnes Modell oft nur mit Teil-Trainingsdaten trainiert
    * -> einfaches Modell = schwache Lerner (weak Learners)
    * -> einzelne Vorhersagen zusammen eine gemeinsame
    * geringe Variance: -> ähnliche/gleiche Ergebnisse bei ähnlichen/gleichen Problemen
    * geringer Bias: -> nah an der Wahrheit
    * Bias/Verzerrung: Eine falsche Schätzung der Modellparameter, so dass sie nicht die tatsächliche Verteilung der Stichprobendaten widerspiegeln. ([2] S. 211, Übersetzt mit DeepL)
    * Varianz: Die Varianz der Vorhersage, die entsteht, wenn das Modell die Verteilung der Trainingsdaten gut wiedergibt, aber die Generalisierung auf neue Daten leidet. ([2] S. 211, Übersetzt mit DeepL)
    * Overfitting:  Das Modell folgt der Verteilung der Trainingsdaten in einem Maße, das seine Genauigkeit bei neuen Daten verringert. ([2] S. 211, Übersetzt mit DeepL)
    * Underfitting: Das Modell spiegelt die Verteilung der Trainingsdaten nicht angemessen wieder. ([2] S. 211, Übersetzt mit DeepL)
    * Random Forest 211ff
      * begging (hoffen das es klappt?)
      * weak Learners (WL)
      * sehr simple
      * Entscheidung aufgrund einer Teilmenge der Merkmale
      * Trainiert mit Teil-Trainings-Sets
      * Weak Learners = decision Trees
      * Abstimmung entscheidet das finale Ergebnis
    * AdaBoost S, 215
      * boosting
      * Kaskade einfacher Klassifikationsmodelle
      * random Subset of Trainingdata -> trainiere ersten WL -> neues Trainingsset (ein Teil zufällig, ein Teil, wo erster WL schlecht war) -> 2. WL training -> ...
  * Neural Networks [2] S. 215
    * an Gehirn angelehnt
    * 2 Mechanismen
      * 1. Vereinigen von vielen Eingaben 
      * 2. eine nicht lineare interne Ausgabefunktion
    * Eingaben gewichtet
    * gewichtete Eingaben summiert (+ Bias)
    * -> kontinuierliches Mappen & Klassifizieren
    * Lernen = Anpassen von Weights und Bias
    * aneinanderhängen und Schichten aufbauen -> artifical neural network (ANN)
    * ein Input Layer
    * n Hidden Layer
    * ein Output Layer
  * Unsupervised Learning - Lernen ohne Labels [2] S. 218
    * Strukturen erkennen -> Beziehungen/Gruppierungen
    * Clustering
      * "einfachste Struktur" ([2] S. 218)
      * Cluster mit höherer internen Ähnlichkeiten
      * verschiedene Ähnlickeitsermittlungen (zB. Euklidische Distanz)
      * k-mean-Cluster -> zufällige Aufteilung von Punkten in einzelne Cluster -> die sich ähnlichsten Cluster zusammenfassen + neuer Durchschnittswert für weitere Rechnung -> Schritt 2 ...
    * Manifolding Learning
      * kein zwingendes Clustern
      * erstellen einer Metrik um Beziehungen darzustellen
      * Metrik notwendig für k-mean-Clustering
      * Metrik zB Euklidische Distanz
      * Metriken können unterschiedlich sein
    * Generative Modelle
      * Modelle, welche realistische Daten erstellen können
      * eine unterliegende, aber nicht beobachtbare Verteilung
      * explizites Dichtemodell schätzt diese zugrundeliegende Verteilung (Gaußschen Mischungsmodell (GMM))
      * implizites Dichtemodell: Beispiele ersetllen, welche nicht mehr von testdaten unterscheidbar sind
  * Reinforcement Learning [2] S. 221
    * keine Trainingsdaten notwendig
    * kreiert einge Trainingsdaten durch Interaktion mit Umfeld
    * Belohnung für gute Ergebnisse
    * Bestrafung für schlechte Ergebnisse
    * learning by doing
    * Agent = ein Individuum, ein Modell
    * Agent Bewegung in Zeitsteps
    * Agent hat Zustand und Aktionspalette
    * je nach Zustand muss eine Aktion ausgewählt werden
    * Neuer Zustand basiert auf Aktion und Umgebungseinfluss
    * Sammeln von Belohnungen um die größtmögliche Belohnung zu erhalten
    * Verhältnis exploration und exploitation
  * Neural Network (DL)
    * 2010 hoch -> Rechenpower + Graphikkarten eigenen sich gut, Verfügbare Daten, Algorithmen haben einen Durchbruch gehabt
    * CNN [2] S. 224f
      * Mehrschichtig
      * viele Verbindungen ausgelassen -> Filtern der Eingabe
      * häufiges Filtern und Gewichten
      * Filter werden über das gesamte Netz wiederverwendet
      * Nachbarschaft ist wichitg -> Input Filter nur zu wenigen anderen Verbunden
      * Reduktion der Möglichkeiten
      * Viele Schichten welche selbst simpel sind -> ähnlich zu Bagging 
    * Recurrent Neural Networks (RNN)
      * für sequenzielle Daten
      * Input + Hidden + Output
      * Eingabe + Aktueller Zustand des Netzwerkes = Ausgabe
      * gut für Kontext
      * Nutzen von Short-Term-Memory und Long-Term-Memory [2] S. 228f
        * nicht nur alten Status als Input
        * auch alten Output
        * auch aktuellen Input
        * alles in sich gewichtbar
    * Autoencoder
      * mehrerer Verschlüsselungsschichten (encoder-Layers)
      * Input wird zu niedrig Dimensionalen Repräsentation
      * Decoder "entschlüsselt" Repräsentation
      * Training = Differenz von Input und Entschlüsseltem Output minimieren
      * Fehlerfunktion während des Lernens anpassen (nicht nur beim Autoencoder)
    * Generative Adversarial Networks (GAN)
      * Generiert Daten ununterscheidbar von echten Daten
      * Input = sampling Vector
      * deconvolution & upscaling
      * Discriminator -> Versucht zu erkennen, was echt und was falsch ist (Benötigt echte und gefakte Trainingsdaten)
      * steigern sich beide
      * mode collapse -> nur noch wenige Beispiele 
      * Catch me if you can -> ein Beispiel solange bis es erkannt wird, dann nächstes Beispiel
      * mgl. statt korrekt und falsch -> einen Kritikwert
* Computer Vision[2] S. 317
  * Informationen aus Visuellen Daten erhalten
  * Analysierbar/bearbeitbar machen
  * Menschliche Sicht nachspielen
  * erkennen, verfolgen, Bewegungsanalyse, text erkennung
  * eng verwandt mit Image processing
    * Bildverbesserung
    * Bildkomprimierung
    * Merkmalserkennung
    * Bildverschmelzung
  * Kantenerkennung
    * Helligkeitsuneinheitlichkeiten
    * Unkontinuierlichkeiten in der Tiefe
    * Unkontinuierlichkeiten bei Oberflächen
    * Wechsel in Textur/Material
    * Beleuchtungsunterschiede
    * Search-Based -> Extrema der Intensität der Änderung (Ableitung) -> Gradienten
    * Zero-Crossing-Based -> Extram in Änderung + Wendepunkt der 2. Ableitung 
* Vertrauenswürdige AI [2] S. 519
  * Guidelines S. 520
    * OECD Principles of AI
      * Inclusive growth, sustainable development and well-being ([2] S. 521) -> Verbesserung menschlicher Fähigkeiten, Verringerung Ungleichheiten, UmweltSchutz
      * Human-centred values and fairness ([2] S. 521) -> Achten von Rechtsstaat, Menschenrechte, Freiheit, Würde, Autonomie, Privatsphäre, Datenschutz, Nichtdiskriminierung
      * Transparency and explainability ([2] S. 521) -> offenlegen von Infos, Nachvollziehbarkeit und Anfechtbarkeit von KI-Ergebnissen
      * Robustness, security and safety ([2] S. 521) -> Datensäzte, Entscheidungen, Prozesse Rückverfolgbar; IT-Sicherheit
      * Accountability ([2] S. 521) -> Entwickler + User sind verantwortlich für KI
    * UNESCO Recomondation of the Ethics of AI 
    * UNICEF Policy Guidance on AI for Children
    * EU HLEG Guidelines for Trustworthy AI
      * Human agency and oversight ([2] S. 521) -> Including fundamental rights, human agency, human oversight. 
      * Technical robustness and safety ([2] S. 521) -> Angriffsrobustheit, Ausweichpläne, Reproduzierbarkeit, Genauigkeit, Zuverlässigkeit
      * Privacy and data governance ([2] S. 521) -> Datenschutz, Datenqualität, Datenintegrität, Datenzugriff
      * Transparency ([2] S. 521) -> Nachverfolgbarkeit, Erklärbarkeit, Kommunikaiton
      * Diversity, non-discrimination and fairness ([2] S. 521) -> Verzerrung vermeiden, Zugriff, Universelles Design, Stakeholder-Teilhabe 
      * Societal and environmental wellbeing ([2] S. 521) -> Unweltschutz, Sozialer Einfluss, Nachhaltigkeit
      * Accountability ([2] S. 521) -> Verantwortungsaufteilung, Berichten negativer Ergebnisse 
    * EU White Paper on AI
  * Richtlinien
    * IEEE Ethically Aligned Design: https://ethicsinaction.ieee.org/#series
    * ISO/IEC Standards on AI and Trustworthy AI:https://www.iso.org/committee/6794475.html
    * NIST Standards for Trustworthy and Responsible AI: https://www.nist.gov/programs-projects/trustworthy-and-responsible-ai
    * CEN-CENELEC Committee on Artificial Intelligence: https://www.cencenelec.eu/areas-of-work/cen-cenelec-topics/artificial-intelligence/
  * Regulierungen
    *  EU Digital Strategy: https://ec.europa.eu/info/strategy/priorities-2019-2024/europe-fit-digital-age_en
    *  GDPR: https://ec.europa.eu/info/law/law-topic/data-protection/data-protection-eu_en
    *  DSA: https://ec.europa.eu/info/strategy/priorities-2019-2024/europe-fit-digital-age/digital-services-act-ensuring-safe-and-accountable-online-environment_en
    *  DMA: https://ec.europa.eu/info/strategy/priorities-2019-2024/europe-fit-digital-age/digital-markets-act-ensuring-fair-and-open-digital-markets_en
    *  EU Draft AI Act: https://digital-strategy.ec.europa.eu/en/policies/european-approach-artificial-intelligence
  * Transparenz [2] S. 533
    * Informationen über Training, genutzte Merkmale, Trainingsmethoden, Performance, ...
    * erhöhen der Transparenz/Verantwortungsverteilung
    * leichtere Reproduzierbarkeit
    * Biases leichter erkennbar
    * Dokumentation soll folgendes beantworten:
      * Why is the data being collected? Who requested/funded the data collection, and for what purpose?
      * What is the composition of the data set (for example, does it contain tabular data, or text data? Multi-modal data?)
      * How was the data collected? What sampling procedure, why was that method chosen, and sampled from which population?
      * Was the data labelled? If so, by whom?
      * What were the pre-processing steps?
      * What are the results of the Exploratory Data Analysis? (For example, how many items, how many features, correlations, sensitive characteristics, etc.)
      * What are the intended uses of this data set, and are there uses to avoid?
      * Will the data set be distributed? If so, how?
      * Who is repsonsible for the maintenance of the data set?
    * Model-Dokumentation
      * Basic logistic information about the model, such as person or organization developing it, licenses, and where to send questions or bug reports..
      * Basic descriptions of the training algorithms, the model parameters, optimization function, fairness constraints, and features.
      * Intended use, in particular optimal uses, primary intended users, and use cases to avoid.
      * Under which conditions – for example, using which target populations; if audio/visual input is required, which kind, and under what environmental conditions – the model performance has been tested.
      * Which metrics were used to measure model performance? Which fairness metrics? What decision thresholds were used?
      * Details on the training and test data (see Documenting the data section above)
    * Erklärbarkeit
      * Feature summary statistics: Merkmalsgewichtung, Beziehung Merkmal-Vorhersage
      * Feature summary visualization: Grafische Merkmals-Vorhersage-Beziehungs-Ausgabe
      * Model internals: Gewichtungen, Bäume, ...
*  Teilhaber [2] S. 524
  * Data provider -> Sammeln, Bearbeiten, Liefern von Daten
  * AI Provider
    * Management
    * "Legal department/Corporate responsibility department"
    * Datenschutz 
    * Systemarchitekt/Data Engineer
    * Entwickler
    * Quality
  * AI User
    * Management
    * "Legal department/Corporate responsibility department"
    * Qualität
    * Datenschutz
    * System Architekt
    * Menschliche Ressourcen
    * Beschaffung
    * direkte Nutzer/wegautomatisierte Arbeiter
  * AI Objekt -> Objekt, über welches Vorhersagen getroffen werden
  * Certifikation Body -> Bescheinigung eingehaltener Standarts
  * Regulator -> Leistungskritieren festlegen, 
  * "Broader society, including for example human rights organizations, consumer protection organizations, envirnomental protection organizations, and media" S. 525 
* Testspezifikation [10] S. 3
  * Enthält
     * Testentwurfsspezifikation
       * *Test design specification*
       * Verfeinerung
       * Merkmalsidentifikation
       * Funktionsidentifikation
       * Definition Erfolgreicher Testfälle/-abläufe
       * Bestanden wird pro Funktion definiert
     * Testfallspezifikation
       * *test case specification*
       * definition Eingabewerte
       * Definition Ausgabewerte
       * Beschreibung Vor- und Nachbedingungen, Ziele, Testaktionen
       * Priorität
       * Dauer
       * mgl. zurücksetzen des Systems
     * Testablaufspezifikation
       * *test procedure specification*
       * alle Schritte zur Durchführung
       * Voraussetzungen herstellen
* Testbericht [10] S. 4
  * Ergebnisse aller Testläufe in eine Version
  * *Testobjektübergabebericht*
    * tests item transmittal report
    * Beschreibung Übergabe der Testfälle
    * für getrennte Entwicklungs- und Teststeams
    * für offiziellen Start der Testphase
    * alle zu testenden Merkmale sind aufgelistet
  * *Testprotokoll*
    * test log
    * Chronologische Aufzeichnung während einer Testausführung
    * intensives Logging -> schlechte Antwortzeit (+ mgl. dadurch neue Fehler), hohe Datenmengen
  * *Testabweichungsbericht*
    * test incident report
    * alle Ereignisse, welche eine Nachprüfung benötigen
  * *Testabschlussbericht*
    * test summary report
    * Zusammenfassen der Testktivitäten
    * Schließt eine Teststufe ab
    * kann Einschränkungen für nächste Teststufe definieren -> nicht alle Fehler gefixed -> Parallel trotzdem Testen und Abweichungen feststellen
    * Bewertung des Testprozesses
    * Erfahrungbericht
  * *Statusbericht*
    * zeigt Zwischenstand
    * bei sehr großen Projekten mit langen Testphasen
    * Informationen im Voraus definieren
  *  fester Reporting-Rythmus
  *  best: Berichte Tagesaktuell
  *  oft weitere, individuelle Bericht (Testfortschrittsbericht, Teststufenbericht, ...)
* Teststrategie [10] S. 9
  * " eine Dokumentation, die die generischen Anforderungen an das Testen in einem oder mehreren Projekten innerhalb einer Organisation beschreibt, einschließlich der Details darüber, wie das Testen durchgeführt werden sol" [10] S. 9 
  * an *Testrichtlinie* ausgerichtet
    * "ein Dokument, in dem auf hohem Abstraktionsniveau die Prinzipien, der Ansatz und die wichtigsten Ziele einer Organisation in Bezug auf das Testen zusammenfasst" [10] S. 9f
    * für ganzes Unternehmen
    * Templates für Testdokumente
  * *Testkonzept*
    * Projekt beschreiben
    * Anforderungen referenzieren
    * Stakeholder
    * Teststufen
    * Termine
  * Intensivität der Teststufen
    * Abhängig von Budget, Risiko, Komplexität, Az. Teams
    * Abstimmung mit Projektleiter + Product Owner
  * Unternehmensabhängige Standartvorgaben
  * Testvoraussetzungen, Testplanung, Integrationsstrategie, Testumfang
  * Testumgebung, Testwerkzeug
  * Prüfung Testergebnisse, Freigabevorgaben
  * *Integrationsstrategie* [10] S. 13
    * Module erst einzeln testen 
    * Module haben verschiedene Testzeiten
    * Module teilweise erst in Umgebung korrekt testbar
    * Abschließend zusammenführen
    * mgl. Platzhalter (Mocks, Stubs) verwenden
    * Reihenfolge der Modulzusammenschließung
    * wichtigsten Module am Anfang
    * Eingabemodule vor Ausgabemodulen
    * Parallele Integration mgl.
  * *Tools* [10] S. 14
    * unternehmensweit einheitlich
    * definiert Testfallaufbau
      * (bsp)
      * Test-ID
      * Testobjekt
      * Testkonfiguration -> Konfiguration, Testumgebung, Vorschritte
      * Testbeschreibung -> genau!!, Beschreibung Testfall + Testprozedur, Schrittfolge
      * Priorität-> zwingend?, Regressionstestnotwendig, 
      * Referenzen -> Bezug Pflichtenheft + andere Testfälle, Matrix Anforderung-Testfall
      * Detailfelder/Kommentare für Ergänzungen
      * Soll-Ergebnis -> messbar formuliert, kein Interpretationsspielraum
      * Ist-Ergebnis
      * Ergebnisbewertung -> OK/NOK; IO/NIO
      * Fehlerreferenz
      * Kommentar zu Ergebnissen
      * Tester/Verantwortlicher
      * Timestamp
      * Testdauer
    * zu beantwortende Fragen [10] S. 15
      * Wozu ist das Projekt gut, was soll der Test bewirken?
      * Was wird gemessen und wie wird gesteuert? (Betrachtungsobjekt – Produkt/Prozess/Ressource/Rahmenbedingung)
      * Welche Aspekte gilt es zu berücksichtigen? (Führungsgrößen/Eigenschaften/Metriken)
      * Mit welchem Maß erfolgt die Messung? (Maßeinheit/Messgröße zur Messung der Ausprägung)
      * Welche Zielwerte werden verfolgt? (Ausgewählte Zielwerte)
      * Wie wird gemessen? (Messmethode)
      * Wann wird gemessen? (Zeitpunkt und Zeitraum der Messung)
      * Wo wird gemessen? (Ort/Stelle)
      * Wer führt die Messung durch? (Person/Gerät)
      * Wie werden die Messergebnisse dokumentiert? (Qualitätsdaten)
      * Wie werden Messergebnisse ausgewertet? (Vergleich gegen Zielwerte)
      * Welche Maßnahmen werden ggf. zur nachhaltigen Verringerung der Abweichung bzw. Streuungen ergriffen und wer kontrolliert deren Wirkung?
      * Welche Maßnahmen werden ggf. zur Vorbeugung ergriffen? 
    * Balenced Scorecard [10] S. 16
      * BSC
      * Instrument zur Steuerung der Umsetzung von Strategien
      * ca. 20 Ziele
      * Ziel monitär und nicht-monitär
      * Zielgrößen mit Sollwerte
      * "Strategische Aktionen" zur Zielerreichung
        * Terminvorgabe
        * Budgetvorgabe
        * Verantwortliche
      * Planung: Top-Down
      * Umsetzung: Bottom-Up
      * Perspektiven:
        * Finanz -> Ziele aus Erwägungen des Kapitalgebers
        * Kunden ->  Ziele für Struktur und Anforderungen unserer Kunden -> finanzielle Ziele erreichen
        * Prozess -> Ziele für Prozessqualität -> Ziele von Finanz- und Kundenperspektive erreichen
        * Potenzial -> Ziele, um aktuellen und zukünfitigen Herausforderungen gewachsen zu sein
      * Nutzen
        * Planung, Entwicklung, Umsetzung von Strategien
        * Leistungsvereinbarung für Führungskräfte
        * Strategieumsetzung überwachen
        * Präsentation bei Stakeholdern
      * Vorteile
        * richtet kritische Erfolgfaktoren auf Strategie aus
        * schneller Überblick
        * leicht verständlich
        * flexibel
      * Nachteile
        * kein umfassendes Strategieentwicklungstool -> nur Kennzahlen
        * zu ungenau für Kosten-Leistung-Rechnung
        * nicht alle Kennzahlen
* IAV [28]
  * übernimmt automatisiert die Erstellung von Testskripten aus manuellen Testbeschreibungen
  * Teil eines Modularen Baukastens
  * Automatierung nicht leicht -> Expertenwissen + Programmierkenntnisse
  * Permanente Testanpassungen
  * lernen aus bekannten Testfallbeschreibung-Skript-Tupels
  * Bestimmung vieler UI-Elemente aus Testbeschreibung
  * Problem: Tippfehler, Multi-Label, ...
  * Effizienz von Testern steigern, nicht ersetzen
* Symflower [29]
  * Integration in den Workflow
  * generierung "high-coverage" Unit-Tests
  * IDEs
    * IntelliJ
    * Visual Studio Code
    * Goland
    * Android Studio
    * CLI
  * Echtzeit Rückmeldungen
  * Languages
    * Go
    * Java
  * keine Integrations-/Systemstests
* applitools [30]
  * Visual AI
  * more Productive
  * higher Testcoverage
  * Support 50 SDK
  * Take Screenshot -> Vergleich nach Kontrolle, keine UI-Elemente mehr zugreifen
* Eggplant software [31]
  * verschiedene Bereiche
    * Performance [32]
    * ...
  * Nutzen des Digital Twin Sufaces [33]
    * Zustände und Aktionen
    * Übergänge
    * durch Modell
    * Alle Möglichen Pfade
  * optimieren der Performance
  * schnellere Tests
  * Verbindung Testen + Monitoring
  * Nutzer-Bewegungen analysieren
  * automatisches Erstellen eines Modelles der Webseite [31]
    * Interaktives Erstellen [33]
    * Model-Erstellung durch existierende Dateien (Gherkin) [33]
    * Model-Erstellung durch echte Kunden [33]
    * Intelligentes Anwendungsschaben (Durcharbeiten der Webseite) [33]
  * Intelligente Testplanung
  * Intelligent Computer Vision
    * verschiedene Browser/Geräte = verschiedene Ergebnisse
    * DOM-Modell
    * verschiedene Auflösung, Schriftgröße, Farben
    * Objekte im Laufe der Entwicklung verändert
    * Optical Character Extraction (OCE) -> vereinfachung automatisierten Testens
  * Universal Fusion Engine
    * identifies, executes and adapts test models automatically
  * API-Bewertung
    * Vergleich Frontendangaben mit Backend-Ausgaben
  * Jede Plattform
    * alle Browser
    * alle OS
    * alle Geräte
  * Model Based Testing
    * App-Verhaltensvorhersage
    * genauere/zuverlässigere Tests
  * CI/CD Integration Adapters
    * schnelleres Testfall erstellen
  * Performance Test [32]
    * Erstellen von Skripten
    * Auto-Generierungen von Skripten
      * Data Collection + Aufzeichnung
      * Szenario einmal durchspielen
      * Aufzeichnung Netzwerk (Sessions, Cookies, dynamic forms, asynchrone Kommunikation, mobile Endgeräte, Sicherheit => Probleme) 
    * Test-Ausführung -> Aufzeichnen der Performance/Anpassen von Parameter in Echtzeit
    * Workflow -> Az. User, Abfolge
    * mehr als 100 000 virtueller Nutzer mgl.
      * Nutzer durch Injektoren angelegt
      * Beliebig viele Injektoren
      * Injektoren in verschiedenen Ländern möglich
      * führen Eggplant (o.a. virtuell-User-Skripte) aus -> End-zu-End-Tests
  * AI [33]
    * Probleme Automatisiertes Testen
      * Tests brechen schnell
      * Wartung der Tests
      * Entwicklung der Tests (Zeitaufwand)
      * nur Teilweise "Autonom"
      * Regression-Test-Set
        * jedes Release
        * vergangene behobene Fehlverhalten kehren nicht zurück
      * Neue-Features-Test-Set
      * Test-Phase zu kurz -> welche Tests/Verzögerung -> erhöhtes Risiko
    * Daten konsumieren -> ML -> optimales Testset
    * verbessert Menschen statt ersetzen
    * vollautonome KI -> kein/wenig Kontext, keine Emotionen, kein Wissen
    * Matrix Autonomes Test-Ausführen (ex) <-> Autonomes Test-Auswählen (sel)
      * high ex - high sel
        * Auwahl Tests
        * vollständige Automatiserung von Testgenerierung bis Testausführung
        * geringe Kosten
        * umfangereiches Reporting
      * low ex - high sel
        * Auswahl Tests
        * wenige notwendige Testdaten
        * keine Testausführung
        * Weniger Tester-Input notwendig
        * Umfangreiche weitere Testautomatisierung notwendig -> hohe Wartungskosten
        * umfangreiches Reporting
      * low ex - low sel
        * "Identify weak areas to test"
        * keine Testauswahl
        * keine Testausführung -> weitere Testautomatisierung notwendig
        * viel manueller Input
        * hohe Wartungskosten
      * high ex - low sel
        * Identifizieren von Bereichen zum konzentrieren
        * wenige vorher bestimmte Tests
        * von Generierung bis Ausführung
        * Umfangreiche, automatische Reports 
    * Testauswahl
      * vorher definierte Tests
      * hilft Testsmanager
      * hoher Enwicklungsaufwand für Testgenerierung
    * Testausführung
      * benötigt Trainingsdaten
      * hilt Testengineer
      * Selbstheilende Tests
      * sehr Trainingsdatenbasiert
      * Risiko Fehler zu heilen
    * Automation Intelligence
      * Entscheidung welcher Applikationsbereich getestet werden muss
      * Input-Daten = Daten aus verschiedenen Algorithmen
      * Betrachten der 
        * Fehlerhistorie
        * Anwendungsänderungen
        * Testcoverage Historie
      * Erstellen der Tests
        * Aus Modell heraus
        * alle mgl. Pfade bekannt
        * Auswahl Regressionstests
        * "AI Bug Hunting" [33] Abb. S. 9
        * Testabdeckungsanalyse
        * Echte Nutzer Verhalten
        * Änderungs- und Fehlermonitoring
      * Ausführen der Tests
        * Digitaler Zwilling
        * Codeschnippsel für Übergänge
          * einfachere Wartung -> eine Änderung = Update vieler Scripts
          * schnellere Testfall-Generierung -> vielfälltige Tests, Entscheidungsbasierte Algorithmen
          * größere Flexibilität -> Wiederverwendbarkeit, 
        * Zusammensetzen der Schnippsel für Script
        * 
      * Report
      * braucht keine guten Trainingsdaten (clean)
      * keine schlechten Tests
      * robuste Tests
      * keine menschliche Eingabe
* Testen mit KI [13]
  * Produktqualität nach ISO2510
    * Funktionale Eignung
    * Leistungseffizients
    * Kompatibilität
    * Gebrauchstauglichkeit
    * Zuverlässigkeit
    * Informationssicherheit
    * Wartbarkeit
    * Übertragbarkeit
    * *Intelligentes Verhalten* -> Sogetis
      * Lernfähigkeit
        * mit Regeln
        * mit Daten und Deuten dieser
        * mit Imitieren von anderen
        * => Verstehen und Erfahrungen nutzen
      * Improvisation
        * Anpassung an neue Situationen
        * Schnelle Interpretation der Daten
        * Anpassen des eigenen Verhaltens
      * Transparenz
        * Nachvollziehbar durch Menschen
        * welche Datenpunkte sind entscheident
      * Zusammenarbeit
        * Mensch-Roboter-Interaktionen
        * Kommunikation
      * Natürliche Interaktion
        * Kommunikation
        * Art und Weise der Kommunikation
    * *Moral* -> Sogetis
      * gutes/schlechtes Verhalten
      * Asimovs Gesetze?
      * Ethik
        * nach Prinzipien handeln
        * Basis:
          * Gesetze
          * Regeln
          * Vorschriften
          * moralische Werte
      * Privatsphäre
        * Schutz der Privatsphäre
      * Freundlichkeit zu Menschen
        * Mensch kein Schaden zufügen
        * Vorteil für menschliche Gemeinschaft
    * *Persönlichkeit* -> Sogetis
      * Stimmung
        * Anpassung der Stimmung an die Umgebung
        * grundsätzlich positiv
      * Empathie
        * Emphatie simulieren
        * Emotionen erkennen + entsprechend reagieren
      * Humor
        * heitere Gelassenheit
        * erkennen von Humor
        * später Nutzen von Humor
      * Charisma
        * ? sehe ich persönlich nicht so
  * Nutzungsqualität nach ISO2510
    * Effektivität
    * Effizienz
    * Zufriedenheit
    * Risikofreiheit
    * Kontextabdeckung
  * Qualitätsmerkmale -> Kennzahlen -> Tests
  * Testen - Zeiträume
    * klassisches Testen - Monate
    * agiles Testen - Wochen
    * kontinuierliches Testen - Tage
    * Digitales Testen - Minuten
  * Testgenerierung durch evolutionäre Algorithmen
  * Durchführung
  * Überwachung
  * Prognose
    * Vorhersage von Fehlern/Fehlverhalten
    * Voraussetzungen:
      * Generierte Tests (Modelbased Testing, Digitaler Zwilling)
      * automatisierte Testausführung
      * Datensammlung in Echtzeit
    * viele Modelle -> viele Ergebnisse
    * Ergebnissmenge manuell Interpretieren
* KI Qualität [14]
  * echte Nutzer erschaffen Daten
  * hohe Diversität der Daten
    * Geschlecht
    * Nation
    * Alter
    * Ethnien
    * Kultur
    * politische Einstellung
    * ökonomische Merkmale
    * Bildungsniveau
    * weniger Bias
  * Suche nach Verzerrungen
* Symflower [15]
  * Autonomes Testen
    * -> höhere Qualität
    * -> Mitarbeiterentlastung
    * -> Kostenreduzierung
  * automatisierte Unit-Test-Erstellung
  * erstellte Tests -> aktuelle Funktion der Methoden
  * Regressionstests/Refactortests automatisch gegeben
  * bei neuen "push" in Reporitory
* AI im Software Tests [24]
  * Reduzierung Time2Market
  * besserers Automatisiertes Testen
  * mehr vollgetestete Software
  * 2 Testtypen
    * manuelles Testen
      * Tester selbst überprüft
      * keine extra Tools
    * Automatisiertes Testen
      * erstellen von Skripts
      * Software testet Software
  * Requirement Analysis -> Testplanning -> Test Development-> Test Execution -> Evaluation exit criteria -> Test Closure -> von vorn
  * Teststages:
    * development testing
      * Unit Tests -> Funktionalitätstest, Konzentration auf eine Funktion/Klasse
      * Component Tests -> Software-Einheiten zusammenführen und Testen, Fokus auf Komponenten-Interfaces
      * System Tests -> Zusammenführung Software verschiedener Teams
    * Release Testing
      * Requirement Testing -> für jede Vorgabe => Testfall
      * Scenario Testing -> Nutzerverhalten nachstellen und Testfälle entsprechend generieren
      * Performance Testing -> Vorgegebene Last aushalten
    * User Testing
      * Apha Testing -> Tests in der Testumgebung
      * Beta Testing -> Tests in der Nutzerumgebung
      * Acceptance Testing -> Tests durch Nutzer
  * Vereinfachung -> schnellere Testfallgenerierung
  * Kategorien von ML
    * Arbeitsweise
    * Mathematische/statistische Modelle
    * Annahmen
    * Characteristiken
    * Genauigkeit
    * Lösungskategorien
  * MELBA
    * MachinE Learning based on BlAckbox test specification
    * ML basierend auf Blackbox Testspezifikationen
    * teilautomatisiierter, iterativer Algorithmus basierend auf C4.5 {? was ist C4.5}
    * C4.5 generiert Entscheidungsbäume
    * höhere Fehlererkennung
    * leicht höherer Testfälle
    * [[4]]
  * Merkmalsextraktion für Modellgenerierung
    * welche Merkmale sind wichtig
    * Daten von automatisierten Tools
    * SVR (Algorithmus) ist genauste
    * [[5]]
  * GUI Testing mit AI
    * HGA (hybrid genetic Algorithm)
    * Optimierung: Test-Sequenz-Optimierung + Testfall-Optimierung
    * [[6,7]]
  * Testfallklassifizierung
    * k-means Clustering
    * Statement Coverage Criterion -> am wichtigsten
  * Testfall-Durchführbarkeit vorhersagbar [[10]]
  * Änderungsanfälligkeit vorhersagen
    * [[13]]