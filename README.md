# Percolazione e robustezza nelle reti complesse: modello di Erdős-Rényi-Gilbert

Studio della transizione di fase di percolazione e della robustezza strutturale nel modello di grafi casuali di Erdős-Rényi-Gilbert (ERG) $G(N,p)$, con analisi teorica e simulazioni numeriche in Python.

---

## Descrizione

Questo progetto analizza la **connettività** e la **robustezza** delle reti complesse attraverso la teoria della percolazione applicata al modello ERG. Il modello $G(N, p)$, in cui ogni coppia di $N$ nodi è connessa da un link con probabilità $p$, costituisce il modello di riferimento ("modello nullo") per le reti casuali.

### Obiettivi principali

- **Transizione di fase**: individuazione della soglia critica $\langle k \rangle_c = 1$ per l'emergenza della componente gigante e stima degli esponenti critici $\beta$ e $\gamma$ tramite fit su ensemble di grafi simulati.
- **Percolazione inversa e robustezza**: derivazione e verifica della soglia critica di rimozione dei nodi $f_c = 1 - 1/\langle k \rangle$ oltre la quale la rete perde la componente gigante.

---
