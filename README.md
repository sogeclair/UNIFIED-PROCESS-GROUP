# Gestion des Processus - sommaire statique

Ce site permet de **visualiser et gérer les processus métiers**. Il repose sur un dépôt GitHub avec déploiement automatique via GitHub Pages. 

# Fonctionnalités principales 
- Consultation des processus par catégorie et recherche par mot-clé.  
- Affichage détaillé avec diagrammes SVG, images et fichiers associés.  
- Gestion centralisée via des archives ZIP.

# Comment ajouter un nouveau processus
### 1. Via l’interface web

- Cliquez sur le bouton `+` dans la barre latérale (section **Ajouter un processus**).  
- Sélectionnez votre fichier ZIP contenant le processus complet.  
- Le site déclenche automatiquement le workflow GitHub Actions pour extraire le contenu et mettre à jour le sommaire.
  -> Vous pouvez suivre l’avancement dans l’onglet **Actions** de GitHub.

### 2. Directement dans le dépôt GitHub

- Placez votre fichier ZIP dans le dossier `zips` à la racine du dépôt.  
- Le workflow GitHub Actions détecte automatiquement les nouveaux fichiers et met à jour le site.

## Fonctionnement technique

- Les ZIP sont extraits dans `docs/processus/`.  
- Le fichier `processus.json` est généré pour alimenter l’affichage dynamique.  
- Le site est **statique**, entièrement hébergé via GitHub Pages.  

## Bonnes pratiques

- Nommez vos ZIP clairement, sans caractères spéciaux. En commençant par le nom de la catégorie en toutes lettres (ex : FINANCE_ProcessV1.zip)
- Soyez patient pour les processus volumineux : le workflow peut prendre plusieurs minutes à déployer.
