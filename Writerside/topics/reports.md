# Gestion des rapports

La section **Gestion des rapports** permet de créer, consulter et gérer tous vos rapports de copropriété. L'application propose plusieurs types de rapports adaptés à vos besoins, avec une structure personnalisable et des fonctionnalités avancées.

---

## Vue d'ensemble des rapports

La [vue d'ensemble](reports-overview.md) centralise tous vos rapports avec des outils de filtrage et de gestion.

**Fonctionnalités** :
- **Filtrage avancé** : Par type, copropriété, période ou auteur.
- **Tableau complet** : Visualisez date, type, immeuble, statut et auteur de chaque rapport.
- **Actions rapides** : Reprendre la saisie, éditer, télécharger, régénérer ou supprimer.
- **Statuts clairs** : Identifiez rapidement les brouillons et rapports finalisés.

> Activez le toggle "Uniquement mes rapports" pour filtrer rapidement vos propres documents.
>
{style="tip"}

[Consulter la vue d'ensemble](reports-overview.md)

---

## Types de rapports disponibles

L'application propose plusieurs types de rapports professionnels :

| Type | Description | Icône |
|------|-------------|-------|
| **Rapport de visite** | Compte rendu détaillé après une visite d'immeuble. | 🏢 |
| **Rapport de fin de travaux** | Vérification et validation de la fin de chantier. | 🔨 |
| **Rapport de sinistre** | Déclaration après un dégât ou incident. | 🔥 |
| **Rapport d'index** | Relevé des index (eau, gaz, électricité). | 📋 |

Chaque type dispose de sa propre structure et de ses propres champs de saisie adaptés au contexte.

---

## Créer un rapport

### Sélection du type

La page [Créer un rapport](reports-create.md) vous permet de choisir le type de rapport à générer.

**Fonctionnalités** :
- **Cartes visuelles** : Chaque type est présenté avec une icône et une description.
- **Barre de recherche** : Filtrez les types disponibles par mot-clé.
- **Accès direct** : Un clic sur une carte ouvre le formulaire correspondant.

[Sélectionner un type de rapport](reports-create.md)

### Rapport de visite

Le [rapport de visite](reports-visit.md) est le type de rapport le plus complet, permettant de documenter une inspection d'immeuble.

**Contenu du rapport** :
- **Informations générales** : Titre, date, type de visite, rédacteur
- **Copropriété** : Sélection et adresse automatique
- **Résidents présents** : Liste des copropriétaires présents lors de la visite
- **Catégories d'observation** : Organisation hiérarchique des constats
  - **Éléments** : Détails observés avec état, spécifications et observations
  - **Images** : Photos illustrant les constats
  - **Informations complémentaires** : Notes additionnelles par catégorie
- **Conclusion** : Résumé et actions prioritaires

**Workflow** :
1. Remplir les informations générales
2. Sélectionner la copropriété
3. Ajouter les résidents présents
4. Ajouter des catégories (Façade, Toiture, Ascenseurs, etc.)
5. Pour chaque catégorie, ajouter des éléments avec observations et photos
6. Rédiger la conclusion avec actions prioritaires
7. Enregistrer en brouillon ou finaliser

[Guide complet du rapport de visite](reports-visit.md)

---

## Structure des rapports

La page [Structure des rapports](reports-structure.md) permet de personnaliser complètement l'organisation de vos rapports.

**Hiérarchie à trois niveaux** :

1. **Catégories principales** : Grandes sections du rapport (ex. *Façade*, *Équipements*)
2. **Sous-catégories** : Organisation interne (ex. *Configuration*, *Maintenance*)
3. **Champs (Templates)** : Éléments de saisie concrets (ex. *Type de chauffage*, *Marque*)

**Fonctionnalités** :
- **Par type de rapport** : Structure indépendante pour Visite, Index et Maintenance
- **Gestion complète** : Ajout, modification et suppression à tous les niveaux
- **Spécifications** : Valeurs prédéfinies pour guider la saisie (ex. Eau, Gaz, Électricité)
- **Indicateur de source** : Badge indiquant si la structure provient de la base ou des données par défaut

> Personnalisez la structure selon vos besoins pour standardiser la saisie et garantir la cohérence de vos rapports.
>
{style="tip"}

[Configurer la structure des rapports](reports-structure.md)

---

## États des rapports

L'application gère deux statuts principaux :

| Statut | Badge | Description |
|--------|-------|-------------|
| **Brouillon** | 🟠 Orange | Rapport en cours de rédaction, peut être modifié librement. |
| **Finalisé** | 🔵 Bleu | Rapport terminé et validé, prêt à être partagé. |

### Cycle de vie d'un rapport

```
Création → Brouillon → Finalisation → Finalisé
     ↓                      ↓
   Édition           Reprendre/Régénérer
```

---

## Actions sur les rapports

Depuis la [vue d'ensemble](reports-overview.md), plusieurs actions sont disponibles :

| Action | Icône | Description | Disponibilité |
|--------|-------|-------------|---------------|
| **Reprendre la saisie** | ![external-link.svg](external-link.svg) | Ouvre le formulaire avec tous les champs préremplis. | Tous les rapports |
| **Éditer** | ![edit.svg](edit.svg) | Ouvre l'éditeur WYSIWYG pour modifier le contenu. | Rapports finalisés |
| **Télécharger** | ![download.svg](download.svg) | Génère et télécharge le PDF. | Tous les rapports |
| **Régénérer** | ![retry.svg](retry.svg) | Remet le rapport dans l'état "après saisie". | Rapports finalisés |
| **Supprimer** | ![trash.svg](trash.svg) | Supprime définitivement le rapport. | Tous les rapports |

---

## Flux de travail typique

<tabs>
<tab title="Créer un rapport de visite complet">

1. Accéder à **Rapports** → **Créer un rapport**.
2. Cliquer sur **Rapport de visite**.
3. Remplir les informations générales.
4. Sélectionner la copropriété.
5. Ajouter les résidents présents.
6. Ajouter une catégorie "Façade" :
   - Élément "Balcons" → État "Médiocre"
   - Ajouter une photo
7. Ajouter une catégorie "Toiture" :
   - Élément "Tuiles" → État "Bon"
8. Rédiger la conclusion avec 2-3 actions prioritaires.
9. Cliquer sur **Finaliser**.

</tab>
<tab title="Enregistrer un brouillon et le reprendre plus tard">

1. Commencer la création d'un rapport.
2. Remplir partiellement le formulaire.
3. Cliquer sur **Enregistrer le brouillon**.
4. Retrouver le rapport dans la vue d'ensemble (badge orange "Brouillon").
5. Cliquer sur la ligne pour reprendre la saisie.
6. Compléter les informations manquantes.
7. **Finaliser** le rapport.

</tab>
<tab title="Personnaliser la structure avant création">

1. Accéder à **Rapports** → **Structure des rapports**.
2. Sélectionner **Rapports de visite**.
3. Ajouter une catégorie "Sécurité incendie" :
   - ID : `fire_safety`
   - Libellé : `Sécurité incendie`
4. Ajouter une sous-catégorie "Équipements" :
   - ID : `fire_equipment`
5. Ajouter des champs :
   - `fire_extinguishers` → *Extincteurs*
   - `smoke_detectors` → *Détecteurs de fumée*
6. Cliquer sur **Sauvegarder la structure**.
7. Créer un nouveau rapport de visite → la catégorie "Sécurité incendie" est maintenant disponible.

</tab>
<tab title="Télécharger et partager un rapport">

1. Depuis la vue d'ensemble, localiser le rapport.
2. Cliquer sur l'icône **Télécharger** ![download.svg](download.svg).
3. Le PDF est automatiquement généré et téléchargé.
4. Partager le fichier PDF avec les copropriétaires.

</tab>
</tabs>

---

## Bonnes pratiques

| Pratique         | Recommandation                                                                                                                                         |
|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Brouillons**   | Enregistrez régulièrement vos rapports en brouillon pour éviter toute perte de données.                                                                |
| **Photos**       | Ajoutez des photos pour chaque constat important (formats JPG ou PNG recommandés).                                                                     |
| **Structure**    | Configurez la structure avant de créer vos premiers rapports pour standardiser la saisie.                                                              |
| **États**        | Pour enregistrer votre rapport vous devez saisir **obligatoirement** **tout** les états.                                                               |
| **Conclusion**   | Classez vos actions par ordre de priorité, en commençant par 1 pour l’action la plus urgente jusqu'a $n$, afin de faciliter le suivi par les lecteurs. |
