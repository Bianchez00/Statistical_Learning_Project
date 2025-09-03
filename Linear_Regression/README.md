# Vehicle Price Regression Project 🚗📊

## 🎯 Obiettivo
L’obiettivo del progetto è sviluppare un modello di **regressione lineare** per stimare il prezzo dei veicoli in base alle loro caratteristiche (es. anno, chilometraggio, alimentazione, marca, ecc.).

Il progetto è pensato come esercizio pratico di:
- **Pulizia dati (EDA & cleaning)**
- **Modellazione e validazione (Linear, Ridge, Lasso)**
- **Interpretazione dei coefficienti**
- **Creazione di un mini-report con risultati e limiti**

---

## 📂 Struttura delle cartelle

```bash
├── Dataset/
│   ├── car_data.csv
│   ├── Car details v3.csv
│   ├── car details v4.csv
│   ├── CAR DETAILS FROM CAR DEKHO.csv
│   └── vehicles_clean.csv   # dataset pronto per la modellazione
│
├── JupyterNotebook/
│   ├── 01_vehicle_eda_cleaning.ipynb
│   ├── 02_vehicle_regression_model.ipynb
│   └── 03_vehicle_model_interpretation.ipynb
│
├── output/
│   └── results/
│       ├── coef_table.csv
│       ├── residuals.png
│       ├── model_performance.json
│       └── report_regression.md
│
├── CheckList.md
└── README.md

```
---

## 📝 Workflow
1. **EDA + Cleaning** (`01_vehicle_eda_cleaning.ipynb`)
   - Esplorazione del dataset
   - Analisi valori mancanti e outlier
   - Pulizia dati e salvataggio `vehicles_clean.csv`

2. **Modeling** (`02_vehicle_regression_model.ipynb`)
   - Preprocessing (scaling numeriche, encoding categoriche)
   - Regressione lineare base
   - Valutazione performance (RMSE, MAE, R²)
   - Regolarizzazione (Ridge, Lasso)

3. **Interpretation** (`03_vehicle_model_interpretation.ipynb`)
   - Analisi dei coefficienti
   - Grafici diagnostici dei residui
   - Report sintetico dei risultati

---

## 🚀 Requisiti
- Python 3.9+
- Librerie principali:
  ```bash
  pip install -r requirements.txt