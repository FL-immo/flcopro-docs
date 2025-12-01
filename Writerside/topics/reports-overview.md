# Rapports — Vue d'ensemble

La page **Vue d'ensemble des rapports** centralise tous les rapports liés aux copropriétés et permet de les filtrer, consulter et gérer facilement.

---

## Raccourci d'utilisation

1. Accéder à **Rapports** → **Vue d'ensemble** depuis le menu principal.
2. Utiliser les **filtres** pour affiner la liste (uniquement mes rapports, type, copropriété, dates).
3. **Cliquer sur une ligne** pour reprendre la saisie du rapport.
4. Utiliser les **icônes d'actions** pour gérer les rapports (éditer, télécharger, regénérer, supprimer).

---

## Filtres de recherche

La page offre plusieurs filtres pour affiner la liste des rapports :

| Filtre                      | Description                                                        |
|-----------------------------|--------------------------------------------------------------------|
| **Uniquement mes rapports** | Toggle pour n'afficher que vos rapports (sinon tous les rapports). |
| **Type**                    | Sélection du type de rapport (par défaut : `Tous`).                |
| **Copropriété**             | Recherche par code ou nom de copropriété.                          |
| **Du / Au**                 | Plage de dates pour filtrer les rapports par période.              |

> Par défaut, seuls vos rapports sont affichés. Désactivez le toggle pour voir tous les rapports de l'équipe.
>
{style="tip"}

---

## Liste des rapports

Les rapports sont présentés sous forme de tableau avec les colonnes suivantes :

| Colonne      | Description                                 |
|--------------|---------------------------------------------|
| **Date**     | Date de création du rapport.                |
| **Type**     | Type de rapport (badge : `Visite`, etc.).   |
| **Immeuble** | Nom de la copropriété associée.             |
| **Statut**   | État du rapport : `Brouillon`, `Finalisé`.  |
| **Auteur**   | Nom de l'utilisateur ayant créé le rapport. |
| **Actions**  | Icônes d'actions rapides.                   |

### Statuts des rapports

| Badge                  | Signification                                |
|------------------------|----------------------------------------------|
| **Brouillon** (orange) | Rapport en cours de rédaction, non finalisé. |
| **Finalisé** (bleu)    | Rapport terminé et validé.                   |

---

## Actions disponibles

Chaque rapport dispose de 5 actions rapides accessibles via les icônes :

| Icône                                   | Action                  | Description                                                                                                                           |
|-----------------------------------------|-------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| ![external-link.svg](external-link.svg) | **Reprendre la saisie** | Ouvre le [formulaire de création](reports-create.md) avec tous les champs préremplis. Disponible quand le rapport est en `brouillon`. |
| ![edit.svg](edit.svg)                   | **Éditer**              | Ouvre l'éditeur WYSIWYG pour modifier le contenu du rapport finalisé.                                                                 |
| ![download.svg](download.svg)           | **Télécharger**         | Génère et télécharge le rapport en PDF.                                                                                               |
| ![retry.svg](retry.svg)                 | **Régénérer**           | Remet le rapport dans l'état "après saisie" (avant édition WYSIWYG).                                                                  |
| ![trash.svg](trash.svg)                 | **Supprimer**           | Supprime définitivement le rapport (confirmation requise).                                                                            |

### Cliquer sur une ligne

**Cliquer n'importe où sur la ligne du rapport** (hors zone Actions) ouvre automatiquement l'action **Reprendre la saisie**, même si le rapport est finalisé.

> Cette action est utile pour créer un nouveau rapport similaire en réutilisant les données d'un rapport existant.
>
{style="tip"}

---

## Interactions

<tabs>
<tab title="Filtrer mes rapports uniquement">

1. Activer le toggle **Uniquement mes rapports**.
2. Seuls vos rapports s'affichent dans la liste.

</tab>
<tab title="Filtrer par copropriété">

1. Saisir le code ou le nom dans le champ **Copropriété**.
2. La liste se met à jour automatiquement.

</tab>
<tab title="Filtrer par période">

1. Sélectionner une date de début dans **Du**.
2. Sélectionner une date de fin dans **Au**.
3. Seuls les rapports dans cette plage s'affichent.

</tab>
<tab title="Reprendre la saisie d'un rapport">

1. Cliquer sur la ligne du rapport (ou sur l'icône ![external-link.svg](external-link.svg)).
2. Le [formulaire de création](reports-create.md) s'ouvre avec tous les champs préremplis.
3. Modifier les données selon vos besoins.
4. Enregistrer comme nouveau rapport ou mettre à jour.

</tab>
</tabs>

