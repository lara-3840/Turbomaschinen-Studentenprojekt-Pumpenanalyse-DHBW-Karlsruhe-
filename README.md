# Turbomaschinen-Studentenprojekt
In diesem Repository sind alle Dateien zur Abgabe des Studentenprojekts enthalten. Hierbei wird eine Wasserpumpe untersucht. Dies erfolgt auf Basis eines gegebenen Pumpendatenblatts sowie einer csv-Datei mit den gemessenen volumetrischen Durchflussraten.

## Fünfstelliger Code für Bewertung:
03840

## Kursbezeichnung:
TMB23PT DHBW Karlsruhe

## Projektbeschreibung
Dieses Repository enthält die Analyse des Betriebsverhaltens einer Kreiselpumpe auf Basis von zeitreihenbasierten Volumenstrom-Messdaten und einem zugehörigen Pumpendatenblatt.

## Projektübersicht
Das Ziel dieses Projekts ist es, die Betriebsdaten einer Pumpe über einen Messzeitraum von 24 Stunden numerisch zu analysieren, Kennlinien zu interpolieren und energetische sowie wirtschaftliche Kennzahlen zu berechnen.

### Analysierte Aufgabenstellungen:
1. **Berechnung des Energieverbrauchs:** Ermittlung des elektrischen Gesamtenergieverbrauchs (inkl. Motor) sowie des Energieverbrauchs direkt an der Pumpenwelle in Kilowattstunden (kWh).
2. **Ermittlung des durchschnittlichen Wirkungsgrads:** Berechnung des arithmetischen Mittels des Pumpenwirkungsgrads sowie des Gesamtwirkungsgrads im Betrieb.
3. **Berechnung der ungenutzten Energie (Verlustleistung):** Quantifizierung der Verlustenergie der Pumpe und des Gesamtsystems durch Gegenüberstellung von aufgewendeter Energie und sinnvoll genutzter hydraulischer Nutzleistung.
4. **Wirtschaftlichkeits- & Betriebspunkt-Analyse:** Berechnung der finanziellen Verluste basierend auf dem Strompreis und Untersuchung der Abweichung vom optimalen Betriebspunkt (*Best Efficiency Point*, BEP).

---

## Technische Parameter & Rahmenbedingungen
Folgende physikalische Konstanten und Spezifikationen aus dem Pumpendatenblatt wurden für die Berechnungen herangezogen:
* **Laufraddurchmesser ($d$):** $269\text{ mm}$ (entsprechende Kennlinie auf S. 3 des Datenblatts)
* **Dichte des Mediums ($\rho_{fluid}$):** $1033\text{ kg/m}^3$
* **Erdbeschleunigung ($g$):** $9.81\text{ m/s}^2$
* **Motorwirkungsgrad ($\eta_{motor}$):** $93.6\,\%$ ($0.936$)
* **Optimaler Betriebspunkt (BEP):** $400\text{ m}^3\text{/h}$ bei einem maximalen Wirkungsgrad von $80.0\,\%$

---

## Wichtigste Ergebnisse der Analyse
Die Berechnungen im Jupyter Notebook liefern für den Messzeitraum (**01.04.2024, 00:00 Uhr bis 23:59 Uhr**) folgende Ergebnisse:

* **Betriebswerte im Mittel:**
  * Mittlerer Volumenstrom: **$253.39\text{ m}^3\text{/h}$**
  * Mittlere Förderhöhe: **$19.76\text{ m}$**
* **Energieverbrauch (Aufgabe 1):**
  * Elektrischer Energieverbrauch (Gesamtsystem): **$501.82\text{ kWh}$**
  * Energieverbrauch an der Pumpenwelle: **$469.70\text{ kWh}$**
* **Wirkungsgrade (Aufgabe 2):**
  * Durchschnittlicher Pumpenwirkungsgrad: **$67.53\,\%$**
  * Durchschnittlicher Gesamtwirkungsgrad (inkl. Motor): **$64.15\,\%$**
* **Energieverluste (Aufgabe 3):**
  * Sinnvoll genutzte hydraulische Energie: **$327.95\text{ kWh}$**
  * Ungenutzte Energie (Verlust nur Pumpe): **$141.75\text{ kWh}$**
  * Ungenutzte Energie (Gesamtverlust inkl. Motor): **$173.87\text{ kWh}$**
* **Wirtschaftlichkeit:**
  * Finanzielle Verluste im Betrieb: **$60.85\text{ €}$** (basierend auf dem im Code hinterlegten Strompreis)

---

## Verzeichnisstruktur
Das Repository ist wie folgt aufgebaut:
```text
├── Zusatzaufgabe_Lara_Adam.ipynb  # Das fertige Jupyter Notebook mit Code, Kommentaren und Diagrammen
├── volume_flow_data.csv          # Der zugrundeliegende Datensatz (Volumenstrom-Zeitreihe)
└── README.md                     # Diese Dokumentation
