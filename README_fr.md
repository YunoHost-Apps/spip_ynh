# SPIP pour YunoHost

[![Integration level](https://dash.yunohost.org/integration/spip.svg)](https://dash.yunohost.org/appci/app/spip)  
[![Install spip with YunoHost](https://install-app.yunohost.org/install-with-yunohost.png)](https://install-app.yunohost.org/?app=spip)

*[Read this readme in english.](./README.md)* 

> *Ce package vous permet d'installer spip rapidement et simplement sur un serveur Yunohost.  
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

SPIP est un système de publication pour l’Internet qui s’attache particulièrement au fonctionnement collectif, au multilinguisme et à la facilité d’emploi. C’est un logiciel libre, distribué sous la licence GNU/GPL. Il peut ainsi être utilisé pour tout site Internet, qu’il soit associatif ou institutionnel, personnel ou marchand.

Source: [spip.net](http://www.spip.net/fr_rubrique91.html)

**Version incluse:** 3.2.8

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

* x86-64 - [![Build Status](https://ci-apps.yunohost.org/ci/logs/spip%20%28Community%29.svg)](https://ci-apps.yunohost.org/ci/apps/spip/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/spip%20%28Community%29.svg)](https://ci-apps-arm.yunohost.org/ci/apps/spip/)

## Migration depuis SPIP2

**Ceci n'est pas encore considéré comme stable, veuillez le faire avec soin et uniquement pour test!**

Ce paquet gère la migration de SPIP2 vers SPIP. Pour cela, votre application SPIP2 doit être **à jour** dans YunoHost. Pour s'en assurer :

```bash
sudo yunohost app upgrade -u https://github.com/YunoHost-Apps/spip2_ynh spip2 --debug
```

Vous devrez ensuite mettre à jour votre application SPIP2 avec ce dépôt.
Cela ne peut se faire qu'à partir de l'interface en ligne de commande - par exemple via SSH. Une fois connecté, il vous suffit d'exécuter ce qui suit :

```bash
sudo yunohost app upgrade -u https://github.com/YunoHost-Apps/spip_ynh spip2 --debug
```

L'option `--debug` vous permettra de voir la sortie complète. Si vous rencontrez un problème, veuillez ouvrir une issue.

Notez qu'une tâche cron sera exécutée après la fin de cette commande. Vous devez attendre cela avant de faire toute autre opération d'application ! Vous devriez voir que SPIP est installé après cela.

## Links

 * Signaler un bug: https://github.com/YunoHost-Apps/spip_ynh/issues
 * Site de l'application: Lien vers le site officiel de cette application
 * Site web YunoHost: https://yunohost.org/

---

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/spip_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
ou
sudo yunohost app upgrade spip -u https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
```
