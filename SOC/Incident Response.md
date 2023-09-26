L'incident response è un insieme di procedure e azioni volte ad affrontare gli #incident. 
L'obiettivo principale dell'incident response è minimizzare gli effetti negativi di un incidente, ripristinare la sicurezza e la normalità delle operazioni e prevenire futuri incidenti simili.
Ne è parte fondamentale il [[Digital Forensic]] che aiuta a velocizzare e a migliorare il lavoro di un team di IR.

**1 _Preparazione_**
Questa fase coinvolge la pianificazione e la preparazione per gli incidenti di sicurezza
- creazione di piani di risposta
- implementazione di controlli di sicurezza

**2 _Identificazione_**
#early-warning 
quando si tenta di rilevare delle minacce in seguito ad eventi sospetti:
- port swap (scansione delle porte)
- utilizzo di porte non standard
- picchi di traffico in giorni/orari sospetti

#incident
quando è accaduto un attacco e si cerca l'attaccante:
- threat intelligence
- malware analysis

**3 _Contenimento_**
La fase in cui si risponde all'attacco, per isolare un sistema le fasi tipiche sono:
- disabilitare le porte dello switch
- bloccare gli IP, domini e URL
- bloccare gli account
- disabilitare software e servizi specifici

**4 _Eradicazione_**
In questa fase l'obiettivo è eliminare definitivamente la minaccia, la correzione delle [[vulnerabilità]] e l'applicazione di eventuali patch di sicurezza.

**5 _Ripristino_**
Dopo l'eliminazione della minaccia si può passare alla fase di recupero degli eventuali dati danneggiati, in questa fase 

**6 _Analisi e apprendimento_**
Alla conclusione dell'incident response, viene condotta un'analisi dettagliata dell'incidente per comprendere le cause, gli impatti e le lezioni apprese. Ciò aiuta a migliorare i processi di sicurezza, a identificare le lacune e a prendere misure correttive per evitare incidenti simili in futuro.



####  #IoC - _Indicatori di Compromissione_
Sono informazioni ricavate nell'identificazione, nell'analisi del malware o fonti pubbliche che stanno ad identificare un vettore d'attacco o attaccante:
- IP address
- porta e protocollo
- URL
- indirizzi mail
- file / HASH