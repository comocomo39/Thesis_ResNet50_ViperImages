# 📌 Identificazione di Serpenti con Deep Learning e Dati Geografici

&#x20;&#x20;

## 📖 Descrizione

Questo progetto esplora il ruolo delle **coordinate geografiche** nel migliorare l'identificazione delle specie di serpenti utilizzando il **deep learning**. L'obiettivo è verificare se l'integrazione delle informazioni geografiche con le immagini possa aumentare l'accuratezza di un modello di classificazione basato su **ResNet-18** e **SVM lineare**.

Due specie di serpenti vengono analizzate:

- 🐍 **Vipera Aspis**
- 🐍 **Vipera Berus**

I dati provengono dalla piattaforma **iNaturalist**, che fornisce immagini geolocalizzate per queste specie.

---

## 🎯 Obiettivi

✔️ **Confrontare le performance di classificazione** utilizzando solo immagini, solo coordinate geografiche e la combinazione di entrambi.\
✔️ **Dimostrare l’impatto dei dati geografici** sulla classificazione di immagini attraverso tecniche di deep learning.\
✔️ **Analizzare l’importanza delle feature estratte** dal modello e il loro contributo alla classificazione finale.

---

## 🛠️ Tecnologie Utilizzate

Il progetto è stato sviluppato utilizzando **Python** con le seguenti librerie:

- 🔥 **PyTorch** (per il deep learning con ResNet-18)
- 📊 **Scikit-learn** (per SVM e analisi delle performance)
- 📈 **Matplotlib e Plotly** (per la visualizzazione dei dati)
- 📂 **Pandas** (per la gestione dei dataset)

---

## 📂 Struttura della Repository

📁 **notebooks/** → Contiene gli script Jupyter Notebook per l’addestramento del modello e l’analisi dei risultati.

- `imageswithoutcoordinates.ipynb` → Addestramento del modello con sole immagini.
- `ResNet50_imageswithcoordinates.ipynb` → Addestramento combinato con immagini e coordinate.
- `onlycoordinates.ipynb` → Modello addestrato solo con coordinate geografiche.

📁 **dataset/** → Contiene le immagini e i dati geografici utilizzati.

- `vipera_aspis/` e `vipera_berus/` → Cartelle con le immagini delle due specie.
- `coordinates.csv` → File CSV con le coordinate geografiche.

📄 **tesi.pdf** → Documento della tesi con dettagli tecnici e risultati.

---

## 🚀 Risultati

I test hanno mostrato che: ✅ La rete **ResNet-18** ottiene un’accuratezza del **87.5%** usando solo immagini. ✅ Il classificatore **SVM con sole coordinate geografiche** raggiunge **89%** di accuratezza. ✅ La combinazione di **immagini + coordinate geografiche** migliora l’accuratezza fino al **96%**. ✅ Anche quando le coordinate vengono alterate, l'accuratezza migliora rispetto all'uso esclusivo delle immagini.

**➡️ Conclusione**: l’integrazione di dati geografici aumenta la precisione della classificazione, rendendola un'informazione preziosa per il riconoscimento delle specie.

---

## 📌 Come Utilizzare il Progetto

1️⃣ **Clona la repository**

```bash
 git clone https://github.com/tuo-username/identificazione-serpenti.git
 cd identificazione-serpenti
```

2️⃣ **Installa le dipendenze**

```bash
pip install -r requirements.txt
```

3️⃣ **Esegui i notebook** per addestrare e testare i modelli.

---

## 📜 Citazioni e Fonti

- Dataset: [iNaturalist](https://www.inaturalist.org/)
- Architettura ResNet: [Deep Residual Learning for Image Recognition](https://arxiv.org/abs/1512.03385)
- SVM: [Scikit-Learn Documentation](https://scikit-learn.org/stable/modules/svm.html)

---


