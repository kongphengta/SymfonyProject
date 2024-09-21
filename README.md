# Le projet Symfony
 ## Environnement de travail
 - PC Windows 11
 - Symfony 7
 - Symfony CLI
 - Composer 2.7.1
 - PHP 8.2.20


Initialiser Projet Symfony.
```
composer create-project symfony/skeleton:"7.1.*" SymfonyProject
```
Une fois l'installation est terminée, aller dans le projet 'SymfonyProject'
```
cd SymfonyProject
```
Puis installer webapp avec Composer.
```
composer require webapp
```
Paramétrer de fichier .env pour travailler en local, il faut d'abord copier ce fichier .env en .env.local et configurer ce dernier, il faut savoir aussi l'utilisateur de ce serveur et la version du serveur.
```
cp .env .env.local
```
Après avoir paramétré le fichier .env.local je vais massurer que mon projet n'a pas de problème côté serveur MySQL (MariaDB) je vais créer une base de données, je lance la commande.

```php
php bin/console doctrine:database:create
```
Avec cette commande doctrine va créer la base de données avec le nom de la base de données que j'ai attribué dans fichier .env.local.


