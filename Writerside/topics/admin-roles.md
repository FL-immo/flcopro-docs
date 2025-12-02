# Administration — Gestion des rôles
<primary-label ref="admin"/>

La page **Gestion des rôles** permet de définir et configurer les permissions associées à chaque rôle utilisateur (Admin et Gestionnaire). Vous pouvez activer ou désactiver des permissions spécifiques pour contrôler l'accès aux différentes fonctionnalités de l'application.

---

## Raccourci d'utilisation

1. Accéder à **Administration** → **Rôles** depuis le menu principal.
2. Utiliser la **barre de recherche** pour filtrer les permissions.
3. **Activer/Désactiver** les toggles pour chaque permission et chaque rôle.
4. Cliquer sur **Enregistrer** pour sauvegarder les modifications.
5. Utiliser **Réinitialiser** pour revenir aux paramètres par défaut.

---

## Structure de la page

La page est organisée sous forme d'un **tableau de permissions** avec trois colonnes :

| Colonne | Description |
|---------|-------------|
| **Permission** | Nom et description de la permission. |
| **Admin** | Toggle pour activer/désactiver cette permission pour le rôle Admin. |
| **Gestionnaire** | Toggle pour activer/désactiver cette permission pour le rôle Gestionnaire. |

---

## Barre de recherche

Un champ de recherche permet de filtrer rapidement les permissions affichées :

| Champ | Description | Exemple |
|-------|-------------|---------|
| **Recherche** | Recherche par nom de permission, description ou mot-clé. | `copropriété`, `rapport`, `utilisateur` |

> La recherche fonctionne sur le **label** (nom) et la **description** de chaque permission.
>
{style="tip"}

**Exemple** : Saisir `copropriété` affichera toutes les permissions liées à la gestion des copropriétés (création, édition, suppression, etc.).

---

## Tableau des permissions

Chaque ligne du tableau représente une **permission spécifique** avec :

| Élément                 | Description                                                                  |
|-------------------------|------------------------------------------------------------------------------|
| **Titre** (en gras)     | Nom de la permission (ex. *Créer une copropriété*, *Supprimer un rapport*).  |
| **Description**         | Explication détaillée de ce que permet cette permission.                     |
| **Toggle Admin**        | Interrupteur pour activer/désactiver la permission pour les administrateurs. |
| **Toggle Gestionnaire** | Interrupteur pour activer/désactiver la permission pour les gestionnaires.   |

## Gestion des permissions

### Activer une permission

1. Localiser la permission dans le tableau (utiliser la recherche si nécessaire).
2. Cliquer sur le **toggle** correspondant au rôle (Admin ou Gestionnaire).
3. Le toggle passe à l'état activé (bleu).
4. Cliquer sur **Enregistrer** pour sauvegarder.

### Désactiver une permission

1. Cliquer sur le **toggle actif** (bleu) de la permission.
2. Le toggle passe à l'état désactivé (gris).
3. Cliquer sur **Enregistrer** pour appliquer les modifications.

> **Astuce** : Survoler un toggle affiche la description complète de la permission dans une info-bulle.
>
{style="tip"}

---

## Boutons d'action

| Bouton | Description |
|--------|-------------|
| **Enregistrer** | Sauvegarde toutes les modifications apportées aux permissions. |
| **Réinitialiser** | Annule toutes les modifications non sauvegardées et revient aux paramètres par défaut. |

## Bonnes pratiques

| Pratique                          | Recommandation                                                                            |
|-----------------------------------|-------------------------------------------------------------------------------------------|
| **Principe du moindre privilège** | N'accordez que les permissions nécessaires à chaque rôle.                                 |
| **Révision régulière**            | Révisez périodiquement les permissions pour s'assurer qu'elles sont toujours pertinentes. |
| **Sauvegarde**                    | Enregistrez toujours après modification pour éviter de perdre vos changements.            |
