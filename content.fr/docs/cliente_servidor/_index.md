---
weight: 3
bookFlatSection: true
title: "Client--> Serveur"
---

# Communication client avec le serveur

Nous allons essayer d'expliquer le processus par lequel un client communique avec un serveur.

L'*architecture client-serveur* ou *modèle client-serveur* est un protocole de communication à travers un réseau (comme Internet) dans lequel les tâches sont réparties entre les fournisseurs de ressources ou de services, appelés **serveurs**, et les demandeurs, appelés **clients**.

Un client fait des requêtes à un autre programme, le serveur, qui répond.

Dans ce cas, pour expliquer comment s'effectue la communication, nous allons nous intéresser au processus de chargement d'une page web.

Il est important de mentionner qu'une grande partie des services Internet obéit à l'*architecture client-serveur*. Le serveur Web met les sites Web à la disposition du client, qui sont accessibles via le navigateur. C'est le serveur qui héberge les données demandées par le client (navigateur).

### Notions importantes:
>> **Client**: appareil connecté à Internet (par exemple, un ordinateur connecté au réseau Wi-Fi ou un téléphone connecté au réseau de téléphonie mobile) et le logiciel disponible et permettant l'accès à Internet (généralement un navigateur).

>> **Serveur**: ordinateur qui stocke des pages Web, des sites ou des applications.

>> **TCP/IP: Transmission Control Protocol et Internet Protocol**, protocoles de communication qui définissent la manière dont les données doivent transiter sur le Web.

>> **DNS**: serveurs du **Domain Name System**, nous pourrions les définir comme un carnet d'adresses de site Web. Lorsque vous saisissez une adresse Web dans votre navigateur, généralement un domaine (comme *www.google.es*), DNS traduit ce nom de domaine en son adresse IP pour savoir sur quel serveur le site Web réside afin qu'il puisse envoyer des messages HTTP à endroit approprié.

>> **HTTP**: Le protocole de transfert hypertexte est un protocole d'application qui définit la manière dont les clients et les serveurs communiquent.

## Que se passe-t-il alors ?
Lorsque vous saisissez une adresse Web (ou un domaine) dans le navigateur:

1. Le navigateur se rend sur le serveur DNS et trouve la véritable adresse du serveur sur lequel le site Web est hébergé.
2. Le navigateur envoie un message de requête HTTP au serveur, lui demandant d'envoyer une copie de la page Web au client. Ce message, ainsi que toutes les données envoyées entre le client et le serveur, sont envoyés via la connexion Internet à l'aide de TCP/IP.
3. Chaque fois que le serveur approuve la demande du client, le serveur commence à envoyer les fichiers de la page Web au navigateur sous la forme d'une série de petits morceaux appelés paquets de données.
4. Le navigateur rassemble les petits morceaux, forme un site Web complet et vous le montre.

## Exemple graphique

{{< mermaid>}}
flowchart LR
    id1(Client - Navigateur)-->id2(DNS)
    id2-- adresse IP -->id1
    id1-->id3{{l'Internet}}-->id4[(Serveur)]
{{< /mermaid >}}

Une fois la demande approuvée:
{{< mermaid>}}
flowchart LR
    id4[(Serveur)]-->id3{{l'Internet}}-->id1(Client - Navigateur)
{{< /mermaid >}}