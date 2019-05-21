# etna-codetest

## Installer le projet

Vérifier que PHP >= 7.1 et Composer sont installés, puis modifier le .env pour pointer sur votre BDD locale.

```
git clone
composer install
php bin/console doctrine:schema:update
```

## Comment le projet a été initialisé

Vérifier que PHP >= 7.1 et Composer sont installés, puis :

```
composer create-project symfony/website-skeleton etna-codetest
composer require symfony/orm-pack
composer require --dev symfony/maker-bundle
```
Modifier le .env pour pointer sur votre BDD locale.
```
php bin/console doctrine:database:create
php bin/console make:entity
php bin/console make:crud Blog
```
