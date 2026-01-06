# Extracteur PDF (OCR)

L'extracteur PDF utilise la technologie OCR (Reconnaissance Optique de Caractères) pour transformer vos documents PDF scannés en fichiers PDF avec texte récupérable.

## Accéder à l'extracteur PDF

1. Dans le menu latéral, cliquez sur **Divers**
2. Cliquez sur **Extracteur PDF**

## Vérification des dépendances

Avant toute utilisation, le système vérifie automatiquement que les dépendances nécessaires sont installées sur le serveur.

### Dépendances requises

- **Tesseract OCR** : Moteur de reconnaissance de texte
- **Poppler** : Librairie pour le traitement des PDF

### En cas de dépendances manquantes

Si des dépendances ne sont pas installées, un avertissement s'affiche :

> ⚠️ **Dépendances manquantes**
>
> Certaines dépendances système ne sont pas installées sur le serveur :
> - **Tesseract OCR** - Requis pour la reconnaissance de texte
> - **Poppler** - Requis pour le traitement des PDF
>
> Contactez l'administrateur système pour installer ces dépendances.

Dans ce cas, la conversion ne sera pas possible tant que les dépendances ne sont pas installées.

## Télécharger un fichier PDF

### Méthode 1 : Glisser-déposer

1. Glissez votre fichier PDF depuis votre explorateur de fichiers
2. Déposez-le dans la zone prévue à cet effet

### Méthode 2 : Sélection manuelle

1. Cliquez sur la zone de téléchargement
2. Sélectionnez votre fichier PDF dans la boîte de dialogue

### Limitations

- **Taille maximale** : 10 MB
- **Format accepté** : PDF uniquement
- **Un seul fichier** à la fois

## Configuration de la conversion

Une fois le fichier sélectionné, configurez les paramètres de conversion :

### Langue(s) du document

Sélectionnez la langue principale du document dans la liste déroulante :
- Français
- Anglais
- Allemand
- Espagnol
- Italien
- Néerlandais
- Portugais
- Et de nombreuses autres langues...

> **Conseil** : Sélectionnez la bonne langue pour améliorer significativement la qualité de la reconnaissance.

### Mode haute précision

Activez le toggle **Mode haute précision** pour :
- Une meilleure qualité de reconnaissance
- Une détection plus fine des caractères
- Moins d'erreurs de transcription

> ⚠️ **Attention** : Le mode haute précision est **plus lent** que le mode normal.

**Utilisez-le pour :**
- Les documents avec une police de petite taille
- Les documents de mauvaise qualité
- Les documents importants nécessitant une grande précision

## Lancer la conversion

1. Vérifiez que votre fichier est bien chargé
2. Sélectionnez la langue appropriée
3. Activez le mode haute précision si nécessaire
4. Cliquez sur **Convertir**

### Barre de progression

Pendant la conversion, une barre de progression animée s'affiche avec :
- Le pourcentage d'avancement
- Un message de statut
- Une animation indiquant que le traitement est en cours

> **Important** : Ne fermez pas la page pendant la conversion.

### Messages de progression

Les messages suivants peuvent s'afficher :
- "Préparation du document..."
- "Conversion en cours..."
- "Traitement des pages..."
- "Finalisation..."

## Résultat de la conversion

### Succès

Si la conversion réussit :
- La barre de progression devient verte
- Un message de succès s'affiche : **"Conversion terminée avec succès !"**
- Le fichier PDF converti est automatiquement téléchargé

### Échec

En cas d'erreur, un message d'erreur rouge s'affiche avec :
- La description du problème
- Des recommandations pour résoudre l'erreur

## À propos de l'OCR

### Informations importantes

- **Taille maximale** : 10 MB
- **Formats acceptés** : PDF uniquement
- **Sortie** : PDF converti avec le texte récupérable
- **Conseil** : Pour de meilleurs résultats, utilisez des PDF de bonne qualité

### Qualité de la reconnaissance

La qualité de la reconnaissance dépend de plusieurs facteurs :
- **Qualité du scan** : Plus le scan est net, meilleure sera la reconnaissance
- **Taille de la police** : Les polices trop petites sont plus difficiles à reconnaître
- **Contraste** : Un bon contraste entre le texte et le fond améliore les résultats
- **Orientation** : Le document doit être droit
- **Langue sélectionnée** : Doit correspondre à la langue du document

## Bonnes pratiques

### Préparation du document

- Scannez vos documents en **300 DPI minimum** pour une meilleure qualité
- Assurez-vous que le document est **bien aligné**
- Utilisez un **bon contraste** (texte noir sur fond blanc idéalement)
- Évitez les documents **trop dégradés** ou **annotés**

### Pendant la conversion

- Ne fermez pas la fenêtre du navigateur
- N'actualisez pas la page
- Patientez jusqu'à la fin du traitement
- En cas d'échec, vérifiez la qualité de votre PDF source

### Après la conversion

- Vérifiez le PDF généré pour vous assurer de la qualité
- Testez la recherche de texte dans le PDF converti
- Si la qualité n'est pas satisfaisante, réessayez avec le mode haute précision
- Si nécessaire, améliorez la qualité du scan source et recommencez

## Cas d'usage

### Documents adaptés à l'OCR

- Contrats scannés
- Factures numérisées
- Courriers administratifs
- Procès-verbaux scannés
- Archives papier numérisées
- Documents anciens à archiver

### Documents moins adaptés

- Documents avec beaucoup de graphiques ou schémas
- Documents manuscrits (écriture à la main)
- Documents en très mauvais état
- Photos de documents (privilégiez un vrai scan)
- Documents avec police artistique ou inhabituelle

## Dépannage

### La conversion échoue

**Causes possibles :**
- Fichier PDF corrompu
- Document trop complexe
- Taille de fichier excessive
- Mauvaise qualité du scan

**Solutions :**
- Vérifiez que votre PDF s'ouvre correctement
- Réduisez la taille du fichier si possible
- Rescannez le document avec une meilleure qualité
- Essayez avec un autre fichier PDF pour tester

### La reconnaissance est de mauvaise qualité

**Solutions :**
- Activez le **mode haute précision**
- Vérifiez que la **langue sélectionnée** est correcte
- Améliorez la qualité du scan source
- Assurez-vous que le document est **bien aligné**
- Augmentez le contraste du document source

### Le téléchargement ne démarre pas

**Solutions :**
- Vérifiez les paramètres de téléchargement de votre navigateur
- Autorisez les téléchargements depuis l'application
- Essayez avec un autre navigateur
- Désactivez les bloqueurs de pop-up

## Contact support

Si vous rencontrez des problèmes persistants avec l'extracteur PDF, contactez l'administrateur système en précisant :
- Le type d'erreur rencontré
- La taille du fichier PDF
- La langue du document
- Les paramètres utilisés (mode haute précision activé ou non)
