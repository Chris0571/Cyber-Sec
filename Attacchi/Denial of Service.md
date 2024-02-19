I **_DoS_** o _**Distributed DoS**_ sono attacchi che rendono risorse o servizi inaccessibili.
L'attacco è _volumetrico_, ovvero quantitativo, spesso eseguito tramite botnet
ad un dispositivo/rete viene inviato più traffico di quanto possa ricevere,
conseguenze:
- perdita di pacchetti
- degrado della performance
- interruzione della rete

Attacchi di tipo *__BPS__* e *__PPS__*
- *BPS* -> è un'attacco alla larghezza di banda
- *PPS* -> un'attacco per numero di pacchetti

Bersagli tipici di DoS:
- #e-commerce
- siti gaming 
- gambling
- health orgs
- #IoT devices con lo scopo di crearsi un punto di accesso in reti aziendali


## Attacchi di tipo #flood

### [[TCP]] #SYN flood
Viene inviato un elevato volume di pacchetti SYN sulla porta target dell'attacco, senza l'intento di completare il 3-way handshake 
- diretto -> senza indirizzi contraffatti (facilmente rintracciabile)
- spoofing -> quando si nasconde l'IP del mittente del pacchetto
- distribuito -> un attacco da botnet e quindi da più indirizzi che può anche essere spoofed
##### come mitigarlo
- aumentare le risorse
- ripristinare la prima connessione TCP rimasta aperta
- cookie SYN


### [[UDP]] garbage flood
Mira all'_inondazione_ di pacchetti UDP su diverse porte costringendo il server a rispondere con _[[ICMP]] type 3_ (un messaggio "Destinazione irraggiungibile")
In questo modo viene inondata la rete sia in entrata che in uscita
Facilmente distinguibile per il contenuto dei pacchetti (garbage)

### [[GRE]] protocol flood
Incapsulando ed inviando grandi quantità di pacchetti GRE porta il server target ad esaurire le risorse di rete per il de-incapsulamento del payload.

### [[DNS]] flood
Attraverso l'utilizzo di #Botnet composte da #IoT a larghezza di banda elevata, si prendono di mira server DNS che vengono stravolti e non riescono a soddisfare le richieste degli utenti legittimi
-> difficile da individuare

### [[HTTPs]] flood
Con l'utilizzo di #Botnet si inonda di richieste HTTPs un server web, anche quest'attacco è difficile da individuare.
Di tipo:
- GET -> richieste di immagini o di altre risorse 
- POST -> invio di dati che il server immagazzina

## Attacco #DRDoS (DistributedReflectiveDoS)
Un attacco DDoS a #riflessione utilizza lo #spoofing con l'indirizzo della vittima stessa, in modo che le richieste che fa al server avranno risposte mandate alla vittima stessa.
È stato utilizzato con il protocollo [[CLDAP]] nel 2016 per un attacco ad Akamai 
![dos](https://www.akamai.com/site/it/images/article/2023/what-is-cldap-ddos.png)

## Attacco #DRDoS _ad Amplificazione_
È l'evoluzione del DRDoS, viene aggiunto un fattore di amplificazione per aumentare la potenza dell'attacco.
Utilizza #spoofing e #riflessione con protocolli che per una richiesta danno una o più risposte
![amplification-protocols|900](https://www.zdnet.com/a/hub/i/2020/06/17/0555c3f2-68fd-4804-88d0-68fb589bac61/ddos-reflection-amplification-vectors-timeline-en.jpg)

## Attacco #DRDoS _Carpet Bombing_
Un'altra variante del DRDoS che anziché prendere di mira un IP specifico della vittima da come IP richiedente una sotto-rete
Difficile da rilevare e gestire


#### #Stresser
Strumenti creati per testare la capacità di resistenza dei sistemi ad attacchi #DoS 

#### #Booter
Sono essenzialmente _stresser_ ma sistemati e venduti come Software as a Service ( #SaaS), pronti per essere usati in attacchi #DoS 

#### Attacco #Pulse-Wave o #Hit-and-Run
È una strategia che consiste nell'attaccare più bersagli contemporaneamente, uno dopo l'altro, con brevi picchi di traffico.
Il tutto avviene in cicli ripetitivi in modo da evitare i sistemi di sicurezza Anti-DoS utilizzati per difendersi da attacchi prolungati.


#### #PDoS Permanent DoS
Un attacco che mira a danneggiare i dispositivi permanentemente.
Attraverso falle di sicurezza dell'amministrazione remota l'attaccante cambia la versione #firmware della macchina 

