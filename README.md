# 🚲 Bicycle Network Design: Combinatorial Optimization

### Progetto di Ricerca Operativa - Laurea Magistrale
**Sviluppato da:** Sara Tullini & Davide Negri

---

## 📌 Panoramica del Progetto
Il progetto affronta un problema di **Network Design** nel contesto della pianificazione urbana. L'obiettivo è progettare una rete ciclabile connessa che massimizzi l'attrattività totale (*Likeness*) per i cittadini, rispettando un vincolo di budget stringente.

Il problema è stato modellato come un problema di ottimizzazione su grafi, risolto attraverso l'implementazione di diverse euristiche e meta-euristiche avanzate.

---

## ⚙️ Metodologia e Algoritmi
Per affrontare la complessità combinatoria del problema, sono stati implementati e confrontati quattro approcci:

1.  **Algoritmo Greedy:** Una tecnica costruttiva che seleziona gli archi con il miglior rapporto attrattività/costo, garantendo la connessione della rete.
2.  **Local Search:** Algoritmo di miglioramento per esplorare l'intorno della soluzione iniziale alla ricerca di ottimi locali.
3.  **G.R.A.S.P. (Greedy Randomized Adaptive Search Procedure):** Introduzione della componente stocastica per sfuggire agli ottimi locali ed esplorare più aree dello spazio di ricerca.
4.  **LNS (Large Neighborhood Search):** L'approccio più avanzato basato sulla strategia **Destroy & Repair**. Rimuovendo e ricostruendo ampie porzioni della rete, l'algoritmo è riuscito a convergere verso il presunto ottimo globale.



---

## 📊 Risultati Ottenuti
L'analisi comparativa ha dimostrato l'efficacia delle meta-euristiche rispetto agli approcci classici:

| Metodo | Attrattività (Likeness) | Budget Utilizzato |
| :--- | :---: | :---: |
| **Greedy** | 129 | 43 / 44 |
| **Local Search** | 129 | 43 / 44 |
| **G.R.A.S.P.** | 154 | 44 / 44 |
| **LNS (Migliorato)** | **154** | **44 / 44** |

I modelli migliorativi (GRASP e LNS) hanno permesso di ottenere un incremento del **19.3%** dell'attrattività della rete rispetto alla soluzione base, saturando il budget in modo efficiente, ottenendo un presunto ottimo globale.

---

## 🖼️ Visualizzazione della Rete
Di seguito, la rappresentazione del grafo ottimizzato dove sono stati selezionati gli archi che garantiscono la massima connessione e appetibilità turistico-culturale:



---

## 🛠️ Tecnologie Utilizzate
* **Linguaggio:** Python
* **Librerie:** `NetworkX` (Teoria dei grafi), `Matplotlib` (Visualizzazione), `Numpy`.
* **Modellazione:** Grafi non orientati, vincoli di connessione e budget.

---

## 🔒 Nota sul Codice
*Per rispettare le policy accademiche e permettere il riutilizzo didattico del progetto, il codice sorgente e le istanze specifiche del problema sono mantenuti in un repository privato.*

---
*A.A. 2024/2025 - Corso di Ricerca Operativa*
