***Récap 3 premières couches du modèle OSI***

Couche 1 : couche physique  
Couche 2 : couche liaison (adressage physique MAC)  
Couche 3 : couche IP, avec protocole IPv4, adresses, relations entre réseaux et sous réseaux, routing  

<br>
Couche transport : TCP et UDP
elle assure qu'un message soit transmis d'un processus vers un autre  

Les adresses de cette couche sont les "ports", sur 16 bits  soit 65535 ports maximum  

Communication par Proxy, à l'instar des cables de la couche 1, switch de la couche 2, routeur de la couche 3  

L'IANA, un ogranisme international, conventionne les ports  
Ex : HTTP 80, 443 HTTPS (SSL/TLS), 22 SSH, 3389 RDP, DHCP Server 67, Client 68

**Exemple du port UDP** :  

Un processus envoie une requête à un second processus, ce dernier envoie une réponse via le port UDP  

![udp](https://github.com/Simplon-AlainCaupin/cours_reseau/blob/75f76754c76a271155efcf5bc9051a4d06c1eed1/IMG/screen2_udp.png)

UDP ne garantit pas la bonne réception ni l'ordre d'arrivée des paquets  

Il existe un flag pour dire que le paquet a bien été échangé :  
envoi de la requête -> numéro de séquence -> réponse à la requête (ack.)  

TCP est un protocole orienté "stream"  
Il y a un "handshake" entre les 2 processus -> échange de paquets avec des "flags"  

![udpexch](https://github.com/Simplon-AlainCaupin/cours_reseau/blob/75f76754c76a271155efcf5bc9051a4d06c1eed1/IMG/screen3_udp-between-processes.png)