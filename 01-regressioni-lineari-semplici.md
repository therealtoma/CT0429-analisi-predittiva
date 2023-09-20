# Statistical learning

L'obiettivo è quell odi predire una risposta basandosi su una serie di variabili esplicative. Questo è un problema di **regressione** se la risposta è continua, oppure di **classificazione** se la risposta è categorica.

Si divide in due:

- **Supervised learning**: si hanno delle osservazioni $(x_1, y_1), \dots, (x_n, y_n)$ e si vuole individuare il valore di $y$ essendo a conoscenza di $x$. Questo è un problema di **regressione** (o **predizione**) se la risposta è continua, oppure di **classificazione** se la risposta è discreta.

- **Unsupervised learning**: si hanno delle osservazioni $(x_1, \dots, x_n)$ e si vuole capire la struttura di $x$.

## Notazione
Per spiegare la notazione faremo uso di un esempio. Supponiamo di voler capire come variano le vendite di una campagna pubblicitaria in base al luogo dove viene trasmessa (*TV*, *radio*, *newspaper*).
![regressioni lineari](./assets/01/01-sales-regressions.PNG)

- $Y$: variabile **risposta** / **obiettivo** / **risultato** / **output** (in questo caso le vendite)
- $X_1, \dots, X_n$: variabili **caratteristiche** / **predittori** / **regressori**  (in questo caso *TV*, *radio*, *newspaper*)
- $X$ è il vettore che contiene le variabili caratteristiche (in questo caso $X = (X_1, X_2, X_3)$)
- Il nostro **modello** sarà quindi la funzione: ($\epsilon$ indica l'errore o discrepanze tra il modello e i dati reali)
$$
Y = m(X) + \epsilon
$$

In pratica, il nostro obiettivo è quello di trovare la funzione $m$ (che in futuro indicheremo con $\hat{m}(X)$)che meglio approssima i dati reali.

I motivi per cui stimeremo $m$ sono:
- predizioni
- inferenza (interpretazione dei dati)

### Predizioni vs inferenza
- **Predizioni**: capire le possibiltà che un determinato evento succeda o meno
- **Inferenza**: determinare il motivo per cui un determinato evento succederà o meno

## Generalità
Quando costruiamo un modello $\hat{m}$ vogliamo che sia **flessibile** (ovvero che si adatti bene ai dati) ma che allo stesso tempo sia **semplice** (ovvero che sia facile da interpretare).
Un modello deve essere il più **bilanciato** possibile, non deve **sottostimare** ne **sovrastimare** i dati.

## Compromesso tra bias e varianza (bias-variance tradeoff)
Il **bias** è l'errore che si commette quando si approssima un problema complesso con un modello semplice. Un modello con un alto bias tenderà a sottostimare i dati. La **varianza** è l'errore che si commette quando si approssima un problema semplice con un modello complesso. Un modello con una alta varianza tenderà a sovrastimare i dati.

![bias-variance trade-off](./assets/01/01-bias-variance-tradeoff.PNG)

## Compromesso tra interpretabilità e flessibiltià (interpretability-flexibility tradeoff)
Possiamo costrutire sia modelli che sono molto flessibili ma poco interpretabili, sia modelli che sono poco flessibili ma molto interpretabili. Un modello flessibile è un modello che si adatta bene ai dati, mentre un modello interpretabile è un modello che è facile da interpretare.

Preferiremo modelli più strutturati rispetto a modelli più flessibili.