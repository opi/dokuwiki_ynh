# DokuWiki for YunoHost

[![Integration level](https://dash.yunohost.org/integration/dokuwiki.svg)](https://dash.yunohost.org/appci/app/dokuwiki) ![](https://ci-apps.yunohost.org/ci/badges/dokuwiki.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/dokuwiki.maintain.svg)  
[![Install DokuWiki with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=dokuwiki)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install DokuWiki quickly and simply on a YunoHost server.  
If you don't have YunoHost, please see [here](https://yunohost.org/#/install) to know how to install and enjoy it.*

## Overview

DokuWiki is a simple to use and highly versatile Open Source wiki software that doesn't require a database. It is loved by users for its clean and readable syntax. The ease of maintenance, backup and integration makes it an administrator's favorite. Built in access controls and authentication connectors make DokuWiki especially useful in the enterprise context and the large number of plugins contributed by its vibrant community allow for a broad range of use cases beyond a traditional wiki.

**Shipped version:** 2020-07-29

## Screenshots

![Screenshot of DokuWiki main window](sources/DokuWiki_Screenshot.png)

## Demo

* [YunoHost demo](https://demo.yunohost.org/dokuwiki/doku.php?id=start&do=login&u=demo&p=demo)

## Configuration

## Documentation

* Official documentation: https://www.dokuwiki.org/manual
* YunoHost documentation: https://yunohost.org/en/app_dokuwiki

## YunoHost specific features

* Integrate with YunoHost users and SSO - i.e. logout button
* Allow one user to be the "administrator" (set at the installation)
* Default authorization is set as read only so guest people cannot edit pages. (Especially needed if wiki is public to avoid spam and defacing. Can be changed from admin panel)
* During the upgrade, official plugins are also upgraded. We recommend that you should check that they run properly in the administration panel after the upgrade. We cannot know if some plugins are broken...

### Supported architectures

* x86-64 - [![Build Status](https://ci-apps.yunohost.org/ci/logs/dokuwiki%20%28Apps%29.svg)](https://ci-apps.yunohost.org/ci/apps/dokuwiki/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/dokuwiki%20%28Apps%29.svg)](https://ci-apps-arm.yunohost.org/ci/apps/dokuwiki/)

## Limitations

* Cannot create or login with DokuWiki internal users, only users from YunoHost (Work needed for [authchained plugin](https://www.dokuwiki.org/plugin:authchained))

## Links

* Report a bug: https://github.com/YunoHost-Apps/dokuwiki_ynh/issues
* App website: https://www.dokuwiki.org
* Upstream app repository: https://github.com/splitbrain/dokuwiki
* YunoHost website: https://yunohost.org

---

## Developers infos

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/dokuwiki_ynh/tree/testing)

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/dokuwiki_ynh/tree/testing --debug
or
sudo yunohost app upgrade dokuwiki -u https://github.com/YunoHost-Apps/dokuwiki_ynh/tree/testing --debug
```
