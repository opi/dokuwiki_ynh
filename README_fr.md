# DokuWiki pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/dokuwiki.svg)](https://dash.yunohost.org/appci/app/dokuwiki) ![](https://ci-apps.yunohost.org/ci/badges/dokuwiki.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/dokuwiki.maintain.svg)  
[![Installer DokuWiki avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=dokuwiki)

*[Read this readme in english.](./README.md)*

> *Ce package vous permet d'installer DokuWiki rapidement et simplement sur un serveur YunoHost.  
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

DokuWiki est un logiciel wiki Open Source simple à utiliser et très polyvalent qui ne nécessite pas de base de données. Il est apprécié par les utilisateurs pour sa syntaxe propre et lisible. La facilité de maintenance, de sauvegarde et d'intégration en fait un favori d'administrateur. Des contrôles d'accès et des connecteurs d'authentification intégrés rendent DokuWiki particulièrement utile dans le contexte de l'entreprise et le grand nombre de plugins apportés par sa communauté dynamique permettent un large éventail de cas d'utilisation au-delà d'un wiki traditionnel.

**Version incluse:** 2020-07-29

## Captures d'écran

![Capture d'écran](sources/DokuWiki_Screenshot.png)

## Démo

* [Démo YunoHost](https://demo.yunohost.org/dokuwiki/doku.php?id=start&do=login&u=demo&p=demo)

## Configuration

## Documentation

* Documentation officielle : https://www.dokuwiki.org/manual
* Documentation YunoHost : https://yunohost.org/fr/app_dokuwiki

## Caractéristiques spécifiques YunoHost

* Fonctionne avec les utilisateurs YunoHost ainsi que le SSO - i.e. button de déconnexion
* Définit un utilisateur "administrateur" lors de l'installation
* Droits d'édition par défaut du wiki définis en lecture seule afin que les invités ne puissent éditer les pages. (Nécessaire surtout lorsque le wiki est public pour éviter le spam et le vandalisme. Peut être changé depuis la partie administration du wiki)
* Lors de la mise à jour, les plugins officiels sont également mis à jour. Nous vous recommandons toutefois de vérifier le bon fonctionnement des plugins dans le panneau d'administration après cette opération. Nous ne pouvons pas savoir si des plugins spéciaux posent problèmes...

### Architectures matérielles supportées

* x86-64 - [![Build Status](https://ci-apps.yunohost.org/ci/logs/dokuwiki%20%28Apps%29.svg)](https://ci-apps.yunohost.org/ci/apps/dokuwiki/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/dokuwiki%20%28Apps%29.svg)](https://ci-apps-arm.yunohost.org/ci/apps/dokuwiki/)

## Limitations

* Impossible d'ajouter et d'utiliser les utilisateurs internes de DokuWiki, seulement ceux de YunoHost (travail nécessaire pour [authchained plugin](https://www.dokuwiki.org/plugin:authchained))

## Informations additionnelles

### Historique des versions

## Liens

 * Signaler un bug : https://github.com/YunoHost-Apps/dokuwiki_ynh/issues
 * Site de l'application : https://www.dokuwiki.org
 * Dépôt de l'application principale : https://github.com/splitbrain/dokuwiki
 * Site web YunoHost : https://yunohost.org/

---

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/dokuwiki_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/dokuwiki_ynh/tree/testing --debug
ou
sudo yunohost app upgrade dokuwiki -u https://github.com/YunoHost-Apps/dokuwiki_ynh/tree/testing --debug
```
