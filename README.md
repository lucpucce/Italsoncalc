# 📉 Simulazione Demografica: Stabilizzazione della Popolazione Italiana

Un simulatore demografico interattivo e autocontenuto in un unico file HTML. Il progetto permette di esplorare visivamente gli scenari futuri della popolazione italiana da qui al 2100, analizzando l'impatto del tasso di fertilità e dei flussi migratori.

---

## 🔬 Il Modello Scientifico e Scenari

Il simulatore si basa sulle dinamiche demografiche (struttura della popolazione per coorti d'età, tassi di mortalità e natalità) e permette di simulare tre scenari principali modificando il **Tasso di Fecondità Totale (TFT)** tramite gli slider:

1. **Scenario di Declino (Inerzia Attuale):** Basato sul tasso di natalità corrente in Italia (circa $1.2$ - $1.3$ figli per donna), che mostra il progressivo e rapido invecchiamento della popolazione e la contrazione dei cittadini in età lavorativa.
2. **Scenario di Stabilizzazione ($2.1$):** Dimostra l'effetto del raggiungimento del **tasso di rimpiazzo generazionale**, fissato matematicamente a **$2.1$ figli per donna**, livello necessario nel lungo periodo per stabilizzare la popolazione al netto delle migrazioni.
3. **Scenario di Transizione Politica:** Permette di simulare una crescita graduale della fertilità nel tempo, legata a potenziali politiche di welfare e sostegno alla natalità.

---

## 🛠️ Caratteristiche del Progetto

* **Tutto in uno (Standalone):** Il simulatore è interamente racchiuso nel file `index.html`. Include l'interfaccia grafica, la logica matematica in JavaScript e la visualizzazione dei grafici.
* **Interattivo:** Muovendo gli slider puoi cambiare istantaneamente il tasso di fertilità e vedere l'impatto sulla curva della popolazione fino al 2100.
* **Nessuna installazione:** Non richiede server, Python, Node.js o database. Funziona direttamente nel browser.

---

## 🚀 Come Usarlo

Puoi utilizzare e testare il simulatore in due modi:

### Opzione 1: Utilizzo Locale
1. Scarica il file `index.html` da questo repository.
2. Fai **doppio clic sul file** per aprirlo in un qualsiasi browser web (Chrome, Safari, Firefox, Edge). Funziona anche offline!

### Opzione 2: Navigazione Online (GitHub Pages)
Per vedere il simulatore direttamente online senza scaricare il file:
1. Vai nelle **Settings** (Impostazioni) di questa repository su GitHub.
2. Nel menu a sinistra, clicca su **Pages**.
3. Sotto *Build and deployment*, imposta il *Branch* su **main** (o `master`) e la cartella su `/ (root)`.
4. Clicca su **Save**. Dopo un minuto, GitHub ti fornirà un link pubblico (es. `https://tuo-username.github.io/nome-repo/`) per usare il simulatore online.

---

## 📊 Fonti e Logica di Calcolo

* **Dati di partenza:** Struttura della popolazione italiana divisa per fasce d'età (basata su proiezioni e storici ISTAT).
* **Algoritmo:** Calcola annualmente i nuovi nati applicando il tasso di fertilità selezionato alla popolazione femminile in età fertile ($15$-$49$ anni), applica i tassi di sopravvivenza per ogni coorte e somma il saldo migratorio impostato.
