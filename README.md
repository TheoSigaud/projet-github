# Projet-git



## Les fonctionnalitées


### Pré-requis

Avant de lancer le projet il vous faudra installer:

- Docker

### Installation

Cloner le repository.

Copier le fichier sample.env en le renommant .env à la racine du projet.

Remplir tous les champs d'authentification de la BDD dans le fichier .env.

Lancer le docker-compose.yml:
```
$ docker-compose up -d --build
```


Dans le container, exécuter les commandes suivantes pour générer la BDD:

```
$ composer install
$ composer update
$ php artisan migrate --seed
```