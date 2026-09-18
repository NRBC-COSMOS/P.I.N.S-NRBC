# P.I.N.S-NRBC

Site statique regroupant les dossiers **P.I.N.S.** (Protocole d'Intervention NRBC
Spécialisé), classés par classe d'objet SCP.

## Structure

```
index.html          Accueil : présentation et accès aux trois classes
scp-safe.html       Liste des dossiers Safe
scp-euclid.html     Liste des dossiers Euclid
scp-keter.html      Liste des dossiers Keter
scp-<id>.html       Un dossier d'intervention par anomalie
assets/style.css    Feuille de style commune à toutes les pages
assets/favicon.svg  Icône du site
```

Aucune dépendance ni étape de build : ouvrir `index.html` dans un navigateur suffit.

## Ajouter un dossier

1. Copier un fichier `scp-<id>.html` existant de la même classe.
2. Remplacer partout l'identifiant (titre, fil d'Ariane, en-tête, référence).
3. Remplir les trois champs du dossier et retirer `class="empty"` des `<dd>`.
4. Ajouter la carte correspondante dans la page de classe (`scp-safe.html`,
   `scp-euclid.html` ou `scp-keter.html`) et mettre à jour le nombre de dossiers
   indiqué sur cette page et sur l'accueil.

## Thème

La couleur d'une page vient de l'attribut `data-classe` posé sur `<html>`
(`safe`, `euclid` ou `keter`). Tout le reste — fond, cartes, badges, boutons —
s'adapte automatiquement à partir des variables CSS définies dans
`assets/style.css`.
