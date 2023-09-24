---
 

title: Terminal
description: Cette note sert est l'une des première à suivre afin de setup de manière agréable son terminal de développement.
date: 2023-01-05 08:49
tags: 
- FR
- Code
- Windows
heroImage: /Images/Terminal/Terminal_hero.png

---


# Terminal

- [Terminal](#terminal)
  - [Introduction](#introduction)
  - [Stack](#stack)
    - [Windows Terminal](#windows-terminal)
    - [Oh My Posh](#oh-my-posh)
      - [Installation](#installation)
      - [Customisation](#customisation)
    - [Terminal Icons](#terminal-icons)
    - [Git](#git)
  - [Facultatif](#facultatif)

## Introduction

Le terminal windows est un outil que les développeurs junior redoutent à tord. L'objectif de ce tutoriel va être de rendre le powershell beaucoup plus élegant et pratique d'utilisation. Aussi cela a pour but de rendre l'experience de développeur plus agréable et l'impliqué dans ses outils du quotidien.

Basé sur le [Tutoriel Officiel Microsoft](https://learn.microsoft.com/fr-fr/windows/terminal/tutorials/custom-prompt-setup)

## Stack

- Windows terminal
- Oh my posh
- Material icons for powershell
- Git

### Windows Terminal

| Description                                                                                                                                                                                                                       | Image                                                          |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| Pour avoir une expérience de terminal plus agréable, il est recommandé de passé par le **Terminal Windows**. Il n'est pas présent sur Windows 10 de base, il faut donc l'installer. Ce logiciel est dispo sur la Microsoft store. | ![Microsost Store](/Images/Terminal/ApplicationFrameHost_C5IMvE6HVk.png) |

Une fois l'installation terminée, on peut configurer le terminal pour avoir une config plus adaptée :

- Lancer le powershell avec les droits d'admin par defaut
- Choisir la transparence du terminal (Optionel)
- Avoir une Police qui supporte les charactères spéciaux venant de [Nerd Fonts](https://www.nerdfonts.com/font-downloads). Je recommande _Nerd Hack NF_ qui est sobre et stable.
  - Telecharger le zip et l'extraire.
  - Choisir dans le dossier la police qui convient ( _Hack Regular Nerd Font Complete Windows Compatible.ttf_ dans le cas de Hack NF) > Installer pour tous les utilisateurs.
  - L'ajouter comme Police par defaut dans les paramètres du Terminal. ![Police par Defaut](/Images/Terminal/WindowsTerminal_yumFGbqj8A.png)

### Oh My Posh

[Oh My Posh](https://ohmyposh.dev/docs) est un outil qui fonctionne sur tout les shell qui donne la possibilité de customisé l'apparence et les couleurs du terminal.

#### Installation

⚠️Pour les différentes étapes de l'installation, il sera surement necessaire de relancer le terminal à plusieurs reprise.

⚠️Bien vérifier que le terminal est en mode admin comme expliqué dans les étapes précedentes.

```bash
winget install oh-my-posh
```

Pour vous assurer que vous disposez des dernières mises à jour, vous pouvez utiliser la commande suivante :

```bash
winget upgrade oh-my-posh
```

Ensuite il est necessaire de créer un profile powershell. Si ce concept est nouveau suivre [ce tutoriel](https://lazyadmin.nl/powershell/powershell-profile/) afin de créer un fichier **$profile** powershell. Voici les étapes clés abregées:

- Vérifier si un profile est deja existant :

```bash
test-path $profile
```

- Si la réponse est false, il faut alors créer un fichier profile :

```bash
New-Item -Path $profile -Type File -Force
```

- Donner les droits au terminal d'utiliser les profils :

```bash
Set-ExecutionPolicy RemoteSigned
```

#### Customisation

Maintenant le choix est de votre coté pour choisir le [theme](https://ohmyposh.dev/docs/themes) que vous souhaitez utiliser pour votre terminal. En voici quelques un recommandés:
![Theme 1](/Images/Terminal/chrome_QEgtSPBCbk.png)
![Theme 1](/Images/Terminal/chrome_8ZZhvFBZFk.png)
...

Pour ajoutez le theme choisi, dans le terminal ouvrez le fichier **$profile**

```bash
notepad $profile
```

Dans le fichier txt ouvert, ajoutez la ligne en remplacant _NOM_DU_THEME_ par le theme choisi:

```txt
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\NOM_DU_THEME.omp.json" | Invoke-Expression
```

### Terminal Icons

Pour plus de lisibilité il est recommandé d'ajouter au fichier **$profile** une ligne qui va permettre d'afficher de la couleur pour chacun des types de fichier du terminal :

```txt
Import-Module -Name Terminal-Icons
```

![Terminal Icons](/Images/Terminal/Terminal_hero.png)

### Git

Git est un outil de versionning **OBLIGATOIRE** pour un développeur. Ainsi nous allons l'ajouter à notre terminal afin de pouvoir s'en servir sans avoir à ouvrir un bash spécifique pour les commandes Git.

- Télecharger l'executable sur le [site officiel](https://git-scm.com/downloads)
- Suivre la procédure d'installation par défaut.
- Faire un test pour bien s'assurer que git est installé
  ![Git dans le terminal](/Images/Terminal/WindowsTerminal_GosuVhBvYs.png)

## Facultatif

Il est recommander d'ajouter quelques utilitaires qui seront surement utile pour rendre votre windows proche d'un Linux et faciliter les installations des projets sous windows. Les processus d'installation ne seront pas détailler:

- Docker Desktop
- WSL 2 Distrib Ubuntu
- Chocolatey
- nvm/nvs (si projet sous node).


#### References
Tags : #FR #Code #Windows