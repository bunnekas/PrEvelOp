# PrEvelOp

**PrEvelOp** – *Production – Development – Optimization*  
Ein modulares Python-Framework zur **automatisierten Datenaufbereitung, explorativen Analyse, Clusterbildung und Evaluierung**, speziell für gemischte Datentypen wie geometrische und prozessbezogene Merkmale in der Fertigung.  
Projektlaufzeit: 2023–2025 | FIR e.V. & WZL an der RWTH Aachen  

🔗 Offizielle Projektseite: [https://www.fir.rwth-aachen.de/forschung/forschungsprojekte/detail/prevelop-22649-n](https://www.fir.rwth-aachen.de/forschung/forschungsprojekte/detail/prevelop-22649-n)

---

## Hintergrund

Produktlebenszyklen werden kürzer, die Nachfrage nach kundenindividuellen Produkten steigt.  
Dies führt zu **steigender Produkt- und Prozessvielfalt** – der sogenannten *Fertigungsprogrammvarianz*.  
PrEvelOp adressiert dieses Problem durch datenbasierte Verfahren des **Unsupervised Learning** und unterstützt KMU dabei:

- Transparenz über Produkt- und Prozessvielfalt zu schaffen  
- Potenziale zur Standardisierung und Segmentierung zu identifizieren  
- Maßnahmen zur Reduzierung von Komplexitätskosten abzuleiten  

Die Ergebnisse wurden im Rahmen des IGF-Vorhabens 22649 N entwickelt und als **Open-Source-Bibliothek** bereitgestellt.

---

## Features

- **Datenaufbereitung (`preparation.py`)**  
  - Bereinigung, Normalisierung, Encoding & Umgang mit fehlenden Werten  
- **Explorative Datenanalyse (`exploration.py`)**  
  - Boxplots, Heatmaps, Pairplots, Isolation Forests u.v.m.  
- **Clustering (`clustering.py`)**  
  - Agglomeratives Clustering, K-Medoids, HDBSCAN, inkl. Silhouette- und DBI/CH/Dunn-Metriken  
- **Evaluierung (`evaluation.py`)**  
  - Feature-Importance (Random Forest), t-SNE/PCA für Visualisierung, Validierung der Clusterqualität  
- **Demo-Frontend**  
  - Vue.js + FastAPI Schnittstellen (lokale Nutzung via Electron), Visualisierung von Clustern & KPIs  

---

## Installation

### 1. Repository klonen

```bash
git clone <repository-url>
cd prevelop
```

### 2. Virtuelle Umgebung einrichten
```bash
python3 -m venv prevelop-env
source prevelop-env/bin/activate  # Linux/Mac
prevelop-env\Scripts\activate     # Windows
```

### 3. Abhängigkeiten installieren
```bash
pip install -r requirements.txt
```

### 4. Entwicklungsmodus aktivieren
```bash
pip install -e .
```

### 5. Testen
```bash
import prevelop
print(prevelop.__version__)
```

## Projektpartner
- FIR e.V. an der RWTH Aachen
- Werkzeugmaschinenlabor WZL

## Lizenz & Nutzung
Die Software wird als Open-Source-Bibliothek veröffentlicht.
Sie richtet sich insbesondere an kleine und mittelständische Unternehmen (KMU), die Methoden des maschinellen Lernens mit geringen Einstiegshürden nutzen möchten.

*Gefördert im Rahmen des IGF-Vorhabens 22649 N. Entwickelt am FIR e.V. & WZL der RWTH Aachen.*