# regressione lineare semplice
La regressione lineare semplice è un metodo statistico fondamentale usato per esaminare la relazione tra due variabili, una variabile **dipendente** e una variabile **indipendente**

### in cosa consiste
La regressione lineare semplice (Simple Linear Regression, **SLR**) è una tecnica statistica che permette di *studiare* e *quantificare* la *relazione* tra due variabili. In particolare, si cerca di modellare la relazione tra una variabile **dipendente** ($Y$) e una variabile **indipendente** ($X$) attraverso una linea retta che **minimizza la distanza** (**errori**) tra i valori osservati e i valori predetti dalla retta di regressione

### obiettivo
L'obiettivo della retta di regressione lineare semplice è quello di **predirre** il valore della variabile **dipendente** $Y$ basandosi sul valore della variabile **indipendente** $X$.
Tramite SLR siamo inoltre in grado di predirre la natura della relazione tra le due variabili. La SLR può anche essere utilizzata per testare ipotesi scientifiche riguardo le relazioni tra variabili.

Attraverso la retta di regressione semplice otteniamo la formula matematica di una retta espressa come

$$
Y = a + bX + \epsilon
$$

- $Y$: rappresenta la variabile **dipendente** che vogliamo prevedere o spiegare
- $X$: è la variabile **indipendente** che stiamo usando per la predizione
- $a$: è l'intercetta sull'asse $Y$ della retta di regresssione
- $b$: è la **pendenza** della retta di regressione, rappresenta il cambiamento di $Y$ per unità di cambiamento di $X$
- $\epsilon$: consiste nell'**errore** di stima, ovvero la differenza tra i valori osservati di $Y$ e quelli predetti dall'equazione della retta di regressione

### assunzioni
- **linearità**: indica che la relazione tra la variabile **indipendente** ($X$) e la variabile **dipendente** ($Y$) è lineare. Questo significa che il cambiamento nella variabile dipendente è proporzionale al cambiamento nella variabile indipendente.
- **normalità**: gli erorri del modello (**residui**) devono essere *normalmente distribuiti*, è possibile verificare questa assunzione attraverso test statistici o graficamente come un `plot Q-Q`
- **omoschedascticità**: indica che la **varianza** degli errori è **costante**; la varianza dei residui (errori) deve rimanere costante attraverso i vari valori della variabile indipendente ($X$). Se la varianza cambia a diversi valori della variabile indipendente, allora si dice che la varianza è **eteroschedastica**, la quale può invalidare le predizioni del modello
- **indipendenza dagli errori**: gli errori (residui) devono rimanere indipendenti l'uno dall'altro. Nel caso in cui gli errori sono dipendenti, si parla di **autocorrelazione**, la quale può invalidare le predizioni del modello

Ognuna di queste assunzioni è fondamentale per garantire l'**accuratezza** e l'**affidabilità** del modello di regressione lineare semplice. Nel caso in cui queste assunzioni sono verificate si parla di un modello in grado di fornire stime **unbiased** (non distorte) 