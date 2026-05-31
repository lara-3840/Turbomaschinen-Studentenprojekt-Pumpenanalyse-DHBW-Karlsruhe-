# Turbomaschinen-Studentenprojekt
In diesem Repository sind alle Dateien zur Abgabe des Studentenprojekts enthalten. Hierbei wird eine Wasserpumpe untersucht. Dies erfolgt auf Basis eines gegebenen Pumpendatenblatts sowie einer csv-Datei mit den gemessenen volumetrischen Durchflussraten. Zur Erstellung des Codes wurde Jupyter Notebook verwendet.

## Fünfstelliger Code für Bewertung:
03840

## Kursbezeichnung:
TMB23PT DHBW Karlsruhe

## Vorgehensweise
1. Bibliotheken laden (pandas, numpy, matplotlib, interp1d)
2. csv-Datei einlesen
3. Physikalische Konstanten festlegen
4. Arrays erstellen durch Ablesen der Kennlinienpunkte aus Pumpendatenblatt
5. Interpolationen erzeugen aus den Arrays
6. Berechnung zeitspezifischer Betriebswerte
7. Berechnung hydraulischer Nutzleistung und Wirkungsgrad
8. Lösung Aufgabe 1: Berechnung Energieverbrauch
9. Lösung Aufgabe 2: Ermitteln des durchschnittlichen Pumpenwirkungsgrads
10. Lösung Aufgabe 3: Berechnung der ungenutzten Energie
11. Wirtschaftlichkeitsanalyse und Betriebspunkt-Auswertung
12. Glättung der Daten
13. Formatierte Ausgabe der Ergebnisse
14. Lösung Aufgabe 4: Erstellung von Diagrammen
    - Leistung vs. Zeit Vergleich (Rohdaten und geglättet)
    - Histogramm zur Verteilung des Wirkungsgrads
    - Analyse des Betriebsverhalten anhand eines Histogramms der Verlustleistungen und eines Boxplots

Die genauen Vorgehensweise wird im Jupyter Notebook-Code mit Kommentaren erleäutert.

## Dateien
* `Zusatzaufgabe_Lara_Adam.ipynb` $\rightarrow$ Das fertige Jupyter Notebook mit Code, Kommentaren und Diagrammen
* `volume_flow_data.csv` $\rightarrow$ Der zugrundeliegende Datensatz (Volumenstrom-Zeitreihe)
* `README.md` $\rightarrow$ Projektbeschreibung
* `Pumpendatenblatt.pdf` $\rightarrow$ Pumpendatenblatt
