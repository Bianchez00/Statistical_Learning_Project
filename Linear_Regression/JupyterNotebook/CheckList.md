# Vehicle Price Regression Project – Checklist ✅

Questo progetto è organizzato in tre notebook principali:
1. `01_vehicle_data_cleaning.ipynb`
2. `02_vehicle_regression_model.ipynb`
3. `03_vehicle_model_interpretation.ipynb`

---

## 📓 01_vehicle_data_cleaning.ipynb
**Obiettivo**: preparare i dati per la modellazione.

- [ ] Importare il dataset originale `vehicles.csv`
- [ ] Esplorare la struttura (`df.head()`, `df.info()`, `df.describe()`)
- [ ] Analizzare valori mancanti (`df.isna().sum()`)
- [ ] Gestire i missing (imputazione o rimozione)
- [ ] Identificare e trattare outlier (es. prezzi anomali, odometer estremi)
- [ ] Definire target (`price`) e features (numeriche/categoriche)
- [ ] Salvare dataset pulito (`vehicles_clean.csv`)

---

## 📓 02_vehicle_regression_model.ipynb
**Obiettivo**: costruire e valutare il modello di regressione.

- [ ] Caricare `vehicles_clean.csv`
- [ ] Separare `X` (features) e `y` (target)
- [ ] Valutare se applicare log-transform a `y` (`log(price)`)
- [ ] Suddividere train/test set
- [ ] Creare una pipeline di preprocessing:
  - [ ] `StandardScaler` per variabili numeriche
  - [ ] `OneHotEncoder` per variabili categoriche
- [ ] Addestrare modello base (`LinearRegression`)
- [ ] Valutare performance su test set (RMSE, MAE, R²)
- [ ] Provare Ridge e Lasso con `GridSearchCV`
- [ ] Salvare il modello migliore o i suoi coefficienti

---

## 📓 03_vehicle_model_interpretation.ipynb
**Obiettivo**: interpretare e comunicare i risultati.

- [ ] Estrarre i coefficienti dal modello
- [ ] Ordinare le feature per importanza
- [ ] Interpretare i coefficienti:
  - [ ] Effetto unitario (numeriche)
  - [ ] Effetto % (se log-transform)
  - [ ] Effetto rispetto alla baseline (categoriche)
- [ ] Analizzare i residui:
  - [ ] Distribuzione dei residui
  - [ ] Residui vs valori predetti
  - [ ] Eventuali pattern di eteroschedasticità
- [ ] Creare grafici di supporto (barplot coeff., residui, QQ-plot)
- [ ] Scrivere mini-report:
  - [ ] Sintesi performance modello
  - [ ] Feature più influenti
  - [ ] Limiti del modello
  - [ ] Possibili sviluppi futuri

---

## 🚀 Prossimi passi
- [ ] Integrare ulteriori feature (es. chilometraggio annuo, marca premium vs non premium)
- [ ] Provare modelli non lineari (es. Random Forest, Gradient Boosting)
- [ ] Creare una presentazione o un report finale con risultati chiave
