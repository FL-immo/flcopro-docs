# Rapports — Relevé de compteurs

La page **Créer un nouveau relevé de compteurs** (ou **Reprendre le relevé de compteurs** en mode édition) permet d'enregistrer les relevés de compteurs (eau, gaz, électricité) pour une copropriété : informations générales, copropriété associée, relevés individuels avec photos.

---

## Raccourci d'utilisation

1. Accéder à la page via **Rapports** → **Nouveau rapport** → **Relevé de compteurs** ou depuis la [vue d'ensemble des rapports](reports-overview.md).
2. Remplir les **informations générales** (titre, date, type de compteur, rédacteur).
3. Sélectionner la **copropriété associée**.
4. Ajouter les **copropriétaires présents** (optionnel).
5. Ajouter des **relevés de compteurs** individuels avec numéro, propriétaire, relevés précédent/actuel, notes et photo.
6. **Enregistrer le brouillon** ou **Finaliser** le rapport.

---

## Informations générales

### Champs principaux

| Champ                | Description                                         | Obligatoire | Exemple                        |
|----------------------|-----------------------------------------------------|-------------|--------------------------------|
| **Titre**            | Titre du rapport.                                   | Oui         | `Relevé compteurs eau Q1 2026` |
| **Date du relevé**   | Date à laquelle le relevé a été effectué.           | Oui         | `15/01/2026`                   |
| **Type de compteur** | Type de compteur relevé (Eau, Gaz, Électricité).    | Oui         | `Eau`                          |
| **Rédacteur**        | Utilisateur responsable de la rédaction du rapport. | Oui         | `Lionel Forni`                 |

> Le type de compteur détermine l'unité de mesure utilisée (m³ pour l'eau, kWh pour l'électricité, etc.).
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

Cette section permet d'enregistrer les résidents présents lors du relevé (optionnel).

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

## Relevés de compteurs

Cette section permet d'enregistrer tous les relevés individuels pour la copropriété.

### Ajouter un relevé

Le formulaire d'ajout contient les champs suivants :

| Champ                  | Description                                           | Obligatoire | Exemple           |
|------------------------|-------------------------------------------------------|-------------|-------------------|
| **Numéro de compteur** | Identifiant unique du compteur.                       | Oui         | `123456789`       |
| **Propriétaire**       | Résident associé au compteur (sélection).             | Oui         | `Jean Dupont`     |
| **Relevé précédent**   | Valeur du relevé précédent.                           | Oui         | `1250`            |
| **Relevé actuel**      | Valeur du relevé actuel.                              | Oui         | `1320`            |
| **Notes / Observations**| Remarques éventuelles.                               | Non         | `Compteur accessible` |
| **Photo du compteur**  | Photo du compteur (une seule image par relevé).       | Non         | -                 |

> La **consommation** est calculée automatiquement : `Relevé actuel - Relevé précédent`.
>
{style="tip"}

### Procédure d'ajout

1. Remplir les champs du formulaire d'ajout.
2. Ajouter une photo du compteur (optionnel) par drag & drop ou sélection.
3. Cliquer sur **Ajouter ce relevé**.
4. Le relevé apparaît dans le tableau des relevés enregistrés.

### Tableau des relevés enregistrés

Une fois ajoutés, les relevés apparaissent dans un tableau récapitulatif :

| Colonne                | Description                                      |
|------------------------|--------------------------------------------------|
| **Numéro de compteur** | Identifiant du compteur.                         |
| **Propriétaire**       | Nom du résident.                                 |
| **Relevé précédent**   | Valeur précédente.                               |
| **Relevé actuel**      | Valeur actuelle.                                 |
| **Consommation**       | Différence calculée avec l'unité (ex: `70 m³`).  |
| **Photo**              | Miniature de la photo (ou "Aucune photo").       |
| **Actions**            | Supprimer le relevé.                             |

> Survolez la photo pour voir les notes associées au relevé.
>
{style="tip"}

### Supprimer un relevé

Cliquer sur l'icône **poubelle** dans la colonne **Actions** du relevé à supprimer.

---

## Badge d'unité

En haut de la section "Relevés de compteurs", un badge affiche l'**unité de mesure** correspondant au type de compteur sélectionné :

- **Eau** : `m³`
- **Gaz** : `m³`
- **Électricité** : `kWh`

---

## État vide

Si aucun relevé n'a été ajouté, un message s'affiche :

> Aucun relevé enregistré. Ajoutez votre premier relevé ci-dessus.

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

Lorsque vous **reprenez la saisie** d'un rapport existant (brouillon ou finalisé), le formulaire est **automatiquement prérempli** avec toutes les données du rapport :

- Informations générales
- Copropriété et adresse
- Copropriétaires présents
- Relevés de compteurs avec photos

Vous pouvez alors modifier n'importe quel champ, ajouter ou supprimer des relevés, et **Enregistrer** ou **Finaliser** à nouveau.

---

## Exemples d'utilisation

<tabs>
<tab title="Créer un relevé de compteurs d'eau">

1. Remplir les **informations générales** :
   - Titre : `Relevé compteurs eau T1 2026`
   - Date : `15/01/2026`
   - Type : `Eau`
   - Rédacteur : `Lionel Forni`
2. Sélectionner la **copropriété** concernée.
3. Ajouter un relevé :
   - N° compteur : `123456789`
   - Propriétaire : `Jean Dupont`
   - Relevé précédent : `1250`
   - Relevé actuel : `1320`
   - Photo : télécharger une photo du compteur
4. Répéter pour chaque compteur de la copropriété.
5. Cliquer sur **Finaliser**.

</tab>
<tab title="Enregistrer un brouillon pour finir plus tard">

1. Remplir partiellement le formulaire avec quelques relevés.
2. Cliquer sur **Enregistrer le brouillon**.
3. Retrouver le rapport dans la [vue d'ensemble](reports-overview.md) avec le statut `Brouillon`.
4. Cliquer sur la ligne pour reprendre la saisie et ajouter les relevés manquants.

</tab>
<tab title="Reprendre un rapport finalisé">

1. Depuis la [vue d'ensemble](reports-overview.md), cliquer sur la ligne du rapport finalisé.
2. Le formulaire s'ouvre avec tous les relevés déjà enregistrés.
3. Modifier ou ajouter des relevés si nécessaire.
4. **Enregistrer** à nouveau.

</tab>
</tabs>