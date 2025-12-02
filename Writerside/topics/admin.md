# Administration
<primary-label ref="admin"/>

La section **Administration** regroupe tous les outils de gestion avancée de l'application, réservés aux utilisateurs disposant du rôle **Administrateur**. Elle permet de gérer les comptes utilisateurs et de configurer finement les permissions de chaque rôle.

---

## Gestion des utilisateurs

La page [Gestion des utilisateurs](admin-users.md) permet d'administrer tous les comptes utilisateurs de l'application.

**Fonctionnalités** :
- **Création de comptes** : Ajout de nouveaux utilisateurs avec génération automatique de l'email.
- **Modification** : Édition des informations, changement de rôle, activation/désactivation.
- **Suppression** : Suppression définitive d'un compte (avec confirmation).
- **Recherche** : Filtrage par email ou nom en temps réel.

**Informations gérées** :
- Prénom et nom
- Adresse email (identifiant de connexion)
- Rôle (Admin ou Gestionnaire)
- Statut du compte (Actif ou Inactif)
- Date de création
- Dernière activité

> Privilégiez la désactivation temporaire plutôt que la suppression pour conserver l'historique des actions.
>
{style="tip"}

[Gérer les utilisateurs](admin-users.md)

---

## Gestion des rôles

La page [Gestion des rôles](admin-roles.md) permet de configurer précisément les permissions accordées à chaque rôle utilisateur.

**Fonctionnalités** :
- **Configuration par rôle** : Définissez les droits pour Admin et Gestionnaire séparément.
- **Tableau de permissions** : Vue d'ensemble claire de tous les droits configurables.
- **Toggles individuels** : Activez ou désactivez chaque permission indépendamment.
- **Recherche** : Filtrez les permissions par nom ou description.
- **Réinitialisation** : Retour aux paramètres par défaut en un clic.

**Types de permissions** :
- Gestion des copropriétés (création, édition, suppression)
- Gestion des rapports (création, édition, suppression, téléchargement)
- Administration (gestion des utilisateurs, configuration des rôles)
- Accès aux fonctionnalités avancées

> Appliquez le principe du moindre privilège : n'accordez que les permissions strictement nécessaires à chaque rôle.
>
{style="warning"}

[Configurer les permissions](admin-roles.md)

---

## Rôles disponibles

L'application propose deux rôles avec des vocations différentes :

### Administrateur

**Vocation** : Gestion complète de l'application et de l'équipe.

**Permissions typiques** :
- Accès à toutes les fonctionnalités de l'application
- Gestion des utilisateurs (création, modification, suppression)
- Configuration des rôles et permissions
- Gestion complète des copropriétés et rapports
- Accès à l'administration

**Badge** : 🔴 Rouge

### Gestionnaire

**Vocation** : Gestion opérationnelle des copropriétés et création de rapports.

**Permissions typiques** (configurables) :
- Création et modification de copropriétés
- Création de rapports de visite
- Consultation des rapports de l'équipe
- Modification de son profil
- Pas d'accès à l'administration

**Badge** : ⚪ Standard

> Les permissions exactes de chaque rôle sont entièrement configurables depuis la [gestion des rôles](admin-roles.md).
>
{style="note"}

---

## Flux de travail typique

<tabs>
<tab title="Ajouter un nouveau gestionnaire">

1. Accéder à **Administration** → **Utilisateurs**.
2. Cliquer sur **Ajouter un utilisateur**.
3. Remplir :
   - **Prénom** : `Marie`
   - **Nom** : `Dupont`
   - **Email** : (auto-généré) `marie.dupont@prevot-immobilier.com`
   - **Rôle** : `Gestionnaire`
4. Cliquer sur **Ajouter**.
5. L'utilisateur reçoit un email pour créer son mot de passe.
6. Il peut se connecter et accéder aux fonctionnalités selon ses permissions.

</tab>
<tab title="Promouvoir un gestionnaire en admin">

1. Accéder à **Administration** → **Utilisateurs**.
2. Rechercher l'utilisateur (ex. `marie.dupont`).
3. Cliquer sur l'icône **Éditer** ![edit.svg](edit.svg).
4. Changer le **Rôle** de `Gestionnaire` à `Admin`.
5. Cliquer sur **Enregistrer**.
6. L'utilisateur dispose maintenant de tous les droits administrateur.

</tab>
<tab title="Désactiver temporairement un compte">

1. Accéder à **Administration** → **Utilisateurs**.
2. Trouver l'utilisateur concerné.
3. Cliquer sur **Éditer** ![edit.svg](edit.svg).
4. Désactiver le toggle **Actif**.
5. Cliquer sur **Enregistrer**.
6. L'utilisateur ne peut plus se connecter (badge "Inactif" gris).
7. Pour le réactiver : répéter l'opération en réactivant le toggle.

</tab>
<tab title="Configurer les permissions des gestionnaires">

1. Accéder à **Administration** → **Rôles**.
2. Localiser la permission "Supprimer une copropriété".
3. **Désactiver** le toggle pour la colonne **Gestionnaire**.
4. Les gestionnaires ne peuvent plus supprimer de copropriétés.
5. Cliquer sur **Enregistrer** pour valider.
6. Les modifications sont immédiatement appliquées.

</tab>
<tab title="Réinitialiser le mot de passe d'un utilisateur">

1. Accéder à **Administration** → **Utilisateurs**.
2. Trouver l'utilisateur qui a oublié son mot de passe.
3. Cliquer sur l'icône **@** (arobase) ![at-sign](at-sign.svg).
4. Un email de réinitialisation est automatiquement envoyé.
5. L'utilisateur reçoit un lien pour créer un nouveau mot de passe.

</tab>
</tabs>

---

## Bonnes pratiques

| Pratique | Recommandation |
|----------|----------------|
| **Principe du moindre privilège** | N'accordez que les permissions strictement nécessaires à chaque rôle. |
| **Révision régulière** | Révisez périodiquement les permissions et les comptes actifs. |
| **Désactivation vs Suppression** | Privilégiez la désactivation pour conserver l'historique des actions. |
| **Rôles Admin** | Limitez le nombre d'administrateurs pour des raisons de sécurité. |
| **Sauvegarde** | Enregistrez toujours après modification des permissions. |

---

## Accès à l'administration

Pour accéder à la section Administration :

1. Se connecter avec un compte **Administrateur**.
2. Cliquer sur **Administration** dans le menu principal.
3. Choisir **Utilisateurs** ou **Rôles** selon vos besoins.

> Seuls les utilisateurs avec le rôle **Administrateur** peuvent accéder à cette section.
>
{style="warning"}
