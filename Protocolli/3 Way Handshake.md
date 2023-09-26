È il processo che 2 #host usano per stabilire una connessione sicura per comunicare attraverso il [[TCP]].
La _stretta di mano_ consiste in appunto 3 passaggi:

1. #SYN  --> un messaggio di 'SYNchronize' dal client al server che contiene il _numero di sequenza_ del client 
2. #SYN-ACK --> un messaggio di 'SYNchronize-ACKnowledgment' che contiene il _numero di sequenza_ e il _numero di conferma_
3. #ACK --> un messaggio di 'ACKnowledgment' che conferma la ricezione del massaggio SYN-ACK

![3way|700](https://afteracademy.com/images/what-is-a-tcp-3-way-handshake-process-three-way-handshaking-establishing-connection-6a724e77ba96e241.jpg)

