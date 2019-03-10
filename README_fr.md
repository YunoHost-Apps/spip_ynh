# SPIP pour YunoHost

[![Integration level](https://dash.yunohost.org/integration/spip.svg)](https://dash.yunohost.org/appci/app/spip)  
[![Install spip with YunoHost](https://install-app.yunohost.org/install-with-yunohost.png)](https://install-app.yunohost.org/?app=spip)

*[Read this readme in english.](./README.md)* 

> *Ce package vous permet d'installer spip rapidement et simplement sur un serveur Yunohost.  
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

SPIP est un système de publication pour l’Internet qui s’attache particulièrement au fonctionnement collectif, au multilinguisme et à la facilité d’emploi. C’est un logiciel libre, distribué sous la licence GNU/GPL. Il peut ainsi être utilisé pour tout site Internet, qu’il soit associatif ou institutionnel, personnel ou marchand.

Source: [spip.net](http://www.spip.net/fr_rubrique91.html)

**Version incluse:** 3.2.3

## Captures d'écran

![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1c/Logo_SPIP.png/220px-Logo_SPIP.png)

## Démo

* [Démo officielle](https://demo.spip.net/)

## Configuration

Comment configurer cette application: via le panneau d'administration.

## Documentation

 * Documentation officielle: https://www.spip.net

## Caractéristiques spécifiques YunoHost

#### Support multi-utilisateurs

L'authentification LDAP et HTTP est-elle prise en charge? **Oui**
L'application peut-elle être utilisée par plusieurs utilisateurs? **Oui**

#### Supported architectures

* x86-64b - [![Build Status](https://ci-apps.yunohost.org/ci/logs/spip%20%28Community%29.svg)](https://ci-apps.yunohost.org/ci/apps/spip/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/spip%20%28Community%29.svg)](https://ci-apps-arm.yunohost.org/ci/apps/spip/)
* Jessie x86-64b - [![Build Status](https://ci-stretch.nohost.me/ci/logs/spip%20%28Community%29.svg)](https://ci-stretch.nohost.me/ci/apps/spip/)

## Links

 * Signaler un bug: https://github.com/YunoHost-Apps/spip_ynh/issues
 * Site de l'application: Lien vers le site officiel de cette application
 * Site web YunoHost: https://yunohost.org/

---

Informations pour les développeurs
----------------

**Seulement si vous voulez utiliser une branche de test pour le codage, au lieu de fusionner directement dans la banche principale.**
Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/spip_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
ou
sudo yunohost app upgrade spip -u https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
```