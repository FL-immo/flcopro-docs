# Administration — Gestion des utilisateurs
<primary-label ref="admin"/>

La page **Gestion des utilisateurs** permet d'administrer les comptes utilisateurs de l'application. Vous pouvez créer, modifier, désactiver ou supprimer des utilisateurs et gérer leurs rôles.

---

## Raccourci d'utilisation

1. Accéder à **Administration** → **Utilisateurs** depuis le menu principal.
2. Utiliser la **barre de recherche** pour filtrer les utilisateurs par email ou nom.
3. Cliquer sur **Ajouter un utilisateur** pour créer un nouveau compte.
4. Utiliser les **actions rapides** (Modifier, Supprimer) pour gérer un utilisateur.
5. **Modifier** un utilisateur pour changer son rôle, ses informations ou le désactiver temporairement.

---

## Barre de recherche

Un champ de recherche permet de filtrer rapidement les utilisateurs :

| Champ | Description | Exemple |
|-------|-------------|---------|
| **Email or name** | Recherche par email ou nom/prénom (insensible à la casse). | `pierre`, `admin@`, `schwartz` |

> La recherche se met à jour en temps réel et filtre simultanément sur l'email, le prénom et le nom.
>
{style="tip"}

---

## Tableau des utilisateurs

Le tableau affiche tous les utilisateurs enregistrés avec les informations suivantes :

| Colonne               | Description                                            | Exemple                                                    |
|-----------------------|--------------------------------------------------------|------------------------------------------------------------|
| **Prénom**            | Prénom de l'utilisateur.                               | `Pierre`                                                   |
| **Nom**               | Nom de famille de l'utilisateur.                       | `Schwartz`                                                 |
| **Email**             | Adresse email (utilisée pour la connexion).            | `pierre.schwartz@prevot-immobilier.com`                    |
| **Role**              | Rôle assigné (badge rouge pour Admin).                 | `Admin`, `Gestionnaire`                                    |
| **Actif**             | État du compte (badge bleu si actif, gris si inactif). | `Actif`, `Inactif`                                         |
| **Créé le**           | Date de création du compte.                            | `15/01/2024`                                               |
| **Dernière activité** | Date et heure de la dernière connexion.                | `02/12/2025 14:30`                                         |
| **Actions**           | Icônes d'actions rapides.                              | ![at-sign](at-sign.svg) ![edit.svg](edit.svg) ![trash.svg](trash.svg) |

### Badges de statut

| Badge            | Couleur    | Signification                           |
|------------------|------------|-----------------------------------------|
| **Admin**        | 🔴 Rouge   | Utilisateur avec tous les droits.       |
| **Gestionnaire** | ⚪ Standard | Utilisateur avec des droits limités.    |
| **Actif**        | 🔵 Bleu    | Compte actif, peut se connecter.        |
| **Inactif**      | ⚫ Gris     | Compte désactivé, connexion impossible. |

---

## Actions disponibles

### Recréer le mot de passe d'un utilisateur

**Icône** : ![at-sign](at-sign.svg) (arobase)

1. Cliquer sur l'**icône arobase** de l'utilisateur concerné.
2. Un mot de passe temporaire est généré automatiquement.

> Cette action permet à un utilisateur qui a oublié son mot de passe de le réinitialiser sans intervention manuelle de l'administrateur.
>
{style="note"}

---

### Modifier un utilisateur

**Icône** : ![edit.svg](edit.svg) (crayon)

1. Cliquer sur l'**icône crayon** de l'utilisateur à modifier.
2. Un panneau latéral s'ouvre avec les champs modifiables :
   - **Prénom**
   - **Nom**
   - **Email**
   - **Rôle** (Admin ou Gestionnaire)
   - **Actif** (toggle pour activer/désactiver le compte)
3. Modifier les informations souhaitées.
4. Cliquer sur **Enregistrer** pour valider les modifications.

> **Désactiver un utilisateur** : Plutôt que de supprimer un compte, il est recommandé de le désactiver en décochant le toggle **Actif**. L'utilisateur ne pourra plus se connecter mais ses données seront conservées.
>
{style="tip"}

**Champs modifiables** :

| Champ | Type | Description |
|-------|------|-------------|
| **Prénom** | Texte | Prénom de l'utilisateur. |
| **Nom** | Texte | Nom de famille. |
| **Email** | Email | Adresse email (login). |
| **Rôle** | Sélection | `Admin` ou `Gestionnaire`. |
| **Actif** | Toggle | Active ou désactive le compte. |

---

### Supprimer un utilisateur

**Icône** : ![trash.svg](trash.svg) (corbeille)

1. Cliquer sur l'**icône corbeille** de l'utilisateur à supprimer.
2. Un panneau de confirmation s'ouvre avec l'email de l'utilisateur.
3. Lire attentivement l'avertissement : la suppression est **irréversible**.
4. Cliquer sur **Supprimer l'utilisateur** pour confirmer ou **Annuler** pour revenir en arrière.

> **Attention** : La suppression d'un utilisateur est définitive. Si vous souhaitez simplement empêcher l'accès temporairement, utilisez plutôt l'option **Actif/Inactif** dans la modification.
>
{style="warning"}

---

## Ajouter un utilisateur

Le bouton **Ajouter un utilisateur** (en haut à droite) ouvre un panneau latéral de création.

### Étapes de création

1. Cliquer sur **Ajouter un utilisateur**.
2. Remplir le formulaire :
   - **Prénom** *(obligatoire)* : Prénom de l'utilisateur.
   - **Nom** *(obligatoire)* : Nom de famille.
   - **Email** *(obligatoire)* : Adresse email professionnelle.
   - **Rôle** *(obligatoire)* : Choisir entre `Admin` ou `Gestionnaire`.
3. Cliquer sur **Ajouter** pour créer le compte.

### Génération automatique de l'email

Lors de la saisie du **prénom** et du **nom**, l'email est automatiquement suggéré au format :

```
prenom.nom@prevot-immobilier.com
```

> Vous pouvez modifier l'email généré automatiquement avant de valider la création.
>
{style="note"}

**Exemple** :
- Prénom : `Pierre`
- Nom : `Schwartz`
- Email généré : `pierre.schwartz@prevot-immobilier.com`

### Champs obligatoires

Tous les champs marqués d'un astérisque sont obligatoires. Si un champ est manquant, un message d'erreur s'affichera.

| Champ | Obligatoire | Exemple |
|-------|-------------|---------|
| **Prénom** | ✅ | `Pierre` |
| **Nom** | ✅ | `Schwartz` |
| **Email** | ✅ | `pierre.schwartz@prevot-immobilier.com` |
| **Rôle** | ✅ | `Gestionnaire` |

---

## Exemples d'utilisation

<tabs>
<tab title="Créer un nouvel utilisateur">

**Scénario** : Ajouter un nouveau gestionnaire de copropriétés.

1. Cliquer sur **Ajouter un utilisateur**.
2. Remplir :
   - **Prénom** : `Marie`
   - **Nom** : `Dupont`
   - **Email** : `marie.dupont@prevot-immobilier.com` (généré automatiquement)
   - **Rôle** : `Gestionnaire`
3. Cliquer sur **Ajouter**.
4. L'utilisateur apparaît dans le tableau avec le statut **Actif**.

</tab>
<tab title="Désactiver un utilisateur temporairement">

**Scénario** : Un gestionnaire part en congé longue durée.

1. Rechercher l'utilisateur dans la barre de recherche.
2. Cliquer sur l'**icône crayon** ![edit.svg](edit.svg).
3. Désactiver le toggle **Actif**.
4. Cliquer sur **Enregistrer**.
5. Le badge passe à **Inactif** (gris), l'utilisateur ne peut plus se connecter.

**Pour le réactiver** : Répéter l'opération en réactivant le toggle.

</tab>
<tab title="Changer le rôle d'un utilisateur">

**Scénario** : Promouvoir un gestionnaire au rôle Admin.

1. Cliquer sur l'**icône crayon** ![edit.svg](edit.svg) de l'utilisateur.
2. Dans le champ **Rôle**, sélectionner `Admin`.
3. Cliquer sur **Enregistrer**.
4. Le badge du rôle passe de standard à **Admin** (rouge).

</tab>
<tab title="Recréer le mot de passe d'un utilisateur">

**Scénario** : Un utilisateur a oublié son mot de passe.

1. Rechercher l'utilisateur dans le tableau.
2. Cliquer sur l'**icône arobase** ![at-sign](at-sign.svg).
3. Le nouveau mot de passe de l'utilisateur est généré automatiquement.

</tab>
<tab title="Supprimer un utilisateur définitivement">

**Scénario** : Un employé a quitté l'entreprise définitivement.

1. Cliquer sur l'**icône corbeille** ![trash.svg](trash.svg).
2. Vérifier l'email de l'utilisateur dans la confirmation.
3. Lire l'avertissement sur le caractère **irréversible** de l'action.
4. Cliquer sur **Supprimer l'utilisateur**.
5. L'utilisateur est définitivement supprimé de la base de données.

> Alternative recommandée : Désactiver le compte au lieu de le supprimer pour conserver l'historique des actions.
>
{style="tip"}

</tab>
</tabs>