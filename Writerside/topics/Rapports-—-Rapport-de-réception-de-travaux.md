# Rapports — Rapport de réception de travaux

La page **Créer un nouveau rapport de réception de travaux** (ou **Reprendre le rapport de réception** en mode édition) permet de documenter la réception de travaux effectués dans une copropriété : informations générales, entrepreneur, description des travaux, non-conformités constatées, observations et commentaires.

---

## Raccourci d'utilisation

1. Accéder à la page via **Rapports** → **Nouveau rapport** → **Réception de travaux** ou depuis la [vue d'ensemble des rapports](reports-overview.md).
2. Remplir les **informations générales** (titre, date, type de réception, rédacteur, statut).
3. Sélectionner la **copropriété associée**.
4. Ajouter les **copropriétaires présents** (optionnel).
5. Renseigner les **informations sur l'entrepreneur**.
6. Décrire les **travaux réalisés**.
7. Ajouter les **non-conformités** constatées avec photos.
8. Ajouter les **constats** (autres observations) avec photos.
9. Rédiger les **commentaires généraux**.
10. **Enregistrer le brouillon** ou **Finaliser** le rapport.

---

## Informations générales

### Champs principaux

| Champ                     | Description                                          | Obligatoire | Exemple                         |
|---------------------------|------------------------------------------------------|-------------|---------------------------------|
| **Titre**                 | Titre du rapport.                                    | Oui         | `Réception travaux toiture`     |
| **Date de la réception**  | Date à laquelle la réception a eu lieu.              | Oui         | `20/01/2026`                    |
| **Type de réception**     | Type de réception (Provisoire, Définitive, etc.).    | Oui         | `Réception provisoire`          |
| **Rédacteur**             | Utilisateur responsable de la rédaction du rapport.  | Oui         | `Lionel Forni`                  |
| **Statut de la réception**| Statut global (Acceptée, Refusée, Avec réserves).    | Oui         | `Acceptée avec réserves`        |

> Le statut de la réception reflète le résultat global de la réception des travaux.
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

---

## Copropriétaires présents

Cette section permet d'enregistrer les résidents présents lors de la réception (optionnel).

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

**Format attendu** : `Prénom Nom` (séparés par un espace).

</tab>
</tabs>

---

## Informations sur l'entrepreneur

Cette section regroupe les coordonnées de l'entreprise ayant réalisé les travaux.

| Champ                       | Description                           | Obligatoire | Exemple                  |
|-----------------------------|---------------------------------------|-------------|--------------------------|
| **Nom de l'entreprise**     | Nom de l'entreprise.                  | Oui         | `Entreprise Dupont`      |
| **Contact**                 | Nom du contact principal.             | Non         | `M. Dupont`              |
| **Téléphone**               | Numéro de téléphone.                  | Non         | `01 23 45 67 89`         |
| **Email**                   | Adresse email.                        | Non         | `contact@entreprise.fr`  |
| **N° de commande / devis**  | Référence de la commande ou du devis. | Non         | `DEV-2023-001`           |

---

## Description des travaux

Zone de texte libre pour décrire en détail les travaux réalisés.

| Champ                                            | Description                                            | Obligatoire | Exemple                                                      |
|--------------------------------------------------|--------------------------------------------------------|-------------|--------------------------------------------------------------|
| **Description détaillée des travaux réalisés**   | Description complète des travaux.                      | Oui         | `Rénovation complète de la toiture avec remplacement des tuiles et isolation.` |

> Soyez précis dans la description pour faciliter le suivi et les futures références.
>
{style="tip"}

---

## Non-conformités constatées

Cette section permet de lister toutes les non-conformités identifiées lors de la réception.

### Structure d'une non-conformité

Chaque non-conformité contient les champs suivants :

| Champ                   | Description                                                | Obligatoire | Exemple                             |
|-------------------------|------------------------------------------------------------|-------------|-------------------------------------|
| **Localisation**        | Lieu de la non-conformité.                                 | Oui         | `Caves, Toit, Parking`              |
| **Type**                | Type de non-conformité (menu avec suggestions).            | Oui         | `Malfaçon`, `Non-conformité grave`  |
| **Gravité**             | Niveau de gravité (Mineure, Moyenne, Majeure, Critique).   | Oui         | `Majeure`                           |
| **Description détaillée**| Description précise de la non-conformité.                 | Oui         | `Tuiles mal fixées sur le versant nord` |
| **Solution proposée**   | Solution pour corriger la non-conformité.                  | Non         | `Refixer les tuiles avec crochets adaptés` |
| **Délai proposé**       | Date limite pour la correction.                            | Non         | `15/02/2026`                        |
| **Statut**              | Statut de résolution (À traiter, En cours, Résolue, etc.). | Oui         | `À traiter`                         |
| **Photos**              | Images illustrant la non-conformité (multiples).           | Non         | -                                   |

### Ajouter une non-conformité

1. Cliquer sur **Ajouter une non-conformité** en bas de la section.
2. Remplir les champs obligatoires (localisation, type, gravité, description, statut).
3. Ajouter des photos par drag & drop ou sélection (optionnel).
4. Répéter pour chaque non-conformité.

### Badge de comptage {id="badge-de-comptage_1"}

En haut de la section, un badge affiche le nombre de non-conformités : **X élément(s)**.

### Supprimer une non-conformité

Cliquer sur l'icône **poubelle** dans l'en-tête de la non-conformité.

---

## Constats (Autres observations)

Cette section permet d'ajouter des observations qui ne sont pas des non-conformités, mais qui méritent d'être documentées.

### Structure d'un constat

| Champ                  | Description                                   | Obligatoire | Exemple                          |
|------------------------|-----------------------------------------------|-------------|----------------------------------|
| **Localisation**       | Lieu de l'observation.                        | Oui         | `Parking, Cave, Combles`         |
| **Priorité**           | Niveau de priorité (1 à 5, ou Faible/Moyenne/Haute). | Oui         | `Haute`                          |
| **Description**        | Description de l'observation.                 | Oui         | `Fissure légère sur le mur nord` |
| **Solution envisagée** | Solution ou recommandation.                   | Non         | `Surveiller l'évolution`         |
| **Photos**             | Images illustrant l'observation (multiples).  | Non         | -                                |

### Ajouter un constat

1. Cliquer sur **Ajouter une observation** en bas de la section.
2. Remplir les champs obligatoires (localisation, priorité, description).
3. Ajouter des photos par drag & drop ou sélection (optionnel).
4. Répéter pour chaque observation.

### Badge de comptage

En haut de la section, un badge affiche le nombre de constats : **X élément(s)**.

### Supprimer un constat

Cliquer sur l'icône **poubelle** dans l'en-tête du constat.

---

## Commentaires généraux

Zone de texte libre pour ajouter des remarques générales sur la réception des travaux.

| Champ                                     | Description                                | Obligatoire | Exemple                                                   |
|-------------------------------------------|--------------------------------------------|-------------|-----------------------------------------------------------|
| **Commentaires et remarques générales**   | Commentaires libres.                       | Non         | `Dans l'ensemble, les travaux sont satisfaisants malgré quelques réserves.` |

---

## Enregistrement et finalisation

### Actions disponibles

| Bouton                       | Description                                                                                                   |
|------------------------------|---------------------------------------------------------------------------------------------------------------|
| **Enregistrer le brouillon** | Sauvegarde le rapport avec le statut `Brouillon`. Vous pourrez le modifier ultérieurement.                    |
| **Finaliser**                | Valide et finalise le rapport avec le statut `Finalisé`. Le rapport est alors considéré comme terminé.        |

> Les boutons sont désactivés si le formulaire contient des erreurs ou si une sauvegarde est en cours.
>
{style="warning"}

### Indicateur de progression

Pendant la sauvegarde, une barre de progression s'affiche avec :
- Un message indiquant l'étape en cours
- Un pourcentage de progression
- Un avertissement : "Ne fermez pas cette page"

---

## Mode édition

Lorsque vous **reprenez la saisie** d'un rapport existant, le formulaire est **automatiquement prérempli** avec toutes les données :

- Informations générales
- Copropriété et résidents
- Informations entrepreneur
- Description des travaux
- Non-conformités avec photos
- Constats avec photos
- Commentaires généraux

Vous pouvez modifier, ajouter ou supprimer des éléments, puis **Enregistrer** ou **Finaliser**.

---

## Exemples d'utilisation

<tabs>
<tab title="Créer un rapport de réception avec réserves">

1. Remplir les **informations générales** :
   - Titre : `Réception travaux toiture`
   - Date : `20/01/2026`
   - Type : `Réception provisoire`
   - Statut : `Acceptée avec réserves`
2. Sélectionner la **copropriété**.
3. Renseigner l'**entrepreneur** : `Entreprise Dupont`.
4. Décrire les **travaux** : `Rénovation de la toiture`.
5. Ajouter une **non-conformité** :
   - Localisation : `Toit`
   - Type : `Malfaçon`
   - Gravité : `Majeure`
   - Description : `Tuiles mal fixées`
   - Statut : `À traiter`
   - Ajouter une photo
6. Ajouter un **constat** :
   - Localisation : `Façade`
   - Priorité : `Moyenne`
   - Description : `Fissure légère`
7. Rédiger les **commentaires généraux**.
8. Cliquer sur **Finaliser**.

</tab>
<tab title="Enregistrer un brouillon">

1. Remplir partiellement le formulaire.
2. Cliquer sur **Enregistrer le brouillon**.
3. Retrouver le rapport dans la [vue d'ensemble](reports-overview.md) avec le statut `Brouillon`.
4. Reprendre la saisie plus tard.

</tab>
</tabs>