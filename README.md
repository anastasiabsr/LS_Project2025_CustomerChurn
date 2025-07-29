
# 📊 Telco Customer Churn – Machine Learning Projekt

Dieses Projekt untersucht das **Kündigungsverhalten von Kunden** eines fiktiven Telekommunikationsunternehmens mit Hilfe von **überwachten und unüberwachten Lernverfahren**.  
Ziel ist es, sowohl **Vorhersagen über Kundenabwanderung (Churn)** zu treffen als auch **Kundengruppen (Cluster)** zu identifizieren, um strategische Entscheidungen zu unterstützen.

---

## 🧠 Inhalt des Projekts

| Datei                              | Beschreibung                                      |
|-----------------------------------|--------------------------------------------------|
| `logistic_regression.ipynb`       | Churn-Vorhersage mit logistischer Regression     |
| `gradient_boosting.ipynb`         | Churn-Vorhersage mit Gradient Boosting           |
| `svm.ipynb`                        | Churn-Vorhersage mit Support Vector Machine      |
| `knn.ipynb`                        | Churn-Vorhersage mit k-Nearest Neighbors         |
| `neural_network.ipynb`            | Churn-Vorhersage mit einem neuronalen Netz       |
| `unsupervised_clustering.ipynb`   | Kundenclustering mit K-Means + Erweiterungen     |
| `requirements.txt`                | Liste der benötigten Python-Bibliotheken         |
| `README.md`                       | Projektbeschreibung                              |

---

## 🔍 Ziel

### 1. Überwachtes Lernen:
- Klassifiziere Kunden in "Churn" oder "Kein Churn"
- Vergleiche mehrere ML-Modelle hinsichtlich Genauigkeit, Precision, Recall und F1-Score

### 2. Unüberwachtes Lernen:
- Segmentiere Kunden anhand ihres Nutzungsverhaltens
- Identifiziere Gruppen mit hohem Kündigungsrisiko ohne Labels
- Nutze Clustering zur späteren Interpretation oder gezielten Kundenansprache

---

## 🧪 Datensatz

- 📄 **Name:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`  
- 🗂️ Quelle: [Kaggle – Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  
- 📦 Enthält:
  - Vertragsdetails (Vertragsdauer, monatliche Gebühren, Internetdienste …)
  - Kundenstatus (Churn ja/nein)
  - Persönliche Angaben (z. B. Geschlecht, Senior)

---

## 🛠️ Installation & Setup

### 1. 🔧 Python-Umgebung vorbereiten

Stelle sicher, dass du **Python 3.10 oder höher** installiert hast.

Dann:

\`\`\`bash
# Virtuelle Umgebung (optional, empfohlen)
python -m venv venv
source venv/bin/activate  # oder venv\Scripts\activate auf Windows

# Benötigte Pakete installieren
pip install -r requirements.txt
\`\`\`

### 2. 📂 Daten
Lege die Datei `WA_Fn-UseC_-Telco-Customer-Churn.csv` im selben Verzeichnis wie die Notebooks ab.

---

## 🚀 Nutzung

1. **Starte JupyterLab**:
   \`\`\`bash
   jupyter lab
   \`\`\`

2. **Öffne nacheinander folgende Notebooks**, z. B.:
   - `logistic_regression.ipynb` zur Churn-Vorhersage mit klassischem ML
   - `unsupervised_clustering.ipynb` zur Analyse von Kundenclustern

3. **Modelliere**, **interpretiere** und **vergleiche** die Ergebnisse – insbesondere:
   - Welche Merkmale beeinflussen Churn?
   - Gibt es klare Cluster?
   - Welche Modelle liefern die besten Vorhersagen?

---

## 📈 Beispiel-Ergebnisse

- **Bestes Modell:** Gradient Boosting oder Neuronales Netz (abhängig von Metriken)
- **Clustering-Erkenntnis:** Kunden mit „Month-to-month“-Verträgen und hohen Gebühren sind häufiger im „Churn“-Cluster
- **Silhouette Score:** ~0.17 bei K-Means → Potenzial für bessere Methoden (z. B. DBSCAN)

---

## ✅ Nächste Schritte / Erweiterungen

- Hyperparameter-Optimierung (GridSearch)
- Feature Selection & One-Hot-Encoding
- Weitere Clusterverfahren: DBSCAN, GMM, Hierarchisch
- Deployment z. B. via Streamlit oder Flask

---

## 🤝 Lizenz / Verwendung

Dieses Projekt ist ein **universitäres Lernprojekt**. Datennutzung gemäß [Kaggle-Lizenzbedingungen](https://www.kaggle.com/datasets/blastchar/telco-customer-churn).
