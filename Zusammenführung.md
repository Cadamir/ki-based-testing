# Datensammlung

1. Einleitung
2. Traditonelle Teststrategien
3. Probleme traditioneller Strategien
4. KI-Basiertes Testen als Ansatz
5. Verschiedene nutzbare KI-Modelle
6. Marktschau
7. Tools theoretisch darstellen
8. Umsetzung/Einführung eines Testframeworks für Java/Angular
9. Auf Umsetzung basierende Bewertung
10. Fazit
11. Literaturverzeichnis

## Einleitung
Grund für die Arbeit
* Testen oft vernachlässigt
* Entlassten der Entwickler
* Erhöhen der Qualität

Grundsätzliche Idee
* KI erstellt Tests
* KI erstellt Testfälle
* Entwickler erstellt keine/wenige Tests

Aufgabenstellung/Zielsetzung:
* Überblick über den Einsatz von KIs für Testen geben
* Darstellen, wie KIs Testfälle erstellen können
* Darstellen, welche Tools wie engesetzt werden könnten mit "proof-of-concept"

Aufbau der Arbeit
* Traditionell
* KI-basiert
* Marktschau

## Traditionelle Teststrategien
### Themen
* Was ist Testen
* Warum Testen
* kurzer historischer Abriss
* Testfallgenerierung
* Darstellen der wichtigsten Teststrategien
* Testmetriken
* Probleme traditioneller Teststrategien

### Daten
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

## KI-basierter Testansatz
### Themen
* Grundidee
* Welche Arten gibt es?
* Welche Einsatzzwecke gibt es?
* Welche Vorteile/Schwächen weisen die KIs auf

### Daten
* Testen mit KI
   * GUI analysieren
   * Testfälle abschätzen, 
   * Automatische Wartung einiger Skripte
   * Optische Veränderungen aufzeigen
   * Testberichte
   * Auswahl und Priorisierung von Regressionstestfällen
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

## verschiedene nutzbare KI-Modelle
### Themen
* Verschiedene Arten von KIs
* vermutlich Neuronale Netze und Deep Learning oder eben auch nicht
* Trainingsmethoden
* Eingabeparameter

### Daten
* Was ist künstliche Intelligenz [1/1]
   * "die Lehre der Automatisierung intelligenten Verahltens, sowie des maschinellens Lernens" ([1/1] - "Künstliche Intelligenz - was bedeutete das eigentlich?")
   * stark vs schwach
   * starke noch nicht ernsthaft vorhanden
   * schwach imitiert Intelligenz basierend auf Regeln
   * Muster/Gesetzmäßigkeiten erkennen/verallgemeinern
   * Arbeitet mit Wahrscheinlickeiten [1/3]
   * KI macht aus Daten Informationen und aus Informationen Wissen [1/3]
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

## Marktschau
* Verschiedene Tools raussuchen
* Demos erhalten und bewerten
* Theoretische Grundlagen zum Tool darstellen
* Vorteile/Nachteile herausfiltern
* Einsatzmöglichkeiten aufzeigen
* Tool(s) für Java raussuchen/entscheiden -> Proof-of-Concept
* Tool(s) für Angular raussuchen/entscheiden -> Proof-of-Concept
* Bewertung/Beurteilung der aktuellen Marktlage
* Weiterentwicklungsaussichten

1. test.ai -> https://test.ai/all-products
2. mabl -> https://www.mabl.com/
3. IAV -> https://www.iav.com/was-uns-bewegt/mit-kuenstlicher-intelligenz-softwaretests-schneller-automatisieren/
4. symflower -> https://symflower.com/en/
5. applitools -> https://applitools.com/


## Fazit
* Zusammenfassen
* Fazit ziehen
* Ausblicke geben

## Literaturverzeichnis

|Quellnummer|Autor|Erscheinungs-datum|Titel|Themen-bereich|Link/Quelle|Downloaded|Durchgearbeitet|
|-|-|-|-|-|-|-|-|
|[1]|SwissQ|-|KI-unterstütztes Testen: Mythen und Fakten zur künstlichen Intelligenz|Allgemein| https://swissq.it/news/ki-unterstuetztes-testen-mythen-und-fakten-zur-kuenstlichen-intelligenz/ [1/1]-  https://swissq.it/management/ki-gesteuerte-software-und-systeme-im-taeglichen-einsatz-teil-2-von-5/ [1/2]- https://swissq.it/news/software-testing-mit-kuenstlicher-intelligenz-eine-marktbetrachtung-teil-3-von-5/ [1/3] - https://swissq.it/testing/ki-gesteuerte-software-meets-testing-etwas-ganz-neues-oder-business-as-usual-teil-4-von-5/ [1/4] - https://swissq.it/testing/ki-gesteuerte-software-testing-gegen-bias-und-drift/ [1/5]
|[2]|Papp, Stefan & Weidinger, Wolfgang & Munro, Katherine|2022|The handbook of data science and AI : generate value from data with machine learning and data analytics|KI|DHBW UniBibo / https://www.hanser-elibrary.com/doi/book/10.3139/9781569908877|
|[3]|Stanislas Chaillou|2022|Artificial intelligence and architecture : from research to practice|KI| DHBW UniBibo / https://www.degruyter.com/document/doi/10.1515/9783035624045/html |yes|no|
|[4]|Umberto Michelucci|2022|Applied Deep Learning with TensorFlow 2 : Learn to Implement Advanced Deep Learning Techniques with Python|KI|DHBW UniBibo / https://link.springer.com/book/10.1007/978-1-4842-8020-1 |yes|no|
|[5]|Matthieu Deru & Alassane Ndiaye|2020|Deep Learning mit TensorFlow, Keras und TensorFlow.js|KI|Zuhause|
|[6] - Vielleicht|Ian Goodfellow, Yoshua Bengio und Aaron Courville|2018|Deep Learning Das umfassende Handbuch|KI|- (noch nicht gefunden)|
|[7]| Francois Chollet|2018|Deep Learning mit Python und Keras: Das Praxis-Handbuch vom Entwickler der Keras-Bibliothek|KI|- (nur empfohlen, nicht online gefunden bisher)|
|[8]|Peter Liggesmeyer|2. Aufl. 2009|Software-Qualität : Testen, Analysieren und Verifizieren von Software|Test|DHBW UniBibo / DNB|yes|no|
|[9]|Baumgartner, Manfred &Gwihs, Stefan & Seidl, Richard & Steirer, Thomas & Wendland, Marc-Florian|3., aktualisierte und überarbeitete Auflage 2021| 	Basiswissen Testautomatisierung : Aus- und Weiterbildung zum ISTQB Advanced Level Specialist – Certified Test Automation Engineer | Test | DNB |
|[10]|Witte, Frank|2020| Strategie, Planung und Organisation von Testprozessen : Basis für erfolgreiche Projektabwicklung im Softwaretest|Test/bisschen KI|DNB|yes|no|
|[11]|Stephan Kleuker|2019|Qualitätssicherung durch Softwaretests : Vorgehensweisen und Werkzeuge zum Testen von Java-Programmen | Test  | DNB|yes|no
|[12]|Witte, Frank|2018| 	Metriken für das Testreporting : Analyse und Reporting für wirkungsvolles Testmanagement | Test | DNB|yes|no
|[13]|Rik Marselis|? (min. 2018)|Testen von und mit KI|Test/KI|https://www.sigs-datacom.de/trendletter/2020-18/8-testen-von-und-mit-ki|
|[14]|it-daily.net|2019|Neue Testing-Methode für Künstliche Intelligenz|Test/KI|https://www.it-daily.net/it-management/business-software/neue-testing-methode-fuer-kuenstliche-intelligenz|
|[15]| Dipl. -Ing. Thomas Drilling / Stephan Augsten|2021|Qualitätssicherung mit Unit und Behaviour Testing Automatisierte Software-Tests mit KI |Test/KI|https://www.dev-insider.de/automatisierte-software-tests-mit-ki-a-1009622/|
|[16]|Hussam Hourani; Ahmad Hammad; Mohammad Lafi|2019|The Impact of Artificial Intelligence on Software Testing|Test/KI|https://ieeexplore.ieee.org/abstract/document/8717439|
|[17]|Josip Bozic; Oliver A. Tazl; Franz Wotawa|2019|Chatbot Testing Using AI Planning|Test/KI/Example| https://ieeexplore.ieee.org/abstract/document/8718222 |
|[18]|Witte, Frank|2016 |Testmanagement und Softwaretest Theoretische Grundlagen und praktische Umsetzung| Test|Uni|yes|
