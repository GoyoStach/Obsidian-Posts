---
 
layout: '../../layouts/BlogPost.astro'
title: Onboarding Logiciel
description: 
date: 2023-03-07 15:57
tags: 
- FR 
- TS
heroImage: /Images/Onboarding_Logiciel/Onboarding_Logiciel_hero.jpg
---
# Onboarding Logiciel

- [Onboarding Logiciel](#onboarding-logiciel)
  - [Logiciels](#logiciels)
    - [Visual Studio Code](#visual-studio-code)
    - [Docker](#docker)
    - [DBeaver](#dbeaver)
    - [Postman](#postman)
    - [KeepassXC](#keepassxc)
    - [mRemoteNG](#mremoteng)
    - [Firefox, Edge, Chrome](#firefox-edge-chrome)
  - [VS Code](#vs-code)
    - [Extension Git](#extension-git)
      - [Git Graph](#git-graph)
      - [Git Lens](#git-lens)
    - [Extension Qualité code](#extension-qualité-code)
      - [Prettier](#prettier)
      - [EsLint](#eslint)
      - [Docker](#docker-1)
      - [Sonar Lint *(Optional)*](#sonar-lint-optional)
      - [ES7+ React/Redux snippets *(Optional)*](#es7-reactredux-snippets-optional)
    - [Extension confort visuel](#extension-confort-visuel)
      - [Mardown All in One](#mardown-all-in-one)
      - [Rainbow CSV](#rainbow-csv)
      - [Material Icon Theme](#material-icon-theme)
      - [Color Highlight](#color-highlight)
      - [:emojisense:](#emojisense)
      - [Theme](#theme)

## Logiciels

### Visual Studio Code

Visual Studio Code est un éditeur de code extensible développé par Microsoft pour Windows, Linux et macOS. Les fonctionnalités incluent la prise en charge du débogage, la mise en évidence de la syntaxe, la complétion intelligente du code, les snippets, la refactorisation du code et Git intégré.

Outil principal, [voir section dedié pour la customisation](#vs-code)

### Docker 

![Docker Desktop](/Images/Onboarding_Logiciel/Docker_Desktop.png)

Docker est une plateforme permettant de lancer certaines applications dans des conteneurs logiciels.

- Permet d'avoir un environnement stable et similaire pour tout les developpeurs.
- Onboaridng rapide sur différents projet.
- Utilisé pour la CI/CD. Outil de devOps très important & puissant.

Docker est un outil complet et complexe. Il ne sera pas nécessaire de comprendre en détail la création et la customisation de configuration de projet sous Docker. Néanmoins certaines commandes de bases seront à connaitre.(Ecrit dans les différents readme des projets).

### DBeaver


![DBeaver](/Images/Onboarding_Logiciel/dbeaver.png)

DBeaver est un logiciel permettant l'administration et le requêtage de base de données.

- Outil graphique permetant la visualisation de base de données
- Permet la modification via interface graphique
- Compaptible avec quasiment tout les languages SQL et base de données relationnels.
- Sera parfois integré à la config de dev docker

### Postman

![Postman](/Images/Onboarding_Logiciel/Postman.png)

Postman est une application permettant de tester des API.

- Interface graphique pour tester ces API
- Possibilité d'ograniser ses différents endpoints
- Creation de configuration en fonction du projet
- Export de collection pour partager ses endpoints 

### KeepassXC

![KeepassXC](/Images/Onboarding_Logiciel/keepassxc.png)

KeePassXC est un gestionnaire de mots de passe gratuit et open-source

- Obligatoire pour des raisons de sécurité
- Bonne pratique à avoir
- Permet le partage de fichier de mot de passe lors d'arrivé sur des projets
- Auto generation de mot de passe complexe
- Stockage des mdp en local

### mRemoteNG

![mRemote](/Images/Onboarding_Logiciel/mRemoteNG.png)

mRemoteNG is a fork of mRemote: an open source, tabbed, multi-protocol, remote connections manager for Windows. mRemoteNG adds bug fixes and new features to mRemote and allows you to view all of your remote connections in a simple yet powerful tabbed interface.

- Utile pour les connexion aux serveurs
- Organisation possible pour différents projets
- Interface graphique ou CLI en fonction du serveur

### Firefox, Edge, Chrome

![navigateur](/Images/Onboarding_Logiciel/navigateur.jpg)

Surtout pour les devs front afin de tester les différentes compaptibilités en fonction du navigateur.

![cssDemo](/Images/Onboarding_Logiciel/cssdemo.png)

Certains navigateur sont plus adapaté que d'autre pour certaines étapes de débugging

- CORS ==> Firefox
- ...

## VS Code

Visual Studio code sera votre outil de travail principal en tant que dev. Il vous servira a visualiser les fichiers de devéloppement mais pas que. C'est un puissant logiciel qui va aussi permettre de gérer par exemple le versionning git, la visualisation de markdown, etc.

Afin de prendre en main VSCode, voici une liste de plusieurs extension recommandées.

### Extension Git


#### Git Graph
![gitGraph](/Images/Onboarding_Logiciel/gitgraph.png)

#### Git Lens
![gitLens](/Images/Onboarding_Logiciel/gitlens.png)

### Extension Qualité code


#### Prettier
![Prettier](/Images/Onboarding_Logiciel/prettier.png)

#### EsLint
![eslint](/Images/Onboarding_Logiciel/eslint.png)

#### Docker

![docker](/Images/Onboarding_Logiciel/docker.png)

#### Sonar Lint *(Optional)*
![sonar](/Images/Onboarding_Logiciel/sonarlint.png)

#### ES7+ React/Redux snippets *(Optional)*
![es7](/Images/Onboarding_Logiciel/es7.png)


### Extension confort visuel
#### Mardown All in One

![markdown](/Images/Onboarding_Logiciel/markdown.png)
#### Rainbow CSV

![rainbowcsv](/Images/Onboarding_Logiciel/rainbowcsv.png)
#### Material Icon Theme

![materialicon](/Images/Onboarding_Logiciel/materialicon.png)

#### Color Highlight
![colorHighlight](/Images/Onboarding_Logiciel/highlightcolor.png)

#### :emojisense:
![emojisense](/Images/Onboarding_Logiciel/emojisense.png)
#### Theme

Il est recommandé d'installer un theme afin de personnalisé son experience en fonction de ses gouts. [En voici quelques uns](https://www.commentcoder.com/themes-vs-code/)






#### References
Tags : #FR #TS