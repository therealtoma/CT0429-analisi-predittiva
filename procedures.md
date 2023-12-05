**confrontare se due variabili sono uguali per due categorie**

un esempio è *dire se i salari medi sono uguali per uomini e donne*
bisogna effettuare un `t.test`. Usare una semplice media non è sufficiente.
Il test t è pensto prorpio per questo scopo: è un metodo statistico usato per determinare se esiste una significativa differenza tra le medie di due gruppi.
Motivi aggiuntivi per i quali è consigliato un `t.test`:
1. varianza all'interno dei gruppi
    anche se le medie sono diverse, questa differenza può essere dovuta da una serie di aspetti (i salari vaiano per molti motivi, non solamente per il genere)
2. valutazione della significatività statistica:
    il `t.test` determina se la differenza delle medie osservata è statisticamente significativa
3. ipotesi nulla e alternativa:
    l'ipotesi nulla indica che non è presente differenza tra le media, l'ipotesi alternativa afferma che la differenza è presente.