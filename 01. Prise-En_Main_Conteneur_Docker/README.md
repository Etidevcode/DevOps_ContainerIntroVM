# Introduction :

## : Introduction pratique à Docker.
**Préparation :** 

Utilisation de `Git Bash` ou d’un terminal pour créer un répertoire et y placer un fichier `Vagrant` basé sur `Ubuntu 20` pour installer Docker.


## Étapes Clés :

+ **Configuration de l'environnement :**

    + Utilisation de `Vagrant` pour configurer une machine virtuelle (VM) avec Docker.
    + Commandes nécessaires disponibles dans la documentation Docker.

+ **Installation de Docker :**

    + Lancer la VM avec `vagrant up`.
    + Se connecter à la `VM` via SSH et vérifier l'état du service Docker (systemctl status docker).

+ **Premier Test Docker :**

    + Exécution de la commande `docker run hello-world` pour tester Docker.
    + Commandes utiles : `docker images` pour voir les images disponibles, `docker ps` pour voir les conteneurs en cours d'exécution, et `docker ps -a` pour tous les conteneurs.

+ **Création et Gestion de Conteneurs :**

    + Exemple de création d'un conteneur Nginx avec des options de nom et de mappage de port (`docker run --name web01 -d -p 9080:80 nginx`).
    + Accéder au conteneur via l'adresse IP de la VM et le port mappé.

+ **Création d'Images Personnalisées :**

    + Création d'un Dockerfile pour définir une image basée sur Ubuntu.
    + Construction de l'image avec `docker build -t <nom_image>` ..

+ **Nettoyage :**

    + Commandes pour arrêter (`docker stop <nom_conteneur>`) et supprimer (`docker rm <nom_conteneur>, docker rmi <ID_image>`) les conteneurs et images pour préparer l'environnement pour la prochaine session.



