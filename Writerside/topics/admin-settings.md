# Administration — Paramètres
<primary-label ref="admin"/>

La page **Paramètres de l'administration** permet de superviser l'état du serveur VPS Hostinger et de gérer les images orphelines stockées dans la base de données. Accessible uniquement aux administrateurs, elle offre des outils de maintenance et d'optimisation de l'application.

---

## Raccourci d'utilisation

1. Accéder à la page via **Administration** → **Paramètres** depuis le [menu principal](navigation.md).
2. Consulter les **informations VPS Hostinger** (état du serveur, ressources, trafic).
3. Actualiser les données avec le bouton **Actualiser**.
4. Consulter les **statistiques des images orphelines**.
5. Supprimer les images orphelines pour libérer de l'espace (si nécessaire).

> Cette page nécessite des droits d'administrateur pour être accessible. L'utilisateur connecté est affiché en haut à droite (ex: "AM Arnaud Michel").
>
{style="warning"}

---

## Informations VPS Hostinger

Cette section affiche l'état et les ressources de votre serveur virtuel hébergé chez Hostinger.

### Actualisation des données

| Action         | Description                                              |
|----------------|----------------------------------------------------------|
| **Actualiser** | Recharge les informations du VPS depuis l'API Hostinger. |

> L'actualisation peut prendre quelques secondes selon la réponse de l'API.
>
{style="note"}

### États possibles

<tabs>
<tab title="Chargement">

Un indicateur de chargement s'affiche :
- Icône de chargement animée
- Message : "Chargement des informations VPS..."

</tab>
<tab title="Erreur">

Si une erreur survient :
- Icône d'alerte
- Message d'erreur explicite
- Instructions pour configurer la clé API si nécessaire

**Exemple d'erreur** : *"Clé API Hostinger non configurée"*

**Solution** : Ajoutez votre clé API dans le fichier `.env` :
```
HOSTINGER_API_KEY=votre_clé
```

</tab>
<tab title="Informations affichées">

Les informations du VPS sont affichées dans plusieurs sections organisées.

</tab>
</tabs>

---

## En-tête VPS

### Informations principales

| Information           | Description                                      | Exemple                  |
|-----------------------|--------------------------------------------------|--------------------------|
| **Nom du VPS**        | Nom du serveur virtuel.                          | `srv8542527.hstgr.cloud` |
| **Statut**            | État actuel du serveur (badge coloré).           | `running` (vert)         |
| **Localisation**      | Centre de données hébergeant le serveur.         | `France - Paris`         |
| **Système**           | Système d'exploitation installé.                 | `Debian 13`              |
| **Uptime**            | Temps de fonctionnement sans interruption.       | `1.3 months`             |
| **Date de création**  | Date de création du VPS.                         | `15/10/2025`             |

### Codes couleur des statuts

| Statut      | Couleur | Signification                              |
|-------------|---------|--------------------------------------------|
| `running`   | Vert    | Le serveur fonctionne normalement.         |
| `active`    | Vert    | Le serveur est actif et opérationnel.      |
| `suspended` | Orange  | Le serveur est suspendu.                   |
| `stopped`   | Rouge   | Le serveur est arrêté.                     |

---

## Plan et ressources

Cette section détaille le plan d'hébergement et l'utilisation des ressources.

### Informations du plan

| Information | Description                              | Exemple         |
|-------------|------------------------------------------|-----------------|
| **Nom**     | Nom du plan d'hébergement.               | `KVM 2`         |

### Ressources disponibles et utilisées

#### CPU (Processeur)

| Information         | Description                                    | Exemple         |
|---------------------|------------------------------------------------|-----------------|
| **vCores**          | Nombre de cœurs virtuels alloués.              | `2 vCores`      |
| **Utilisation**     | Pourcentage d'utilisation actuel.              | `1.25%`         |

> Si aucune donnée n'est disponible, le message "Aucune donnée" s'affiche.
>
{style="note"}

#### RAM (Mémoire)

| Information         | Description                                    | Exemple         |
|---------------------|------------------------------------------------|-----------------|
| **Capacité**        | Mémoire RAM totale allouée.                    | `8 GB`          |
| **Utilisation**     | Mémoire actuellement utilisée.                 | `0.98 GB / 8 GB` |

#### Disque (Stockage)

| Information         | Description                                    | Exemple           |
|---------------------|------------------------------------------------|-------------------|
| **Capacité**        | Espace disque total alloué.                    | `100 GB`          |
| **Utilisation**     | Espace disque actuellement utilisé.            | `6.33 GB / 100 GB`|

#### Bande passante (Réseau)

| Information         | Description                                    | Exemple         |
|---------------------|------------------------------------------------|-----------------|
| **Capacité**        | Bande passante mensuelle allouée.              | `8 TB`          |
| **Utilisation**     | Trafic total du mois en cours.                 | `0.01 GB`       |

### Affichage des ressources

Chaque ressource est présentée sous forme de carte avec :
- Une **icône** représentative (CPU, RAM, Disque, Réseau)
- Un **badge** indiquant la capacité totale
- La **valeur d'utilisation** actuelle

---

## Trafic réseau

Cette section détaille le trafic réseau du VPS.

| Métrique        | Description                              | Icône       | Exemple   |
|-----------------|------------------------------------------|-------------|-----------|
| **Entrant**     | Trafic reçu par le serveur.              | Flèche bas  | `0 GB`    |
| **Sortant**     | Trafic envoyé par le serveur.            | Flèche haut | `0.01 GB` |
| **Total**       | Somme du trafic entrant et sortant.      | Activité    | `0.01 GB` |

> Le trafic réseau est réinitialisé chaque mois selon le cycle de facturation.
>
{style="note"}

---

## Configuration réseau

Cette section affiche les informations de configuration réseau du VPS.

| Information  | Description                                  | Exemple                  |
|--------------|----------------------------------------------|--------------------------|
| **HOSTNAME** | Nom de domaine du serveur.                   | `srv2074782.hstgr.cloud` |
| **IPv4**     | Adresse IPv4 publique.                       | `71.58.123.42`           |
| **IPv6**     | Adresse IPv6 publique (si disponible).       | `2a5b:3268:e5:b6a7::2`   |
| **NS1**      | Premier serveur de noms (nameserver).        | `94.254.132.12`          |
| **NS2**      | Second serveur de noms (nameserver).         | `1.1.1.1`                |

---

## Gestion des images orphelines

Cette section permet de détecter et supprimer les images qui ne sont plus référencées par aucun document dans la base de données.

### Qu'est-ce qu'une image orpheline ?

Une **image orpheline** est un fichier stocké dans GridFS (système de stockage MongoDB) qui n'est plus référencé par aucun rapport, copropriété ou autre document. Ces images peuvent être supprimées en toute sécurité pour libérer de l'espace.

**Causes possibles** :
- Suppression d'un rapport sans suppression des images associées
- Erreur lors de l'upload d'une image
- Modification d'un rapport avec remplacement d'images

### Actualisation des statistiques

| Action       | Description                                                    |
|--------------|----------------------------------------------------------------|
| **Actualiser**| Recharge les statistiques depuis la base de données.          |

---

## Statistiques des images

Les statistiques s'affichent sous forme de cartes :

| Statistique              | Description                                           | Exemple    |
|--------------------------|-------------------------------------------------------|------------|
| **Images dans GridFS**   | Nombre total d'images stockées dans la base.          | `227`      |
| **Images référencées**   | Nombre d'images utilisées par au moins un document.   | `227`      |
| **Images orphelines**    | Nombre d'images non référencées.                      | `0`        |
| **Espace récupérable**   | Taille totale des images orphelines.                  | `0 B`      |

### Code couleur

| Valeur                     | Couleur | Signification                            |
|----------------------------|---------|------------------------------------------|
| Images référencées         | Vert    | Situation normale.                       |
| Images orphelines > 0      | Orange  | Des images peuvent être nettoyées.       |
| Images orphelines = 0      | Vert    | Aucune image orpheline, base propre.     |
| Espace récupérable > 0     | Orange  | De l'espace peut être libéré.            |
| Espace récupérable = 0     | Vert    | Aucun espace à récupérer.                |

> Lorsque le nombre d'images orphelines est à 0, c'est la situation idéale. Votre base de données est propre et optimisée.
>
{style="tip"}

---

## Liste des images orphelines

Si des images orphelines sont détectées, une liste détaillée s'affiche avec pour chaque image :

| Information     | Description                              | Exemple                                    |
|-----------------|------------------------------------------|--------------------------------------------|
| **Nom du fichier**| Nom original du fichier.               | `facade-balcon-rouille.jpg`                |
| **ID**          | Identifiant unique dans GridFS.          | `507f1f77bcf86cd799439011`                 |
| **Taille**      | Taille du fichier.                       | `2.4 MB`                                   |

### Affichage

- Les images orphelines sont affichées dans une **zone scrollable** si la liste est longue.
- Chaque image est présentée avec une icône, ses informations et sa taille dans un badge.

---

## Suppression des images orphelines

### Procédure de suppression

1. Consulter la liste des images orphelines.
2. Cliquer sur **Supprimer les images orphelines (X)**.
3. Une **modale de confirmation** s'ouvre.
4. Vérifier les informations affichées :
   - Nombre d'images à supprimer
   - Espace qui sera libéré
5. Cliquer sur **Confirmer la suppression**.

### Modale de confirmation

La modale affiche :

| Élément                    | Description                                              |
|----------------------------|----------------------------------------------------------|
| **Titre**                  | "Confirmer la suppression"                               |
| **Nombre d'images**        | Nombre d'images orphelines à supprimer.                  |
| **Avertissement**          | "Cette action est irréversible"                          |
| **Espace à libérer**       | Taille totale des images qui seront supprimées.          |
| **Bouton Annuler**         | Ferme la modale sans supprimer.                          |
| **Bouton Confirmer**       | Lance la suppression des images.                         |

> **Attention** : La suppression est définitive et ne peut pas être annulée.
>
{style="warning"}

### Résultat du nettoyage

Après la suppression, un message s'affiche avec :
- Le **nombre d'images supprimées** avec succès
- Le **nombre d'erreurs** éventuelles
- Un message récapitulatif : *"X image(s) supprimée(s) avec succès"*

---

## État "Aucune image orpheline"

Si aucune image orpheline n'est détectée, un message de confirmation s'affiche :

- Icône de validation verte
- Message : "Aucune image orpheline détectée"
- Sous-texte : "Votre base de données est propre"

> C'est la situation idéale. Aucune action n'est nécessaire.
>
{style="tip"}

---

## États de chargement

### Chargement des statistiques

Lors du chargement des statistiques :
- Icône de chargement animée
- Message : "Chargement des statistiques..."

### Nettoyage en cours

Lors de la suppression des images :
- Les boutons sont désactivés
- Un indicateur de progression peut s'afficher

---

## Cas d'usage

<tabs>
<tab title="Surveiller l'état du serveur">

1. Accéder à **Administration** → **Paramètres**.
2. Consulter la section **Informations VPS Hostinger**.
3. Vérifier le statut (doit être `Active`).
4. Vérifier l'utilisation des ressources (CPU, RAM, Disque).
5. Si une ressource approche 100%, envisager une mise à niveau du plan.

</tab>
<tab title="Nettoyer les images orphelines">

1. Accéder à **Administration** → **Paramètres**.
2. Consulter la section **Gestion des images orphelines**.
3. Cliquer sur **Actualiser** pour obtenir les statistiques à jour.
4. Si des images orphelines sont détectées :
   - Consulter la liste des images
   - Cliquer sur **Supprimer les images orphelines (X)**
   - Confirmer la suppression dans la modale
5. Vérifier le message de confirmation.
6. Actualiser les statistiques pour vérifier que les images ont bien été supprimées.

</tab>
<tab title="Surveiller le trafic réseau">

1. Accéder à **Administration** → **Paramètres**.
2. Consulter la section **Trafic réseau**.
3. Vérifier le trafic total par rapport à la bande passante allouée.
4. Si le trafic approche la limite mensuelle, envisager :
   - Une optimisation des images
   - Une mise à niveau du plan

</tab>
<tab title="Serveur bien optimisé">

**Exemple d'un serveur en bonne santé** (comme sur la capture) :

1. **CPU** : `1.25%` → Excellent, très faible utilisation
2. **RAM** : `0.98 GB / 8 GB` → Excellent, seulement 12% utilisé
3. **Disque** : `6.33 GB / 100 GB` → Excellent, seulement 6% utilisé
4. **Trafic** : `0.01 GB / 8 TB` → Quasi nul, début de mois
5. **Images orphelines** : `0` → Base de données propre
6. **Uptime** : `1.3 months` → Excellente stabilité

> Ce serveur est dans un état optimal. Aucune action de maintenance n'est nécessaire.
>
{style="tip"}

</tab>
</tabs>

---

## Bonnes pratiques

### Maintenance du serveur

- **Vérifier régulièrement** l'état du VPS (hebdomadaire recommandé).
- **Surveiller l'uptime** pour détecter d'éventuels redémarrages inattendus.
- **Monitorer l'utilisation des ressources** pour anticiper les besoins en mise à niveau.
- **Vérifier le trafic réseau** avant la fin du mois pour éviter les dépassements.

### Gestion des images

- **Nettoyer les images orphelines** au moins une fois par mois.
- **Actualiser les statistiques** après chaque suppression de rapport important.
- **Vérifier l'espace récupérable** pour optimiser le stockage.
- **Surveiller la croissance** du nombre total d'images dans GridFS.

### Sécurité

- **Limiter l'accès** à cette page aux administrateurs uniquement.
- **Vérifier la clé API Hostinger** dans le fichier `.env`.
- **Ne pas partager** les informations de configuration réseau (IP, NS) publiquement.
- **Sauvegarder régulièrement** la base de données avant tout nettoyage massif.

---

## Configuration requise

### Clé API Hostinger

Pour afficher les informations VPS, vous devez configurer une clé API Hostinger :

1. Se connecter au **panneau Hostinger**.
2. Générer une **clé API** dans les paramètres.
3. Ajouter la clé dans le fichier `.env` de l'application :
   ```
   HOSTINGER_API_KEY=votre_clé_api_ici
   ```
4. Redémarrer l'application.
5. Actualiser la page **Paramètres**.

> Sans clé API configurée, un message d'erreur s'affichera avec les instructions de configuration.
>
{style="warning"}

---

## Dépannage

### Les informations VPS ne s'affichent pas

**Causes possibles** :
- Clé API non configurée
- Clé API invalide ou expirée
- Problème de connexion à l'API Hostinger

**Solutions** :
1. Vérifier la configuration de la clé API dans `.env`.
2. Tester la validité de la clé depuis le panneau Hostinger.
3. Vérifier la connexion internet du serveur.
4. Consulter les logs de l'application pour plus de détails.

### Les statistiques des images sont incorrectes

**Causes possibles** :
- Cache des statistiques non actualisé
- Problème de connexion à la base de données

**Solutions** :
1. Cliquer sur **Actualiser** pour recharger les statistiques.
2. Vérifier la connexion à MongoDB.
3. Redémarrer l'application si nécessaire.

### La suppression des images échoue

**Causes possibles** :
- Erreur de connexion à GridFS
- Permissions insuffisantes sur la base de données
- Images verrouillées par un autre processus

**Solutions** :
1. Vérifier les logs d'erreur affichés après la suppression.
2. Vérifier les permissions de l'utilisateur MongoDB.
3. Réessayer après quelques minutes.
4. Contacter un administrateur système si le problème persiste.
