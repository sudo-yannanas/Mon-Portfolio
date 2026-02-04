---
layout: default
title: zabbix
nav_order: 3
parent: Stage1-Docs
---

# Installation et Sécurisation d'un Domaine ADDS avec "Hello-My-Directory"

Cette documentation détaille la mise en œuvre d'un contrôleur de domaine Active Directory Domain Services (ADDS) en suivant les recommandations de sécurité actuelles, grâce à l'outil **Hello-My-Directory**.

## 1. Présentation de l'outil

**Hello-My-Directory** est un script PowerShell conçu pour automatiser l'installation d'Active Directory tout en appliquant immédiatement des configurations de durcissement (*hardening*). Contrairement à une installation classique, il structure nativement l'annuaire pour limiter les vecteurs d'attaque (Tiering model simplifié, délégations de droits, etc.).

> **Référence :** [Guide complet IT-Connect](https://www.it-connect.fr/comment-creer-un-domaine-active-directory-respectueux-des-bonnes-pratiques-de-securite/)

---

## 2. Processus d'installation en trois étapes

L'installation se déroule en trois phases distinctes, nécessitant chacune une exécution du script.

### Phase 1 : Configuration initiale et collecte d'informations

Lors du premier lancement, le script prépare l'environnement et demande les paramètres essentiels du futur domaine :

* **Nom du domaine** (ex: `corp.contoso.com`).
* **NetBIOS** du domaine.
* **Chemins d'accès** pour la base de données NTDS et les journaux.
* **Mot de passe de restauration** (DSRM).

### Phase 2 : Installation des rôles et promotion

La deuxième exécution installe les fonctionnalités Windows nécessaires et configure le serveur en tant que Contrôleur de Domaine.

* Installation du rôle **AD DS** et des outils d'administration RSAT.
* Configuration du rôle **DNS**.
* **Redémarrage obligatoire :** À la fin de cette étape, le serveur redémarre pour finaliser la promotion du domaine.

### Phase 3 : Sécurisation et Post-Configuration

Après le redémarrage, le script est lancé une dernière fois pour appliquer la couche de sécurité :

* **Structure d'Unités d'Organisation (OU) :** Création d'une hiérarchie propre.
* **Groupes de sécurité :** Création de groupes spécifiques pour l'administration.
* **Comptes de service :** Mise en place de comptes dédiés.
* **GPO de sécurité :** Application de stratégies de groupe pour durcir la configuration (désactivation de protocoles obsolètes, restrictions d'accès, etc.).

---

## 3. Conclusion et prochaines étapes

Une fois le script terminé, l'infrastructure Active Directory est opérationnelle et sécurisée selon les standards modernes.
