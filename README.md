# DevExplorer2

DevExplorer est une application web simple et interactive permettant d'explorer des défis de développement classés par thème, avec des ressources utiles pour approfondir chaque sujet.

## 🔍 Aperçu

L'utilisateur peut sélectionner une catégorie de défis (comme **PHP** ou **Déploiement**) via un menu déroulant. Pour chaque défi, une fiche détaillée est affichée contenant :

- Une **image illustrative**
- Un **titre**
- Une **description**
- Un **concept clé**
- Une **liste de ressources** (liens externes)

L'application récupère dynamiquement les données depuis des fichiers JSON localisés dans le dossier `defis/`.

## 📁 Structure du projet

devexplorer2/
├── index.html # Page principale
├── defis/
│ ├── php.json # Données des défis PHP
│ └── deploiement.json # Données des défis Déploiement

## ✍️ Ajouter un nouveau défi
Créez un nouveau fichier .json dans le dossier defis/.

Respectez la structure suivante :

```json
{
  "Catégorie": [
    {
      "title": "Titre du défi",
      "description": "Description du défi",
      "concept": "Concept clé",
      "image_url": "URL de l'image",
      "resources": [
        "https://lien1.com",
        "https://lien2.com"
      ]
    }
  ]
}
```

Ajoutez l’option correspondante dans la balise `<select>` du fichier index.html.

## 📄 Licence
Ce projet est open-source.