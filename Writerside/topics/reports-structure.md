# Rapports — Structure des rapports

La page **Structure des rapports** permet de définir et personnaliser la structure hiérarchique des différents types de rapports (visite, index, maintenance). Vous pouvez gérer les catégories principales, sous-catégories et champs de saisie (templates) pour chaque type de rapport.

---

## Raccourci d'utilisation

1. Accéder à **Rapports** → **Structure des rapports** depuis le menu principal.
2. Sélectionner le **type de rapport** à configurer (Visite, Index, Maintenance).
3. Ajouter ou modifier les **catégories principales** du rapport.
4. Pour chaque catégorie, ajouter des **sous-catégories**.
5. Pour chaque sous-catégorie, définir les **champs** (templates) de saisie.
6. **Sauvegarder la structure** pour enregistrer les modifications.

---

## Indicateur de source des données

Un **badge coloré** indique l'origine de la structure affichée :

| Badge | Description |
|-------|-------------|
| **🔵 Chargé depuis la base de données** | La structure a été sauvegardée et provient de la base de données. |
| **⚪ Données par défaut (non sauvegardées)** | La structure affichée est celle par défaut. Les modifications ne sont pas encore enregistrées. |

> Tant que vous n'avez pas cliqué sur **Sauvegarder**, les modifications restent en mémoire locale et peuvent être perdues.
>
{style="warning"}

---

## Sélection du type de rapport

Un **sélecteur à onglets** permet de basculer entre les différents types de rapports :

| Type | Description |
|------|-------------|
| **Rapports de visite** | Structure des comptes rendus de visite d'immeuble. |
| **Rapports d'index** | Structure des relevés d'index (eau, gaz, électricité). |
| **Rapports de maintenance** | Structure des rapports d'intervention et maintenance. |

**Interaction** : Cliquer sur un onglet charge automatiquement la structure correspondante.

---

## Catégories principales

Les catégories principales organisent les grandes sections d'un rapport (ex. *Premier contact*, *Configuration générale*, *Maintenance*).

### Affichage d'une catégorie

Chaque catégorie principale est présentée dans une **carte** contenant :

| Élément | Description |
|---------|-------------|
| **Libellé** | Nom affiché de la catégorie (ex. *Premier contact*). |
| **ID** | Identifiant technique unique (ex. `first_contact`). |
| **Badge bleu** | Affiche l'ID de la catégorie. |
| **Actions** | Boutons Éditer ![edit.svg](edit.svg) et Supprimer ![trash.svg](trash.svg). |

### Ajouter une catégorie principale

1. Cliquer sur **➕ Ajouter une catégorie** (en haut à droite).
2. Remplir le formulaire :
   - **ID** : Identifiant technique (ex. `first_contact`, `general_config`).
   - **Libellé** : Nom affiché (ex. *Premier contact*, *Configuration générale*).
3. Cliquer sur **✓ Enregistrer** ou **✗ Annuler**.

> **Bonnes pratiques pour l'ID** :
> - Utiliser uniquement des minuscules et underscores (`_`).
> - Éviter les espaces, accents et caractères spéciaux.
> - Exemple : `equipment_inspection`, `incident_report`.
>
{style="tip"}

### Modifier une catégorie principale

1. Cliquer sur l'**icône Éditer** ![edit.svg](edit.svg) de la catégorie.
2. Modifier le **libellé** ou l'**ID** directement dans les champs.
3. Cliquer sur l'**icône Sauvegarder** ✓.

### Supprimer une catégorie principale

1. Cliquer sur l'**icône Supprimer** ![trash.svg](trash.svg).
2. Confirmer la suppression dans la boîte de dialogue.

> ⚠️ La suppression d'une catégorie principale supprime également **toutes ses sous-catégories et champs associés**.
>
{style="warning"}

---

## Sous-catégories

Les sous-catégories permettent d'organiser les champs de saisie au sein d'une catégorie principale (ex. *Configuration*, *Détails de l'intervention*).

### Affichage d'une sous-catégorie

Chaque sous-catégorie est présentée dans une **carte imbriquée** contenant :

| Élément | Description |
|---------|-------------|
| **Libellé** | Nom affiché de la sous-catégorie. |
| **ID** | Identifiant technique (affiché dans un badge). |
| **Actions** | Boutons Éditer ![edit.svg](edit.svg) et Supprimer ![trash.svg](trash.svg). |
| **Liste des champs** | Champs de saisie (templates) associés à cette sous-catégorie. |

### Ajouter une sous-catégorie

1. Dans une catégorie principale, cliquer sur **➕ Ajouter une sous-catégorie**.
2. Remplir le formulaire :
   - **ID** : Identifiant technique (ex. `config`, `intervention_details`).
   - **Libellé** : Nom affiché (ex. *Configuration*, *Détails de l'intervention*).
3. Cliquer sur **✓ Enregistrer** ou **✗ Annuler**.

### Modifier une sous-catégorie

1. Cliquer sur l'**icône Éditer** ![edit.svg](edit.svg) de la sous-catégorie.
2. Modifier le **libellé** ou l'**ID**.
3. Cliquer sur l'**icône Sauvegarder** ✓.

### Supprimer une sous-catégorie

1. Cliquer sur l'**icône Supprimer** ![trash.svg](trash.svg).
2. Confirmer la suppression.

> La suppression d'une sous-catégorie supprime également **tous ses champs associés**.
>
{style="warning"}

---

## Champs (Templates)

Les champs (ou **templates**) sont les éléments de saisie concrets qui apparaîtront dans les formulaires de rapports.

### Affichage d'un champ

Chaque champ est représenté par :

| Élément | Description |
|---------|-------------|
| **Libellé** | Nom affiché du champ (ex. *Chaufferie collective*, *Type d'intervention*). |
| **ID** | Identifiant technique (badge). |
| **Valeur par défaut** | Valeur pré-remplie dans le formulaire (optionnel). |
| **Specs** | Liste de valeurs prédéfinies pour ce champ (ex. Eau, Gaz, Électricité). |
| **État non requis** | Badge indiquant si l'état de conformité n'est pas demandé pour ce champ. |

### Ajouter un champ

1. Dans une sous-catégorie, cliquer sur **➕ Ajouter un champ**.
2. Remplir le formulaire :
   - **ID** : Identifiant technique (ex. `chaufferie`, `type_intervention`).
   - **Libellé** : Nom affiché (ex. *Chaufferie collective*, *Type d'intervention*).
   - **Valeur par défaut** : Valeur optionnelle pré-remplie.
   - **État non requis** : Cocher si le champ n'a pas besoin d'un état de conformité.
3. Cliquer sur **✓ Enregistrer** ou **✗ Annuler**.

### Modifier un champ

1. Cliquer sur l'**icône Éditer** ![edit.svg](edit.svg) du champ.
2. Le formulaire d'édition s'affiche avec les champs :
   - **Libellé** et **ID**.
   - **Valeur par défaut**.
   - **État non requis** (toggle).
   - **Spécifications** (voir section suivante).
3. Cliquer sur l'**icône Sauvegarder** ✓.

### Supprimer un champ

1. Cliquer sur l'**icône Supprimer** ![trash.svg](trash.svg).
2. Confirmer la suppression.

---

## Gestion des spécifications (Specs)

Les **spécifications** sont des valeurs prédéfinies qu'un champ peut prendre (ex. pour un champ "Type de compteur" : *Eau*, *Gaz*, *Électricité*).

### Ajouter une spécification

En mode édition d'un champ :

1. Saisir la valeur dans le champ **Nouvelle spécification**.
2. Cliquer sur le bouton **➕** ou appuyer sur **Entrée**.
3. La spécification apparaît sous forme de **badge bleu**.

### Supprimer une spécification

1. Dans la liste des specs (badges bleus), cliquer sur l'**icône ✗** du badge.
2. La spécification est immédiatement supprimée.

**Exemple d'utilisation** :

Pour un champ "Type de compteur" :
- Ajouter les specs : `Eau`, `Gaz`, `Électricité`.
- Lors de la création d'un rapport, l'utilisateur pourra sélectionner parmi ces valeurs.

---

## Exemples d'utilisation

<tabs>
<tab title="Ajouter une nouvelle catégorie complète">

**Objectif** : Créer une catégorie "Équipements" avec une sous-catégorie "Ascenseurs" et un champ "Marque".

1. Cliquer sur **➕ Ajouter une catégorie**.
2. Remplir :
   - **ID** : `equipment`
   - **Libellé** : `Équipements`
3. Cliquer sur **✓ Enregistrer**.
4. Dans la catégorie "Équipements", cliquer sur **➕ Ajouter une sous-catégorie**.
5. Remplir :
   - **ID** : `elevators`
   - **Libellé** : `Ascenseurs`
6. Cliquer sur **✓ Enregistrer**.
7. Dans la sous-catégorie "Ascenseurs", cliquer sur **➕ Ajouter un champ**.
8. Remplir :
   - **ID** : `brand`
   - **Libellé** : `Marque`
   - **Valeur par défaut** : (laisser vide)
9. Cliquer sur **✓ Enregistrer**.
10. Cliquer sur **💾 Sauvegarder la structure**.

</tab>
<tab title="Ajouter des spécifications à un champ">

**Objectif** : Ajouter des valeurs prédéfinies pour un champ "Type de chauffage".

1. Trouver le champ "Type de chauffage" dans la structure.
2. Cliquer sur **Éditer** ![edit.svg](edit.svg).
3. Dans la section **Spécifications**, saisir `Collectif` et cliquer sur **➕**.
4. Saisir `Individuel` et cliquer sur **➕**.
5. Saisir `Mixte` et cliquer sur **➕**.
6. Les trois specs apparaissent en badges bleus.
7. Cliquer sur **✓ Sauvegarder** (icône de sauvegarde du champ).
8. Cliquer sur **💾 Sauvegarder la structure**.

</tab>
<tab title="Réorganiser la structure d'un rapport de visite">

**Scénario** : Vous souhaitez ajouter une nouvelle catégorie "Sécurité incendie" au rapport de visite.

1. Sélectionner **Rapports de visite** dans les onglets.
2. Cliquer sur **➕ Ajouter une catégorie**.
3. Remplir :
   - **ID** : `fire_safety`
   - **Libellé** : `Sécurité incendie`
4. Cliquer sur **✓ Enregistrer**.
5. Ajouter une sous-catégorie :
   - **ID** : `fire_equipment`
   - **Libellé** : `Équipements de sécurité`
6. Ajouter des champs :
   - `fire_extinguishers` → *Extincteurs*
   - `smoke_detectors` → *Détecteurs de fumée*
   - `emergency_exits` → *Issues de secours*
7. Cliquer sur **💾 Sauvegarder la structure**.

</tab>
<tab title="Modifier un ID ou libellé">

**Objectif** : Renommer "Premier contact" en "Visite initiale".

1. Trouver la catégorie **Premier contact**.
2. Cliquer sur **Éditer** ![edit.svg](edit.svg).
3. Modifier le **Libellé** : `Visite initiale`.
4. (Optionnel) Modifier l'**ID** : `initial_visit`.
5. Cliquer sur **✓ Sauvegarder**.
6. Cliquer sur **💾 Sauvegarder la structure**.

> Attention : modifier l'ID d'une catégorie peut affecter les rapports existants qui y font référence.
>
{style="warning"}

</tab>
</tabs>