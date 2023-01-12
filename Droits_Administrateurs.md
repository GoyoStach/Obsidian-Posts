# Avoir les droits d'administrateurs permanents sur windows Keyrus.

- Dans un premier temps il faudra faire une demande GLPI pour avoir les droits temporaires.
- Une fois les droits acquis, lancer la **Gestion de l'ordinateur** via la barre de recherche windows en tant qu'administrateur (via la combinaison identifiant/mdp fournis par l'IT).
- Aller dans Utilisateurs et groupes locaux

![Demo](/Images/Droits_Administrateurs/img1.png)

- Clique droit sur Administrateurs > Propriétés > Ajouter...
- Mettre le **_Nom.Prenom_** > Verifier les noms
- Popup ou il faut mettre son compte user dans l'Active Directory Keyrus.
- Normalement devrait auto-completer et afficher le mail keyrus.

![AD](/Images/Droits_Administrateurs/img2.png)

- Valider
- Redémarrer le PC.
- Tester si les droits d'admins sont maintenants bien actif pour le compte courant de l'utilisateur.

⚠️ Il se peut qu'il soit nécessaire d'être connecter au reseau Keyrus pour trouver son compte dans l'AD. ⚠️
