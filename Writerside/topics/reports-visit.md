# Rapports — Rapport de visite

La page **Créer un nouveau rapport** (ou **Reprendre le rapport** en mode édition) permet de rédiger un compte rendu de visite détaillé pour une copropriété : informations générales, copropriétaires présents, éléments observés par catégorie, images et conclusion.

---

## Raccourci d'utilisation

1. Accéder à la page via **Rapports** → **Nouveau rapport** → **Rapport de visite** ou depuis la [vue d'ensemble des rapports](reports-overview.md).
2. Remplir les **informations générales** (titre, date, type, rédacteur).
3. Sélectionner ou saisir la **copropriété associée**.
4. Ajouter les **copropriétaires présents** à la visite.
5. Ajouter des **catégories** d'observation (Façade, Ascenseurs, etc.).
6. Pour chaque catégorie, ajouter des **éléments** (Balcons, Murs, etc.) avec leurs observations.
7. Ajouter des **images** et des **informations complémentaires** par catégorie.
8. Rédiger la **conclusion** avec un résumé et des points à retenir.
9. **Enregistrer le brouillon** ou **Finaliser** le rapport.

---

## Informations générales

### Champs principaux

| Champ               | Description                                         | Obligatoire | Exemple                 |
|---------------------|-----------------------------------------------------|-------------|-------------------------|
| **Titre**           | Titre du rapport.                                   | Oui         | `Compte rendu immeuble` |
| **Date de visite**  | Date à laquelle la visite a eu lieu.                | Oui         | `28/11/2025`            |
| **Type de rapport** | Type de visite (Premier contact, Suivi, etc.).      | Oui         | `Premier contact`       |
| **Rédacteur**       | Utilisateur responsable de la rédaction du rapport. | Oui         | `Lionel Forni`          |

> Le type de rapport détermine les catégories disponibles pour structurer votre compte rendu.
>
{style="note"}

---

## Copropriété associée

### Sélection de la copropriété

| Champ                            | Description                                                            |
|----------------------------------|------------------------------------------------------------------------|
| **Sélectionner une copropriété** | Menu déroulant avec recherche par code ou nom.                         |
| **Identifiant**                  | Code unique de la copropriété (lecture seule, rempli automatiquement). |

### Adresse

Une fois la copropriété sélectionnée, l'adresse est **automatiquement préremplie** :

| Champ           | Description                            |
|-----------------|----------------------------------------|
| **Rue(s)**      | Adresse(s) de la copropriété.          |
| **Code postal** | Code postal.                           |
| **Ville**       | Ville.                                 |
| **Pays**        | Pays (sélecteur de pays).              |

> Vous pouvez modifier l'adresse si nécessaire, par exemple si la visite concerne un bâtiment spécifique dans un ensemble plus large.
>
{style="tip"}

---

## Copropriétaires présents

Cette section permet d'enregistrer les résidents présents lors de la visite.

### Ajout de copropriétaires

<tabs>
<tab title="Depuis la liste existante">

1. Cliquer dans le champ **Ajouter des copropriétaires**.
2. Sélectionner un résident dans la liste déroulante.
3. Cliquer sur **Ajouter un copropriétaire**.

</tab>
<tab title="Saisie manuelle">

1. Saisir directement `Prénom Nom` dans le champ.
2. Cliquer sur **Ajouter un copropriétaire**.
3. Le résident est ajouté temporairement au rapport.

**Format attendu** : `Prénom Nom` (séparés par un espace).

</tab>
</tabs>

### Tableau des résidents

Une fois ajoutés, les résidents apparaissent dans un tableau :

| Colonne     | Description                       |
|-------------|-----------------------------------|
| **Prénom**  | Prénom du résident.               |
| **Nom**     | Nom du résident.                  |
| **Email**   | Adresse email (si disponible).    |
| **Actions** | Supprimer le résident du rapport. |

---

## Catégories et éléments

### Ajouter une catégorie

1. Sélectionner une catégorie dans le menu déroulant en bas de page (ex. `Façade`, `Ascenseurs`, `Intérieur - Hall d'entrée`).
2. Cliquer sur **Ajouter une catégorie**.
3. Une nouvelle section apparaît avec un formulaire dédié.

> Les catégories disponibles dépendent du **type de rapport** sélectionné dans les informations générales.
>
{style="note"}

### Structure d'une catégorie

Chaque catégorie contient :

| Section                          | Description                                                             |
|----------------------------------|-------------------------------------------------------------------------|
| **Titre de la catégorie**        | Nom de la catégorie (ex. `Façade`).                                     |
| **Type - [Catégorie]**           | Menu déroulant pour ajouter des éléments prédéfinis (Balcons, Murs...). |
| **Liste des éléments**           | Éléments ajoutés avec leurs observations.                               |
| **Informations complémentaires** | Zone de texte libre pour ajouter des commentaires.                      |
| **Images**                       | Zone de drag & drop pour ajouter des photos.                            |

### Ajouter un élément à une catégorie

1. Dans la section de la catégorie, sélectionner un type d'élément (ex. `Huisseries`).
2. Cliquer sur l'icône **+** (Ajouter).
3. Un nouvel élément apparaît dans la liste avec les champs suivants :

| Champ              | Description                                                | Obligatoire | Exemple               |
|--------------------|------------------------------------------------------------| ----------- |-----------------------|
| **Désignation**    | Nom de l'élément observé.                                  | Oui         | `Huisseries`          |
| **Spécifications** | Matériau ou caractéristique (Aluminium, Bois, etc.).       | Non         | `Aluminium`           |
| **Observations**   | Remarques ou commentaires libres.                          | Non         | `Présence de rouille` |
| **État**           | État général (Excellent, Bon, Correct, Médiocre, Mauvais). | Oui*        | `Médiocre`            |

> *L'état est obligatoire pour la plupart des éléments, sauf exceptions (ex. nombre d'ascenseurs, etc.).
>
{style="warning"}

### Supprimer un élément ou une catégorie

- **Élément** : cliquer sur l'icône **poubelle** dans l'en-tête de l'élément.
- **Catégorie** : cliquer sur l'icône **poubelle** dans l'en-tête de la catégorie (supprime tous les éléments associés).

---

## Images

Chaque catégorie peut contenir plusieurs images illustrant les observations.

### Ajouter des images

<tabs>
<tab title="Par drag & drop">

1. Faire glisser une ou plusieurs images depuis votre explorateur de fichiers.
2. Déposer dans la zone **Images** de la catégorie.

</tab>
<tab title="Par sélection">

1. Cliquer sur la zone **Images**.
2. Sélectionner un ou plusieurs fichiers depuis votre appareil.

</tab>
</tabs>

> Formats acceptés : `.jpg`, `.jpeg`, `.png`. Les images sont automatiquement uploadées lors de l'enregistrement du rapport.
>
{style="tip"}

---

## Conclusion

La section **Conclusion** permet de synthétiser le rapport et de lister les actions prioritaires.

### Résumé

Zone de texte libre pour rédiger une synthèse générale du rapport.

**Exemple** :  
*"L'immeuble nécessite des travaux urgents sur la façade avant et le remplacement de plusieurs fenêtres. La toiture est en bon état général."*

### Actions / Points à retenir

Liste structurée des éléments importants identifiés lors de la visite.

| Champ           | Description                                          | Exemple                                      |
|-----------------|------------------------------------------------------|----------------------------------------------|
| **Priorité**    | Niveau d'importance (1 = le plus urgent).            | `1`, `2`, `3`                                |
| **Libellé**     | Titre court de l'action.                             | `Réparer balcons`                            |
| **Description** | Description détaillée ou contexte supplémentaire.    | `Présence de rouille, risque de chute`       |

### Ajouter un élément de conclusion

1. Cliquer sur **Ajouter un élément de conclusion**.
2. Remplir les champs (Priorité, Libellé, Description).
3. Répéter pour chaque point important.

### Supprimer un élément

Cliquer sur l'icône **poubelle** à droite de l'élément.

---

## Enregistrement et finalisation

### Actions disponibles

| Bouton                       | Description                                                                                                   |
|------------------------------|---------------------------------------------------------------------------------------------------------------|
| **Enregistrer le brouillon** | Sauvegarde le rapport avec le statut `Brouillon`. Vous pourrez le modifier ultérieurement.                    |
| **Finaliser**                | Valide et finalise le rapport avec le statut `Finalisé`. Le rapport est alors considéré comme terminé.        |

> Un rapport finalisé peut toujours être modifié via l'action **Reprendre la saisie** depuis la [vue d'ensemble](reports-overview.md), mais cela n'est pas recommandé.
>
{style="warning"}

---

## Mode édition

Lorsque vous **reprenez la saisie** d'un rapport existant (brouillon ou finalisé), le formulaire est **automatiquement prérempli** avec toutes les données du rapport :

- Informations générales
- Copropriété et adresse
- Copropriétaires présents
- Catégories, éléments et observations
- Images
- Conclusion

Vous pouvez alors modifier n'importe quel champ et **Enregistrer** ou **Finaliser** à nouveau.

---

## Exemples d'utilisation

<tabs>
<tab title="Créer un rapport de visite complet">

1. Remplir les **informations générales** (titre, date, type, rédacteur).
2. Sélectionner la **copropriété** concernée.
3. Ajouter les **résidents présents**.
4. Ajouter une catégorie `Façade` :
   - Ajouter un élément `Balcons` → État `Médiocre` → Observation `Rouille visible`.
   - Ajouter une image de la façade.
5. Ajouter une catégorie `Toiture` :
   - Ajouter un élément `Tuiles` → État `Bon`.
6. Rédiger la **conclusion** avec un résumé et 2 actions prioritaires.
7. Cliquer sur **Finaliser**.

</tab>
<tab title="Enregistrer un brouillon pour finir plus tard">

1. Remplir partiellement le formulaire.
2. Cliquer sur **Enregistrer le brouillon**.
3. Retrouver le rapport dans la [vue d'ensemble](reports-overview.md) avec le statut `Brouillon`.
4. Cliquer sur la ligne pour reprendre la saisie.

</tab>
<tab title="Reprendre un rapport finalisé">

1. Depuis la [vue d'ensemble](reports-overview.md), cliquer sur la ligne du rapport finalisé.
2. Le formulaire s'ouvre avec toutes les données.
3. Modifier les informations nécessaires.
4. **Enregistrer** à nouveau.

</tab>
</tabs>

