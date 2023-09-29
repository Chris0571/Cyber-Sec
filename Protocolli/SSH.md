#### *__Secure Shell__* è un protocollo che fornisce l'interfaccia di #shell sicura da remoto 

Ecco alcune delle caratteristiche di SSH:

- Crittografia #end-to-end
- Autenticazione forte
- Compressione dei dati
- Tunneling
- Scambio di chiavi

## _Utilizzo

#### `$ ssh-keygen` 
genera le #chiavi pubbliche e private per configurare e stabilire le connessioni 

#### `$ ssh-copy-id <user>@<host>`
utilizzato per copiare la chiave del host remoto sul proprio host

#### `$scp`
utilizzato per il trasferimento di #file via ssh


### _I file di configurazione sono_
- `/etc/ssh/sshd_config`
- `/etc/ssh/ssh_config`
