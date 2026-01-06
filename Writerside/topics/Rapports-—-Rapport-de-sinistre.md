# Rapports — Rapport de sinistre

La page **Créer un nouveau rapport de sinistre** (ou **Reprendre le rapport de sinistre** en mode édition) permet de documenter une expertise d'assurance ou une recherche de fuite : informations générales, expertise, lieu du sinistre, personnes présentes, objet de l'expertise, constatations, actions à suivre et conclusion.

---

## Raccourci d'utilisation

1. Accéder à la page via **Rapports** → **Nouveau rapport** → **Rapport de sinistre** ou depuis la [vue d'ensemble des rapports](reports-overview.md).
2. Remplir les **informations générales** (titre, date, type de sinistre, rédacteur).
3. Sélectionner la **copropriété associée**.
4. Ajouter les **copropriétaires présents** (optionnel).
5. Renseigner les **informations de l'expertise** (date, horaires).
6. Renseigner l'**adresse exacte du lieu du sinistre**.
7. Ajouter les **personnes présentes à l'expertise**.
8. Compléter l'**objet de l'expertise** (assuré, lésé, assureur, expert, etc.).
9. Décrire le **sinistre constaté** avec photos.
10. Rédiger le **compte rendu de réunion**.
11. Ajouter les **actions à suivre**.
12. Rédiger la **conclusion** avec points clés.
13. **Enregistrer le brouillon** ou **Finaliser** le rapport.

---

## Informations générales

### Champs principaux

| Champ                | Description                                         | Obligatoire | Exemple                                              |
|----------------------|-----------------------------------------------------|-------------|------------------------------------------------------|
| **Titre**            | Titre du rapport.                                   | Oui         | `Compte rendu expertise assurance - Recherche de fuite` |
| **Date du rapport**  | Date de rédaction du rapport.                       | Oui         | `10/01/2026`                                         |
| **Type de sinistre** | Type de sinistre (menu avec suggestions).           | Oui         | `Dégât des eaux`, `Recherche de fuite`               |
| **Rédacteur**        | Utilisateur responsable de la rédaction du rapport. | Oui         | `Lionel Forni`                                       |

---

## Copropriété associée

### Sélection de la copropriété

| Champ                            | Description                                                            |
|----------------------------------|------------------------------------------------------------------------|
| **Sélectionner une copropriété** | Menu déroulant avec recherche par code ou nom.                         |
| **Identifiant**                  | Code unique de la copropriété (lecture seule, rempli automatiquement). |

### Adresse

Une fois la copropriété sélectionnée, l'adresse est **automatiquement préremplie**.

---

## Copropriétaires présents

Cette section permet d'enregistrer les résidents présents (optionnel). Fonctionne de la même manière que dans les autres rapports.

---

## Informations de l'expertise

Horaires et date de l'expertise sur site.

| Champ                | Description                   | Obligatoire | Exemple      |
|----------------------|-------------------------------|-------------|--------------|
| **Date de l'expertise** | Date de l'expertise.       | Oui         | `08/01/2026` |
| **Heure de début**   | Heure de début de l'expertise.| Oui         | `09:00`      |
| **Heure de fin**     | Heure de fin de l'expertise.  | Oui         | `11:30`      |

---

## Adresse exacte du lieu du sinistre

Cette section permet de préciser l'emplacement exact du sinistre, qui peut différer de l'adresse générale de la copropriété.

| Champ                         | Description                              | Obligatoire | Exemple                   |
|-------------------------------|------------------------------------------|-------------|---------------------------|
| **Nom Occupant**              | Nom de l'occupant du logement.           | Non         | `Mme DUPONT Marie`        |
| **Nom Copropriétaire**        | Nom du copropriétaire.                   | Non         | `M. MARTIN Jean`          |
| **N° appartement et entrée**  | Numéro d'appartement et entrée.          | Non         | `Appt 12, Entrée B`       |
| **Étage**                     | Étage du logement.                       | Non         | `3ème étage`              |
| **Adresse complète**          | Adresse complète du lieu du sinistre.    | Non         | `8 rue Paul Bert`         |

---

## Personnes présentes à l'expertise

Cette section permet d'ajouter toutes les personnes physiques présentes lors de l'expertise (experts, syndic, entrepreneurs, etc.).

### Formulaire d'ajout

| Champ          | Description                  | Obligatoire | Exemple                  |
|----------------|------------------------------|-------------|--------------------------|
| **Nom**        | Nom de la personne.          | Oui         | `DUPONT`                 |
| **Prénom**     | Prénom de la personne.       | Oui         | `Jean`                   |
| **Entreprise** | Nom de l'entreprise/cabinet. | Non         | `STIHLE`                 |
| **Email**      | Adresse email.               | Non         | `contact@entreprise.fr`  |
| **Téléphone**  | Numéro de téléphone.         | Non         | `01 23 45 67 89`         |

### Ajouter une personne

1. Remplir les champs **Nom** et **Prénom** (obligatoires).
2. Remplir les autres champs si disponibles.
3. Cliquer sur **Ajouter**.

### Liste des personnes

Une fois ajoutées, les personnes apparaissent dans une liste avec :
- **Nom Prénom** - Entreprise (si renseignée)
- Email et téléphone (si renseignés)
- Bouton **Supprimer**

### Compteur de personnes

En haut de la section, un badge affiche : **X personne(s)**.

---

## Objet de l'expertise - Recherche de fuite

Cette section regroupe toutes les informations administratives liées à l'expertise.

| Champ                        | Description                            | Obligatoire | Exemple                                          |
|------------------------------|----------------------------------------|-------------|--------------------------------------------------|
| **Assuré**                   | Entité assurée.                        | Oui         | `SDC Le Paul BERT`                               |
| **Lésé**                     | Personne lésée.                        | Non         | `Mme DUPONT locataire / M. MARTIN copropriétaire`|
| **Assureur**                 | Compagnie d'assurance.                 | Non         | `CITYA ASSURANCES - SADA ASSURANCES`             |
| **N° Contrat**               | Numéro de contrat d'assurance.         | Non         | `1H0408440`                                      |
| **Expert d'assurance**       | Cabinet ou expert mandaté.             | Non         | `Cabinet EXPERT`                                 |
| **Tiers responsable**        | Tiers identifié comme responsable.     | Non         | `N/A`                                            |
| **Prestataire de services**  | Entreprise intervenant sur site.       | Non         | `STIHLE`                                         |
| **Courtier Assurance**       | Courtier en assurance.                 | Non         | `CITYA ASSURANCES pour le syndic`                |
| **Autres**                   | Autres informations.                   | Non         | -                                                |

---

## Sinistre constaté

Description détaillée du sinistre avec photos à l'appui.

| Champ                          | Description                                | Obligatoire | Exemple                                          |
|--------------------------------|--------------------------------------------|-------------|--------------------------------------------------|
| **Description du sinistre**    | Description complète du sinistre constaté. | Oui         | `Infiltrations d'eau au plafond de la chambre`   |
| **Photos du sinistre**         | Images illustrant le sinistre (multiples). | Non         | -                                                |

### Ajouter des photos

Utiliser la zone de drag & drop pour ajouter plusieurs images du sinistre.

> Formats acceptés : `.jpg`, `.jpeg`, `.png`.
>
{style="tip"}

---

## Compte rendu de réunion

Zone de texte libre pour documenter les échanges et observations faites lors de l'expertise.

| Champ                                                                    | Description                              | Obligatoire | Exemple                                             |
|--------------------------------------------------------------------------|------------------------------------------|-------------|-----------------------------------------------------|
| **Dégâts constatés / Lieux visités / Première conclusion de l'expertise**| Compte rendu détaillé de l'expertise.    | Non         | `Visite de l'appartement sinistré, constat d'infiltrations...` |

---

## Actions à suivre

Liste structurée des actions identifiées lors de l'expertise.

### Structure d'une action

| Champ              | Description                          | Obligatoire | Exemple                              |
|--------------------|--------------------------------------|-------------|--------------------------------------|
| **Objet**          | Description de l'action.             | Oui         | `Faire un constat avec le syndic`    |
| **Date objectif**  | Date limite ou date de réalisation.  | Non         | `Fait le 06/08/25`                   |
| **Statut**         | Statut de l'action (menu déroulant). | Non         | `À faire`, `En cours`, `Terminée`    |

### Ajouter une action

1. Cliquer sur **Ajouter une action** en bas de la section.
2. Remplir le champ **Objet** (obligatoire).
3. Renseigner la date objectif et le statut (optionnel).
4. Répéter pour chaque action.

### Numérotation automatique

Chaque action est automatiquement numérotée : `1`, `2`, `3`, etc.

### Compteur d'actions

En haut de la section, un badge affiche : **X action(s)**.

### Supprimer une action

Cliquer sur l'icône **poubelle** à droite de l'action.

---

## Conclusion

La section conclusion comprend deux parties : commentaires généraux et points clés.

### Conclusion générale

Zone de texte libre pour rédiger la conclusion de l'expertise.

| Champ                   | Description                        | Obligatoire | Exemple                                              |
|-------------------------|------------------------------------|-------------|------------------------------------------------------|
| **Conclusion générale** | Synthèse et remarques finales.     | Non         | `L'expertise révèle une fuite au niveau de la toiture...` |

### Points clés / Actions recommandées

Liste d'éléments prioritaires identifiés dans la conclusion.

| Champ           | Description                                  | Obligatoire | Exemple                                |
|-----------------|----------------------------------------------|-------------|----------------------------------------|
| **Priorité**    | Niveau de priorité (numérique).              | Non         | `1`, `2`, `3`                          |
| **Libellé**     | Titre court de l'élément.                    | Non         | `Réparer la toiture`                   |
| **Description** | Description détaillée de l'élément.          | Non         | `Intervention urgente sur le versant nord` |

### Ajouter un élément de conclusion

1. Cliquer sur **Ajouter un élément de conclusion**.
2. Remplir les champs (Priorité, Libellé, Description).
3. Répéter pour chaque point clé.

### Supprimer un élément

Cliquer sur l'icône **poubelle** à droite de l'élément.

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
- Informations de l'expertise
- Lieu du sinistre
- Personnes présentes
- Objet de l'expertise
- Sinistre constaté avec photos
- Compte rendu
- Actions à suivre
- Conclusion

Vous pouvez modifier, ajouter ou supprimer des éléments, puis **Enregistrer** ou **Finaliser**.

---

## Exemples d'utilisation

<tabs>
<tab title="Créer un rapport d'expertise complet">

1. Remplir les **informations générales** :
   - Titre : `Expertise assurance - Recherche de fuite`
   - Date : `10/01/2026`
   - Type : `Dégât des eaux`
2. Sélectionner la **copropriété**.
3. Renseigner l'**expertise** : Date `08/01/2026`, 09:00 - 11:30.
4. Préciser le **lieu** : Appt 12, 3ème étage.
5. Ajouter les **personnes présentes** (expert, syndic, etc.).
6. Compléter l'**objet de l'expertise** (assuré, assureur, etc.).
7. Décrire le **sinistre** avec photos.
8. Rédiger le **compte rendu**.
9. Ajouter 3 **actions** à suivre.
10. Rédiger la **conclusion** avec 2 points clés.
11. Cliquer sur **Finaliser**.

</tab>
<tab title="Enregistrer un brouillon">

1. Remplir partiellement le formulaire après la visite.
2. Cliquer sur **Enregistrer le brouillon**.
3. Retrouver le rapport dans la [vue d'ensemble](reports-overview.md).
4. Reprendre la saisie pour compléter les éléments manquants.

</tab>
</tabs>