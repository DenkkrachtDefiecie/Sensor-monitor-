# Sensor Data Analyse Tool

Python-programma dat sensormetingen simuleert, analyseert met NumPy en visualiseert met Matplotlib.

## Functionaliteit

- Genereert gesimuleerde metingen met `random` (reproduceerbaar via een seed, standaard 42).
- Of laadt bestaande metingen uit een CSV-bestand.
- Berekent aantal, gemiddelde, minimum, maximum, standaardafwijking en het aantal metingen boven de drempel.
- Toont de metingen die de drempel overschrijden.
- Maakt een lijngrafiek (met drempellijn) en een histogram; beide worden getoond en opgeslagen als PNG.
- Slaat gegenereerde metingen op als CSV (`sample`, `reading`, `sensor_type`).
- Vangt ongeldige invoer en bestandsfouten af met duidelijke foutmeldingen.

## Installatie

Vereist Python 3.10 of nieuwer.

```bash
pip install -r requirements.txt
```

## Gebruik

```bash
python sensor_monitor.py
```

Kies `1` om nieuwe metingen te genereren of `2` om een bestaand CSV-bestand in te laden.

## Uitvoerbestanden

- `<sensortype>_readings.csv` (alleen bij optie 1)
- `readings_line_plot.png`
- `readings_histogram.png`
