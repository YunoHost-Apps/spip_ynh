# SPIP pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/spip.svg)](https://dash.yunohost.org/appci/app/spip) ![](https://ci-apps.yunohost.org/ci/badges/spip.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/spip.maintain.svg)  
[![Installer SPIP avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=spip)

*[Read this readme in english.](./README.md)*
*[Lire ce readme en français.](./README_fr.md)*

> *Ce package vous permet d'installer SPIP rapidement et simplement sur un serveur YunoHost.
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

CMS conçu pour l'édition collaborative et le multilinguisme

**Version incluse :** 4.1.0-rc~ynh1

**Démo :** https://demo.spip.net/

## Captures d'écran

![](./doc/screenshots/220px-Logo_SPIP.png)

## Avertissements / informations importantes

## Configuration

Comment configurer cette application: via le panneau d'administration.

#### Support multi-utilisateurs

 * L'authentification LDAP et HTTP est-elle prise en charge? **Oui**
 * L'application peut-elle être utilisée par plusieurs utilisateurs? **Oui**

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

## Documentations et ressources

* Site officiel de l'app : http://www.spip.net/
* Documentation officielle utilisateur : https://www.spip.net/en_rubrique57.html
* Documentation officielle de l'admin : https://www.spip.net/en_rubrique209.html
* Dépôt de code officiel de l'app : https://git.spip.net/spip/spip
* Documentation YunoHost pour cette app : https://yunohost.org/app_spip
* Signaler un bug : https://github.com/YunoHost-Apps/spip_ynh/issues

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/spip_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
ou
sudo yunohost app upgrade spip -u https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
```

**Plus d'infos sur le packaging d'applications :** https://yunohost.org/packaging_apps