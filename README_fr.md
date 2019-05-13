# Dokuwiki pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/dokuwiki.svg)](https://dash.yunohost.org/appci/app/dokuwiki)  
[![Installer DokuWiki grâce à YunoHost](https://install-app.yunohost.org/install-with-yunohost.png)](https://install-app.yunohost.org/?app=dokuwiki)

*[Read this readme in english.](./README.md)* 

> *Ce package vous permet d'installer Dokuwiki rapidement et simplement sur un serveur Yunohost.  
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

DokuWiki est un logiciel wiki Open Source simple à utiliser et très polyvalent qui ne nécessite pas de base de données. Il est apprécié par les utilisateurs pour sa syntaxe propre et lisible. La facilité de maintenance, de sauvegarde et d'intégration en fait un favori d'administrateur. Des contrôles d'accès et des connecteurs d'authentification intégrés rendent DokuWiki particulièrement utile dans le contexte de l'entreprise et le grand nombre de plugins apportés par sa communauté dynamique permettent un large éventail de cas d'utilisation au-delà d'un wiki traditionnel.

**Version incluse:** 2018-04-22a "Greebo"

## Captures d'écran

![](https://www.dokuwiki.org/_media/dokuwikimainwindow.png)

## Démo

* [Démo YunoHost](https://demo.yunohost.org/dokuwiki/doku.php?id=start&do=login&u=demo&p=demo)

## Configuration

## Documentation

* Documentation officielle: https://www.dokuwiki.org/manual
* Documentation YunoHost: https://yunohost.org/#/app_dokuwiki

## Caractéristiques spécifiques YunoHost

* Fonctionne avec les utilisateurs YunoHost ainsi que le SSO - i.e. button de déconnexion
* Définit un utilisateur "administrateur" lors de l'installation
* Droits d'édition par défaut du wiki définis en lecture seule afin que les invités ne puissent éditer les pages. (Nécessaire surtout lorsque le wiki est public pour éviter le spam et le vandalisme. Peut être changé depuis la partie administration du wiki)
* Lors de la mise à jour, les plugins officiels sont également mis à jour. Nous vous recommandons toutefois de vérifier le bon fonctionnement des plugins dans le panneau d'administration après cette opération. Nous ne pouvons pas savoir si des plugins spéciaux posent problèmes...

### Architectures matérielles supportées

* x86-64b - [![Build Status](https://ci-apps.yunohost.org/ci/logs/dokuwiki%20%28Official%29.svg)](https://ci-apps.yunohost.org/ci/apps/dokuwiki/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/dokuwiki%20%28Official%29.svg)](https://ci-apps-arm.yunohost.org/ci/apps/dokuwiki/)
* Jessie x86-64b - [![Build Status](https://ci-stretch.nohost.me/ci/logs/dokuwiki%20%28Official%29.svg)](https://ci-stretch.nohost.me/ci/apps/dokuwiki/)

## Limitations

* Impossible d'ajouter et d'utiliser les utilisateurs internes de DokuWiki, seulement ceux de Yunohost (travail nécessaire pour [authchained plugin](https://www.dokuwiki.org/plugin:authchained))

## Informations additionnelles

### Historique des versions

* *Many missing - List taken from previous documentation*
* 07 Mar 2017 - Update app
* 11 Feb 2017 - Create script app

## Liens

 * Signaler un bug: https://github.com/YunoHost-Apps/dokuwiki_ynh/issues
 * Site de l'application:https://www.dokuwiki.org
 * Site web YunoHost: https://yunohost.org/

---

## Informations pour les développeurs

**Seulement si vous voulez utiliser une branche de test pour le codage, au lieu de fusionner directement dans la banche principale.**

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/REPLACEBYYOURAPP_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/dokuwiki_ynh/tree/testing --debug
ou
sudo yunohost app upgrade dokuwiki -u https://github.com/YunoHost-Apps/dokuwiki_ynh/tree/testing --debug
```
