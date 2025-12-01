# Copropriétés — Détail

La page **Détail d'une copropriété** centralise toutes les informations relatives à une copropriété : ses données générales, les rapports associés, ainsi que la liste complète des résidents.

---

## Raccourci d'utilisation

1. Accéder à la page via la [liste des copropriétés](condominiums-list.md) ou la [vue d'ensemble](condominiums-overview.md).
2. Consulter les **informations de la copropriété** (code, adresse, année de construction).
3. Cliquer sur **Modifier les informations** pour [éditer la fiche](condominiums-edit.md).
4. Consulter les **rapports** existants et gérer leurs statuts.
5. Cliquer sur **Nouveau rapport** pour [créer un rapport](reports-create.md).
6. Gérer la liste des **résidents** (consulter, ajouter, modifier, supprimer).

---

## Informations de la copropriété

Cette section présente les données essentielles de la copropriété.

### Données affichées

| Champ                     | Description                           | Exemple                |
|---------------------------|---------------------------------------|------------------------|
| **Code**                  | Identifiant unique de la copropriété. | `CDM 001`              |
| **Année de construction** | Année de construction du bâtiment.    | `1895`                 |
| **Rue**                   | Adresse(s) de la copropriété.         | `12 avenue Montrosier` |
| **Ville**                 | Code postal et ville.                 | `75016 Paris, France`  |
| **Photo**                 | Image de la copropriété.              |                        |

### Bouton d'action

Le bouton **Modifier les informations** permet d'accéder au [formulaire d'édition](condominiums-edit.md) de la copropriété.

> Les informations modifiées sont immédiatement reflétées dans toutes les pages (liste, vue d'ensemble).
>
{style="note"}

---

## Rapports

Cette section liste tous les rapports créés pour cette copropriété.

### Structure du tableau

| Colonne       | Description                                                  | Exemple                                                                     |
|---------------|--------------------------------------------------------------|-----------------------------------------------------------------------------|
| **Titre**     | Nom du rapport (cliquable pour ouvrir le rapport).           | `Compte rendu immeuble`                                                     |
| **Date**      | Date de création du rapport.                                 | `28/11/2025`                                                                |
| **Type**      | Type de rapport (badge coloré).                              | `Visite`                                                                    |
| **Rédacteur** | Nom de l'utilisateur ayant créé le rapport.                  | `Frederic Voirin`                                                           |
| **Statut**    | État actuel du rapport (badge avec couleur distinctive).     | `Finalisé`, `Brouillon`                                                     |
| **Actions**   | Icônes d'actions rapides (modifier, télécharger, supprimer). | ![edit.svg](edit.svg) ![download.svg](download.svg) ![trash.svg](trash.svg) |

### Détail des actions rapides

<table>
<tr>
<td>Icône</td>
<td>Action</td>
<td>Description</td>
</tr>
<tr>
<td>
<img src="edit.svg" alt="edit"/>
</td>
<td><b>Modifier</b></td>
<td>Ouvre le rapport en mode édition.</td>
</tr>
<tr>
<td>
<img src="download.svg" alt="download"/>
</td>
<td><b>Télécharger</b></td>
<td>Permet de télécharger.</td>
</tr>
<tr>
<td>
<img src="trash.svg" alt="delete"/>
</td>
<td><b>Supprimer</b></td>
<td>Supprime définitivement le rapport (confirmation requise).</td>
</tr>
</table>

### Création d'un rapport

Le bouton **Nouveau rapport** (en bas à droite de la section) ouvre le [formulaire de création d'un rapport](reports-create.md) pour cette copropriété.

> Un rapport peut être modifié a tout moment, même après avoir été finalisé, toutefois cela n'est pas recommandé.
>
{style="tip"}

---

## Résidents

Cette section affiche la liste complète des résidents de la copropriété.

### Colonnes du tableau

| Colonne     | Description                                     | Exemple                                       |
|-------------|-------------------------------------------------|-----------------------------------------------|
| **Prénom**  | Prénom du résident.                             | `Laura`, `Sylvain`                            |
| **Nom**     | Nom de famille du résident.                     | `Robert`, `Morawiec`                          |
| **Email**   | Adresse email du résident.                      | `lrobert@gmail.com`                           |
| **Actif**   | Statut du résident (actif ou inactif).          | Badge `Actif` (bleu) ou `Inactif` (gris)      |
| **Actions** | Icônes d'actions rapides (modifier, supprimer). | ![edit.svg](edit.svg) ![trash.svg](trash.svg) |

### Statuts des résidents

| Badge              | Signification                                      | Utilisation                                                      |
|--------------------|----------------------------------------------------|------------------------------------------------------------------|
| **Actif** (bleu)   | Résident actuellement présent dans la copropriété. |                                                                  |
| **Inactif** (gris) | Ancien résident                                    | Permet de conserver l'historique sans encombrer la liste active. |

### Actions sur les résidents

| Icône                   | Action        | Description                                                     |
|-------------------------|---------------|-----------------------------------------------------------------|
| ![edit.svg](edit.svg)   | **Modifier**  | Ouvre un formulaire pour modifier les informations du résident. |
| ![trash.svg](trash.svg) | **Supprimer** | Supprime définitivement le résident (confirmation requise).     |

### Ajout de résidents

| Bouton                  | Description                                                                                        |
|-------------------------|----------------------------------------------------------------------------------------------------|
| **Importer**            | Permet d'importer une liste de résidents (depuis un export en `EXCEL` depuis le logiciel `spirit`. |
| **Ajouter un résident** | Ouvre un formulaire pour ajouter manuellement un nouveau résident.                                 |

> L'import de résidents en masse facilite l'ajout de nombreux résidents simultanément. Assurez-vous que votre fichier respecte le format attendu.
>
{style="tip"}

---

## Supprimer la copropriété

Cette section permet de **supprimer définitivement** la copropriété et toutes ses données associées un message de confirmation est affiché avant la suppression finale.

> Une fois la copropriété supprimée, cette action est irréversible.
> 
{style="warning"}