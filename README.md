# SPIP for YunoHost

[![Integration level](https://dash.yunohost.org/integration/spip.svg)](https://dash.yunohost.org/appci/app/spip) ![](https://ci-apps.yunohost.org/ci/badges/spip.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/spip.maintain.svg)  
[![Install spip with YunoHost](https://install-app.yunohost.org/install-with-yunohost.png)](https://install-app.yunohost.org/?app=spip)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allow you to install spip quickly and simply on a YunoHost server.  
If you don't have YunoHost, please see [here](https://yunohost.org/#/install) to know how to install and enjoy it.*

## Overview

SPIP is a publishing system for the Internet in which great importance is attached to collaborative working, to multilingual environments, and to simplicity of use for web authors. It is free software, distributed under the GNU/GPL licence. This means that it can be used for any Internet site, whether personal or institutional, non-profit or commercial.

Source: [spip.net](http://www.spip.net/en_rubrique25.html)

**Shipped version:** 3.2.8

## Screenshots

![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1c/Logo_SPIP.png/220px-Logo_SPIP.png)

## Demo

* [Official demo](https://demo.spip.net/)

## Configuration

How to configure this app: by an admin panel.

## Documentation

 * Official documentation: https://www.spip.net

## YunoHost specific features

#### Multi-users support

Are LDAP and HTTP auth supported? **Yes**
Can the app be used by multiple users? **Yes**

#### Supported architectures

* x86-64 - [![Build Status](https://ci-apps.yunohost.org/ci/logs/spip%20%28Community%29.svg)](https://ci-apps.yunohost.org/ci/apps/spip/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/spip%20%28Community%29.svg)](https://ci-apps-arm.yunohost.org/ci/apps/spip/)

## Migrate from SPIP2

**This is not considered as stable yet, please do it with care and only for testing!**

This package handle the migration from SPIP2 to SPIP. For that, your
SPIP2 application must be **up-to-date** in YunoHost. To ensure that, execute:

```bash
sudo yunohost app upgrade -u https://github.com/YunoHost-Apps/spip2_ynh spip2 --debug
```

You will then have to upgrade your SPIP2 application with this repository.
This can only be done from the command-line interface - e.g. through SSH. Once you're connected, you simply have to execute the following:

```bash
sudo yunohost app upgrade -u https://github.com/YunoHost-Apps/spip_ynh spip2 --debug
```

The `--debug` option will let you see the full output. If you encounter any issue, please paste it.

Note that a cron job will be executed at some time after the end of this
command. You must wait that before doing any other application operations!
You should see that SPIP is installed after that.

## Links

 * Report a bug: https://github.com/YunoHost-Apps/spip_ynh/issues
 * App website: https://www.spip.net
 * YunoHost website: https://yunohost.org/

---

## Developers info

Please do your pull request to the [testing branch](https://github.com/YunoHost-Apps/spip_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
or
sudo yunohost app upgrade spip -u https://github.com/YunoHost-Apps/spip_ynh/tree/testing --debug
```
