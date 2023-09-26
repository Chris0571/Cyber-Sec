Il __*Network Time Protocol*__ è un protocollo di rete che sincronizza i clock di computer su una rete. È stato sviluppato negli anni '80 e da allora è diventato lo *standard* per la sincronizzazione del tempo su Internet.

1. Il client NTP invia una richiesta al server NTP, che contiene l'ora corrente del client. 
2. Il server NTP risponde con l'ora corrente del server, insieme a una differenza di tempo tra l'ora del client e l'ora del server. 
3. Il client NTP utilizza quindi questa differenza di tempo per sincronizzare il proprio orologio con l'orologio del server.

NTP è molto importante per il funzionamento di Internet e di altre reti tra cui [[Active Directory]]