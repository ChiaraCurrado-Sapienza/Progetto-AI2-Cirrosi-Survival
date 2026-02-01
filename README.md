# Analisi Predittiva della Sopravvivenza: Cirrhosis Patient Survival

## Descrizione del Progetto
Questo progetto si occupa dello sviluppo di un modello di apprendimento supervisionato per la **classificazione binaria** applicata all'ambito medico. L'obiettivo principale è predire la mortalità dei pazienti affetti da **Cirrosi Biliare Primitiva**, basandosi su un dataset reale fornito dalla Mayo Clinic.

Il lavoro segue l'intero flusso di una pipeline di Data Science:
1. **Analisi Esplorativa dei Dati (EDA)**: Identificazione di sbilanciamenti, outlier e correlazioni tra i parametri biochimici.
2. **Preprocessing**: Gestione dei valori mancanti tramite imputazione, codifica delle variabili categoriche (One-Hot Encoding) e standardizzazione delle feature numeriche.
3. **Modellazione**: Implementazione di un modello di Regressione Logistica.
4. **Ottimizzazione**: Ricerca degli iperparametri ottimali tramite GridSearchCV e validazione robusta con Cross-Validation.

## Dataset
Il dataset utilizzato è il **Cirrhosis Patient Survival Prediction Dataset**, reperito dall'archivio UCI Machine Learning Repository. 
- **Samples**: 418
- **Feature predittive**: 19 (tra cui Bilirubina, Colesterolo, Albumina, Età, Prolina, ecc.)
- **Target**: Status (Deceduto vs Censito/Sopravvissuto)

## Librerie Utilizzate
Il progetto è stato sviluppato in Python utilizzando le seguenti librerie:
- `pandas` e `numpy`: per il caricamento e la manipolazione dei dati.
- `matplotlib` e `seaborn`: per la visualizzazione statistica e i grafici (Boxplot, Heatmap, Confusion Matrix).
- `scikit-learn`: per l'intera parte di machine learning (Preprocessing, Logistic Regression, GridSearchCV, Metrics).

## Come eseguire il codice
1. Scaricare il repository contenente il file del codice (notebook `.ipynb` o script `.py`).
2. Assicurarsi di disporre del file `cirrhosis.csv` nella stessa directory del codice.
3. Installare le dipendenze necessarie:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
