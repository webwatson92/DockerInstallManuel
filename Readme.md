# Installation de la distro linux sur window 10

  - wsl -l -v
  - wsl --install -d Ubuntu
  - wsl -l -o
  - wsl --set-default : mettre par defaut

## Configure Ubuntu

- sudo apt update
- sudo apt upgrade
- Prêt à être utiliser comme un os normal

docker ps -a : voir la liste des containers existant dans docker
docker start id_container : demarrage
docker stop id_container : arret
docker rm id_container : pour delete le container

## Utilise éfficacement un container docker

l'option-v : permet de faire le mapping entre un repertoire du pc vers un container

```
    docker run -p 80:80 -v C:\Users\HardFive\devApp:/usr/local/apache/htdocs/ httpd

```

C:\Users\HardFive\devApp: étant le path du dossier des projets

---


![Docker Image](/docker.PNG "Image de resultat final")


---

## Création d'un container Linux au sein de notre Ubuntu

- Ouvrir le powershell ou cm en administrateur
```
    wsl -d <distro name>
    exemple : wsl -d Ubuntu-20.04
```
Le container de base pour les tests, vérification du bon fonction de votre installation
```
   docker run hello-world
```

## Docker compose
l'application qui facilite l'hébergement de plusieurs container avec chacun une fonction de base
Un container bdd, un container serveur etc...

Dans cette section, nous allons utiliser **NEXTCLOUD**, qui est un service de synchroniseur de fichier  comme dropbox ou onedrive.

Il est composer de deux parties, une partie qui gère la base de donnée et une autre qui s'occupe du serveur/code nextCloud

```
   docker-compose up -d
```
Vérification de son bon fonction via les logs
```
   docker-compose logs -f
```
![](/logs_docker.PNG "Résultat après le lancement de la commande.")

Arrêt du service
```
   docker-compose down
```
---

## PARLONS DIGITAL DEVELPMENT DEPARTMENT 

- **[FORMATION BLOG](http://BLOG.parlons-digital.com/)**
- **[PARLONS DIGITAL](http://www.parlons-digital.com/)**

## Conctat

- **[Youtube formation](https://www.youtube.com/parlonsdiital/)**
- **[Linkedin](https://www.linkedin.com/in/ouattaraelhadjy//)**
- **[Facebook](https://www.facebook.com/elhadjyoussouf.o/)**
- **[Discord group](https://discord.gg/uQ9UpWqC/)**
- **[Telegram group ](https://t.me/parlonsd/)** 
- **[Whatsapp Plateforme ](https://chat.whatsapp.com/JhXaVxWXmyN7E5FckGxrNQ/)** 

## License

This fil open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

