# Projet Enchères - R3.06

## Jonathan LECLERC  F2 

## Description
Application client/serveur simulant un système d'enchères en temps réel.

## Exécution

### 1. Lancer le Serveur

    java EnchereServeur

Le serveur vous demandera de configurer le premier objet à vendre (Nom et Prix de départ).

### 2. Lancer un Client ( 2 façon possible )
Dans un nouveau terminal (autant de fois que de clients souhaités) :

1. Client connecté au serveur : java Client
2. Ou se connecter via :
		Linux   :	nc localhost 6000
	    Windows :	telnet localhost 6000

Le client demandera un pseudo et l'adresse du serveur (par défaut 'localhost' en appuyant sur Entrée).

## Fonctionnement
- Une fois connecté, le client reçoit l'état actuel de l'enchère.
- Pour enchérir, le client tape simplement un montant entier et valide avec Entrée.
- Si 10 secondes s'écoulent sans enchère, le message "Une fois" apparaît.
- Si 10 secondes supplémentaires s'écoulent, "2 fois" apparaît.
- Enfin, l'objet est adjugé et le serveur demande à l'administrateur de configurer la vente suivante.