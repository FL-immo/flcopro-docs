# Profil utilisateur

La page **Profil** permet à chaque utilisateur de consulter et modifier ses informations personnelles, ainsi que de gérer les paramètres de sécurité de son compte.

---

## Raccourci d'utilisation

1. Accéder à **Profil** depuis le menu principal ou l'icône utilisateur.
2. Consulter vos **informations personnelles** (nom, email, rôle, statut).
3. Cliquer sur **Modifier le profil** pour éditer vos informations.
4. Utiliser la section **Paramètres de sécurité** pour changer votre mot de passe.
5. Cliquer sur **Sauvegarder** pour valider les modifications.

---

## Informations personnelles

Cette section affiche toutes les informations relatives à votre compte utilisateur.

### Consultation

Les informations suivantes sont affichées en mode lecture :

| Information                | Description                                                     | Exemple                                 |
|----------------------------|-----------------------------------------------------------------|-----------------------------------------|
| **Nom complet**            | Prénom et nom de l'utilisateur.                                 | `Pierre Schwartz`                       |
| **Rôle**                   | Rôle attribué (badge rouge pour Admin, bleu pour Gestionnaire). | `Admin`, `Gestionnaire`                 |
| **Statut**                 | État du compte (badge vert si actif, gris si inactif).          | `Actif`, `Inactif`                      |
| **Email**                  | Adresse email utilisée pour la connexion.                       | `pierre.schwartz@prevot-immobilier.com` |
| **Identifiant**            | ID technique unique du compte.                                  | `507f1f77bcf86cd799439011`              |
| **Créé le**                | Date de création du compte.                                     | `15 janvier 2024`                       |
| **Dernière activité**      | Date et heure de la dernière connexion.                         | `02/12/2025 14:30`                      |
| **Copropriétés épinglées** | Nombre de copropriétés favorites.                               | `4`                                     |

### Badges de statut

| Badge            | Couleur  | Signification                                   |
|------------------|----------|-------------------------------------------------|
| **Admin**        | 🔴 Rouge | Utilisateur avec tous les droits.               |
| **Gestionnaire** | 🔵 Bleu  | Utilisateur avec des droits limités.            |
| **Actif**        | 🟢 Vert  | Compte actif, peut se connecter.                |
| **Inactif**      | ⚫ Gris   | Compte désactivé (seul un admin peut modifier). |

> Les informations de votre profil ne sont visibles que par vous-même et les administrateurs du système.
>
{style="note"}

---

## Modifier le profil

### Activation du mode édition

1. Cliquer sur le bouton **Modifier le profil**.
2. Le formulaire passe en mode édition avec trois champs modifiables.

### Champs modifiables

En mode édition, vous pouvez modifier :

| Champ      | Description                                 | Exemple                                 |
|------------|---------------------------------------------|-----------------------------------------|
| **Email**  | Adresse email (utilisée pour la connexion). | `pierre.schwartz@prevot-immobilier.com` |
| **Prénom** | Votre prénom.                               | `Pierre`                                |
| **Nom**    | Votre nom de famille.                       | `Schwartz`                              |

> **Attention** : Si vous modifiez votre email, vous devrez utiliser la nouvelle adresse pour vos prochaines connexions.
>
{style="warning"}

### Sauvegarder les modifications

1. Modifier les champs souhaités.
2. Cliquer sur **Sauvegarder** pour valider.
3. Cliquer sur **Annuler** pour revenir en mode lecture sans enregistrer.

Un message de confirmation s'affiche si la sauvegarde est réussie.

---

## Paramètres de sécurité

La section **Paramètres de sécurité** permet de modifier votre mot de passe.

### Changer le mot de passe

Pour modifier votre mot de passe :

1. Remplir le formulaire de changement de mot de passe :
   - **Mot de passe actuel** : Saisir votre mot de passe actuel pour vérification.
   - **Nouveau mot de passe** : Choisir un nouveau mot de passe sécurisé.
   - **Confirmer le mot de passe** : Ressaisir le nouveau mot de passe pour confirmation.

2. Cliquer sur **Changer le mot de passe**.

### Règles de sécurité

Pour garantir la sécurité de votre compte, votre mot de passe doit :

- Contenir au minimum **8 caractères**
- Inclure au moins **une lettre majuscule**
- Inclure au moins **une lettre minuscule**
- Inclure au moins **un chiffre**
- Inclure au moins **un caractère spécial** (!, @, #, $, etc.)

### Validation

Si les deux mots de passe ne correspondent pas, un message d'erreur s'affiche :

> ⚠️ Les mots de passe ne correspondent pas.
>
{style="warning"}

Si le mot de passe actuel est incorrect, la modification sera refusée.

---

## Messages système

L'application affiche des messages pour vous informer du résultat de vos actions :

| Type de message       | Description                                | Exemple                                  |
|-----------------------|--------------------------------------------|------------------------------------------|
| **Message de succès** | Confirmation que l'action a été effectuée. | `✓ Profil mis à jour avec succès`        |
| **Message d'erreur**  | Indication qu'une erreur s'est produite.   | `✗ Le mot de passe actuel est incorrect` |

---

## Exemples d'utilisation

<tabs>
<tab title="Modifier ses informations">

**Scénario** : Vous souhaitez mettre à jour votre prénom.

1. Accéder à **Profil**.
2. Cliquer sur **Modifier le profil**.
3. Modifier le champ **Prénom** : `Jean-Pierre`.
4. Cliquer sur **Sauvegarder**.
5. Un message de confirmation s'affiche.
6. Les modifications sont immédiatement visibles.

</tab>
<tab title="Changer d'adresse email">

**Scénario** : Vous avez changé d'adresse email professionnelle.

1. Accéder à **Profil**.
2. Cliquer sur **Modifier le profil**.
3. Modifier le champ **Email** : `nouvelle.adresse@prevot-immobilier.com`.
4. Cliquer sur **Sauvegarder**.
5. À votre prochaine connexion, utiliser la nouvelle adresse email.

> Pensez à noter votre nouvelle adresse pour ne pas oublier lors de la prochaine connexion.
>
{style="tip"}

</tab>
<tab title="Changer son mot de passe">

**Scénario** : Vous souhaitez renforcer la sécurité de votre compte.

1. Accéder à **Profil**.
2. Dans la section **Paramètres de sécurité** :
   - **Mot de passe actuel** : `AncienMotDePasse123!`
   - **Nouveau mot de passe** : `NouveauMotDePasse456@`
   - **Confirmer le mot de passe** : `NouveauMotDePasse456@`
3. Cliquer sur **Changer le mot de passe**.
4. Un message de confirmation s'affiche.
5. À votre prochaine connexion, utiliser le nouveau mot de passe.

</tab>
<tab title="Vérifier ses copropriétés épinglées">

**Scénario** : Vous voulez savoir combien de copropriétés vous avez épinglées.

1. Accéder à **Profil**.
2. Consulter la ligne **Copropriétés épinglées** : `4`.
3. Pour gérer vos favoris, accéder à [Copropriétés → Liste](condominiums-list.md).
4. Épingler ou désépingler des copropriétés selon vos besoins (maximum 6).

</tab>
<tab title="Annuler une modification">

**Scénario** : Vous avez commencé à modifier vos informations mais changez d'avis.

1. Cliquer sur **Modifier le profil**.
2. Commencer à modifier des champs.
3. Cliquer sur **Annuler**.
4. Le formulaire revient en mode lecture avec les données originales.
5. Aucune modification n'a été enregistrée.

</tab>
</tabs>

---

## Bonnes pratiques

| Pratique         | Recommandation                                                                |
|------------------|-------------------------------------------------------------------------------|
| **Mot de passe** | Changez régulièrement votre mot de passe (tous les 3 à 6 mois).               |
| **Sécurité**     | Utilisez un mot de passe unique, différent de vos autres comptes.             |
| **Email**        | Vérifiez que votre email est toujours valide pour recevoir les notifications. |
| **Déconnexion**  | Déconnectez-vous toujours après utilisation sur un poste partagé.             |
| **Activité**     | Signalez à un administrateur toute activité suspecte sur votre compte.        |

## Informations techniques

### Données modifiables par l'utilisateur

- ✅ Email
- ✅ Prénom
- ✅ Nom
- ✅ Mot de passe

### Données modifiables uniquement par les administrateurs

- ❌ Rôle (Admin / Gestionnaire)
- ❌ Statut (Actif / Inactif)
- ❌ Date de création
- ❌ Identifiant technique

### Sécurité

- Les mots de passe sont **chiffrés** et ne sont jamais stockés en clair.
- Le changement de mot de passe nécessite la **vérification du mot de passe actuel**.
