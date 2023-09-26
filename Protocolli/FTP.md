Il protocollo File Transfer Protocol (FTP) è un protocollo di rete utilizzato per trasferire file tra computer su Internet. È un protocollo di livello applicativo che opera su top di TCP.

Il protocollo FTP utilizza due porte TCP: la porta 21 per la comunicazione di controllo e la porta 20 per la comunicazione di dati. La porta 21 viene utilizzata per scambiare comandi tra il client FTP e il server FTP. La porta 20 viene utilizzata per trasferire i dati effettivi tra il client FTP e il server FTP.

##### I comandi FTP più comuni sono:

- **USER:** Questo comando viene utilizzato per specificare l'utente che si sta tentando di autenticare.
- **PASS:** Questo comando viene utilizzato per specificare la password dell'utente che si sta tentando di autenticare.
- **PWD:** Questo comando viene utilizzato per ottenere il percorso corrente del server FTP.
- **DIR:** Questo comando viene utilizzato per elencare i file e le directory nel percorso corrente del server FTP.
- **RETR:** Questo comando viene utilizzato per scaricare un file dal server FTP.
- **STOR:** Questo comando viene utilizzato per caricare un file sul server FTP.

##### Alcuni degli svantaggi di utilizzare FTP includono:

- Non è un protocollo sicuro. I dati trasferiti su FTP non sono crittografati, il che significa che possono essere intercettati da terzi.
- Non è un protocollo efficiente. Il trasferimento di file su FTP può essere lento, soprattutto per file di grandi dimensioni.