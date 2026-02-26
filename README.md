# Percolazione e robustezza nelle reti complesse: modello di Erdős-Rényi-Gilbert

Studio della transizione di fase di percolazione e della robustezza strutturale nel modello di grafi casuali di Erdős-Rényi-Gilbert (ERG) $G(N,p)$, con analisi teorica e simulazioni numeriche in Python.

---

## Descrizione

Questo progetto analizza la **connettività** e la **robustezza** delle reti complesse attraverso la teoria della percolazione applicata al modello ERG. Il modello $G(N, p)$, in cui ogni coppia di $N$ nodi è connessa da un link con probabilità $p$, costituisce il modello di riferimento ("modello nullo") per le reti casuali.

### Obiettivi principali

- **Transizione di fase**: individuazione della soglia critica $\langle k \rangle_c = 1$ per l'emergenza della componente gigante e stima degli esponenti critici $\beta$ e $\gamma$ tramite fit su ensemble di grafi simulati.
- **Percolazione inversa e robustezza**: derivazione e verifica della soglia critica di rimozione dei nodi $f_c = 1 - 1/\langle k \rangle$ oltre la quale la rete perde la componente gigante.

---

## Struttura del repository

```
ER-model/
├── relazione/          # Relazione scritta in LaTeX
│   ├── relazione.tex
│   ├── bibliografia.bib
│   └── images/         # Grafici prodotti dalle simulazioni
├── presentazione/      # Presentazione in LaTeX (beamer)
│   └── presentazione.tex
└── simulazione/        # Notebook Jupyter con le simulazioni numeriche
    ├── teo_graphs.ipynb        # Analisi teorica del modello ERG
    ├── phase_tr.ipynb          # Transizione di fase (parametro d'ordine e suscettività)
    ├── percolation.ipynb       # Percolazione inversa e robustezza
    └── percolation_UF.ipynb    # Percolazione con algoritmo Union-Find
```

---

## Dipendenze

Le simulazioni sono scritte in **Python 3** e richiedono le seguenti librerie:

- [igraph](https://igraph.org/python/) — generazione e analisi di grafi
- [NumPy](https://numpy.org/) — calcolo numerico
- [SciPy](https://scipy.org/) — fit e analisi statistica
- [Matplotlib](https://matplotlib.org/) — visualizzazione dei risultati

Installazione rapida:

```bash
pip install python-igraph numpy scipy matplotlib
```

---

## Utilizzo

Aprire i notebook nella cartella `simulazione/` con Jupyter:

```bash
jupyter notebook simulazione/
```

I notebook sono indipendenti e possono essere eseguiti in qualsiasi ordine.

---

## Risultati

| Quantità | Valore teorico | Valore ottenuto dal fit |
|---|---|---|
| Esponente critico $\beta$ | $1$ | $0.94 \pm 0.04$ |
| Esponente critico $\gamma$ | $1$ | $0.997 \pm 0.001$ |
| Parametro robustezza $\alpha$ | $1$ | $0.985 \pm 0.001$ |

---

## Riferimenti

- M. E. J. Newman, *Networks*, Oxford University Press, 2018.
- A.-L. Barabási, *Network Science*, Cambridge University Press, 2016.
- D. Stauffer & A. Aharony, *Introduction to Percolation Theory*, Taylor & Francis, 1994.

---

## Autore

**Giacomo Cicala**
