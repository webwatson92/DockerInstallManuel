# Installation de la distro linux sur window 10

  - wsl -l -v
  - wsl --install -d Ubuntu
  - wsl -l -o

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

