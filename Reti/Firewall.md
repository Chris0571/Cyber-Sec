Un _FW_ è un componente di _sicurezza informatica_ che controlla e monitora il traffico per via della [[Packet-Inspection]] di rete tra una rete interna (come una rete aziendale o domestica) e una rete esterna (come Internet).
Il suo scopo principale è quello di proteggere la rete interna da potenziali minacce provenienti dalla rete esterna, come intrusioni, attacchi informatici o accessi non autorizzati.

Per garantire più sicurezza una rete può essere divisa in #sotto-reti, come ad esempio:
- #WAN - Wide Area Network
	generalmente la sotto-rete che ha accesso all'esterno e quindi con internet.
- #LAN - Local Area Network
	una parte di rete che può essere considerata locale
- #DMZ - Demilitarized Zone
	una parte di rete che è in contatto con la rete locale ed allo stesso tempo con internet  perché magari ha un servizio che deve essere pubblico.

## Criteri o Policy

#default-deny -> viene accettato solo ciò che è stato dichiarato esplicitamente.
#default-allow -> viene vietato solo ciò che è stato dichiarato proibito, il resto passa.

Azioni applicabili ai pacchetti in base alle loro caratteristiche sono:
- **allow**  lascia passare il pacchetto
- **deny** blocca il pacchetto e lo rimanda indietro
- **drop** blocca il pacchetto senza rispondere 


## #Stateless-Firewall 
È un tipo di _FW_ che analizza i pacchetti singolarmente senza tenere in considerazione i pacchetti precedenti.

## #Stateful-Firewall
Come lo stateless analizza i pacchetti nel dettaglio ma a differenza sua tiene in considerazione lo stato della connessione e se per esempio arriva un pacchetto da qualcuno con cui non ha instaurato una connessione viene bloccato.

## #Application-Firewall 
È host-based perciò gira singolarmente sui vari host 
Molto utile poiché agisce su tutti i [[Livelli OSI]] filtrando tutto il traffico delle singole applicazioni, richiede però più potenza in quanto analizza il pacchetto complessivamente analizzando anche il #payload.
Possiede inoltre anche funzionalità #anti-malware.

## #Next-Gen _FW_
Sono dei Firewall con più funzionalità per garantire la sicurezza informatica, tra questi:
- Ispezione dei pacchetti a livello applicativo
- Prevenzione delle intrusioni
- Controllo degli URL
- Antivirus
- [[VPN]]
- [[IDS]]

