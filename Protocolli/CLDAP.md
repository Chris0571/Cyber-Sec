Il protocollo *__Connection-less Lightweight Directory Access Protocol__* è una versione leggera del protocollo [[LDAP]] che utilizza il protocollo [[UDP]] invece del protocollo ~~[[TCP]]~~.
CLDAP è stato sviluppato da Microsoft per l'utilizzo con i servizi di [[Active Directory]].

### Caratteristiche principali
- Utilizza UDP invece di TCP, il che lo rende più efficiente in termini di risorse.
- Più facile da implementare rispetto a LDAP.
- Comunemente utilizzato in scenari in cui è necessario accedere a un servizio di directory da un dispositivo con risorse limitate.
- Non così affidabile come LDAP e non è ideale per applicazioni in cui è necessario garantire l'integrità dei dati.