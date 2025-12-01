# Ajouter une copropriété

## Objectif
Créer une nouvelle fiche copropriété en remplissant le formulaire « Ajouter une copropriété ». Cette page est destinée aux utilisateurs disposant des informations de base (nom, adresse, année ou date de création, photo éventuelle).

## Raccourci d'utilisation
1. Ouvrir **Ajouter une copropriété** (menu : Copropriétés → Ajouter une copropriété).
2. Saisir le nom.
3. Vérifier et, si besoin, modifier le `Code` proposé.
4. Renseigner la date de création (ou `01/01/AAAA` si seule l'année est connue).
5. Ajouter une photo (optionnel) — privilégier paysage.
6. Remplir au moins un bloc d'adresse ou ajouter plusieurs rues via **Ajouter une rue**.
7. Cliquer sur **Créer**.

---

## Champs et comportements détaillés

#### Nom
Saisir le nom officiel de la copropriété.

#### Code — génération et modification
{style="note"}
Le code proposé est une suggestion calculée à partir du dernier code enregistré ; il est destiné à accélérer la saisie mais il reste entièrement modifiable.

- Comportement courant : si le dernier code est de la forme `PREFIX-NNN` (ex. `CDM-010`), la méthode d'incrément propose généralement `PREFIX-(NNN+1)` → `CDM-011`.
- Cas à connaître :
  - Si le compteur contient des zéros à gauche, l'incrément préserve la longueur numérique (ex. `CDM-009` → `CDM-010`).
  - Si le code ne suit pas un pattern numérique simple, la proposition peut être différente ; vérifiez toujours.

> Exemples : 
> 
> `CDM-010` → valeur proposée : `CDM-011`.
> 
> `CDM-999` → valeur proposée : `CDM-1000`.
>
{style="tip"}

> Le code proposé n'est pas définitif tant que vous n'avez pas cliqué sur **Créer** — vérifiez la cohérence avec vos conventions internes.
>
{style="warning"}

#### Date de création
- Si la date complète est connue : renseignez `jj/mm/aaaa`.
- Si seule l'année est connue (ou si la date exacte est inconnue) : renseignez `01/01/AAAA` (ex. `01/01/2019`).

> Remarque : dans les cas où l'année est connue mais pas le jour/mois, utiliser `01/01/AAAA` permet de conserver l'information temporelle sans inventer une date précise.
> 
{style="note"}

#### Photo
- L'image n'est pas nécessaire, mais recommandée pour l'affichage dans les rapports.
- Format conseillé : paysage (ratio largeur > hauteur).
- Formats usuels : JPEG, PNG. Pré-compresser si possible pour améliorer les performances.


#### Adresse (plusieurs rues)
- Le formulaire propose un bloc d'adresse standard : Rue, Code postal, Ville, Pays.
- Si la copropriété possède plusieurs rues (entrées, accès secondaires), vous pouvez **ajouter autant de blocs d'adresse que souhaité** en cliquant sur **Ajouter une rue**.
- Chaque bloc est indépendant : remplissez au minimum la rue et la ville pour qu'il soit exploitable.

---

## Boutons & actions
- **Créer** : enregistre la copropriété si tous les champs obligatoires sont valides.
- **Annuler** : ferme le formulaire sans enregistrer.