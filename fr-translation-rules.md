# Guide de Traduction Française de DatoCMS

Ce guide définit les règles pour garantir la cohérence des traductions françaises de l'interface DatoCMS.

## Règles Fondamentales

- **Tutoiement** dans toute l'interface (jamais « vous »)
- **Termes techniques en anglais** : build, build trigger, deploy, webhook, adapter, schema, hook, payload, token, plugin, API, SEO, URL
- **Accord du participe passé** avec le nom qu'il qualifie : « Élément créé », « Filtre mis à jour »
- **Espace insécable avant** `!`, `?`, `:`, `;` (typographie française)
- **« Asset »** se traduit par **« média »** (masculin) → « le média », « les médias », « ce média »
- **« Save »** se traduit **toujours** par **« Enregistrer »** (jamais « Sauvegarder »)
- **Masculin par défaut** : quand le contexte ne permet pas de déterminer le genre du nom qualifié, utiliser le masculin (ex. « Créé avec succès » et non « Créé(e) avec succès »)
- **Capitalisation française** : seul le premier mot d'un titre prend la majuscule (ex. « Paramètres du projet », jamais « Paramètres Du Projet »)

## Règles de Désambiguïsation

### Dépublier / Dépublication

Contrairement à l'anglais « unpublish », le français utilise **« dépublier »** (verbe) et **« dépublication »** (nom) :

| Anglais                  | Français                |
| ------------------------ | ----------------------- |
| Unpublish                | Dépublier               |
| Unpublishing             | Dépublication           |
| Couldn't unpublish       | Impossible de dépublier |
| Successfully unpublished | Dépublié avec succès    |

### Accord du Participe Passé (IMPORTANT)

Le participe passé doit **toujours** s'accorder en genre et en nombre avec le sujet ou le nom qualifié :

| ✅ Correct                        | ❌ Incorrect                   |
| -------------------------------- | ----------------------------- |
| Élément **créé** avec succès     | Élément créée avec succès     |
| Élément **mis** à jour           | Élément mise à jour           |
| Élément **dépublié** avec succès | Élément dépublier avec succès |
| Élément **publié** avec succès   | Élément publiée avec succès   |
| Le média a été **supprimé**      | Le média a été supprimée      |
| Les éléments ont été **créés**   | Les éléments ont été créées   |

**Rappel** : « Élément » est masculin, « média » est masculin, « filtre » est masculin.

Quand le contexte ne permet pas de déterminer le genre (ex. message générique réutilisé pour plusieurs types d'objets), utiliser le **masculin par défaut** : « Créé avec succès », « Mis à jour avec succès ».

### Titres des Dialogues de Confirmation

Pour les titres des dialogues qui demandent confirmation, utiliser l'**infinitif** avec point d'interrogation :

| Type               | Exemple                   |
| ------------------ | ------------------------- |
| Dialogue confirmer | Supprimer cet élément ?   |
| Dialogue confirmer | Dépublier ce contenu ?    |
| Dialogue confirmer | Restaurer cette version ? |

Pour les **boutons d'action**, utiliser l'**infinitif** (style français courant) :

| Type   | Exemple     |
| ------ | ----------- |
| Bouton | Supprimer   |
| Bouton | Dépublier   |
| Bouton | Enregistrer |

### Heading vs Titre

- **« Heading »** (H1-H6 dans l'éditeur) → **« Titre »** (Titre 1, Titre 2, etc.)
- **« Title »** (champ titre, titre de page) → **« Titre »**

En français, les deux se traduisent par « Titre », mais le contexte les distingue :

| Anglais     | Français           |
| ----------- | ------------------ |
| Heading 1   | Titre 1 / Titre H1 |
| Heading 2   | Titre 2 / Titre H2 |
| Title field | Champ titre        |
| Page title  | Titre de la page   |

### Capitalisation des Titres

En français, contrairement à l'anglais, on ne met **pas** de majuscule à chaque mot d'un titre. Seul le premier mot prend la majuscule (ainsi que les noms propres) :

| ✅ Correct               | ❌ Incorrect (anglicisme) |
| ----------------------- | ------------------------ |
| Paramètres du projet    | Paramètres Du Projet     |
| Gestion des médias      | Gestion Des Médias       |
| Créer un nouvel élément | Créer Un Nouvel Élément  |
| Tableau de bord         | Tableau De Bord          |

Cette règle s'applique aux titres de pages, de sections, de menus, de dialogues et de boutons.

### Ponctuation dans les Messages

| Type de message        | Ponctuation             | Exemple                               |
| ---------------------- | ----------------------- | ------------------------------------- |
| **Erreur/Échec**       | Point d'exclamation `!` | Impossible de sauvegarder l'élément ! |
| **Succès avec action** | Point d'exclamation `!` | Élément créé avec succès !            |
| **Succès neutre**      | Aucune ou point         | Élément créé avec succès              |
| **Description/Info**   | Point `.`               | Ce champ est obligatoire.             |
| **Label UI**           | Aucune                  | Enregistrer l'élément                 |

**Règle importante** : En typographie française, il y a **toujours une espace** avant les signes de ponctuation doubles (`!`, `?`, `:`, `;`).

| ✅ Correct                       | ❌ Incorrect                    |
| ------------------------------- | ------------------------------ |
| Filtre créé avec succès !       | Filtre créé avec succès!       |
| Impossible de créer le filtre ! | Impossible de créer le filtre! |

### Pattern pour Messages d'Erreur

Utiliser **toujours** le pattern « Impossible de + infinitif » :

| ✅ Correct                 | ❌ Incorrect                  |
| ------------------------- | ---------------------------- |
| Impossible de sauvegarder | Erreur lors de la sauvegarde |
| Impossible de supprimer   | N'a pas pu supprimer         |
| Impossible de charger     | Échec du chargement          |

### Média (IMPORTANT)

Le terme anglais **« asset »** se traduit **toujours** par **« média »**. **Ne jamais** laisser « asset » en anglais, ni traduire par « actif » ou « élément multimédia ».

| ✅ Correct               | ❌ Incorrect             |
| ----------------------- | ----------------------- |
| Supprimer le média      | Supprimer l'asset       |
| Les médias sélectionnés | Les assets sélectionnés |
| Ce média est utilisé    | Cet actif est utilisé   |

**Genre** : masculin → « le média », « les médias », « un média », « ce média »

### Listes (Bulleted/Numbered)

- **Bulleted list** → **Liste à puces**
- **Numbered list** → **Liste numérotée**

### Environment

Le terme **« environment »** se traduit par **« environnement »** en français :

| Anglais             | Français                |
| ------------------- | ----------------------- |
| sandbox environment | environnement sandbox   |
| primary environment | environnement principal |
| all environments    | tous les environnements |

### Déplier/Replier

- **« Expand »** → **« Déplier »**
- **« Collapse »** → **« Replier »**

| Anglais      | Français     |
| ------------ | ------------ |
| Expand       | Déplier      |
| Expand all   | Tout déplier |
| Collapse     | Replier      |
| Collapse all | Tout replier |

### Enregistrer (IMPORTANT)

Le terme **« Save »** se traduit **toujours** par **« Enregistrer »**. **Ne jamais** utiliser « Sauvegarder ».

| ✅ Correct                | ❌ Incorrect              |
| ------------------------ | ------------------------ |
| Enregistrer              | Sauvegarder              |
| Enregistrer l'élément    | Sauvegarder l'élément    |
| Enregistrer et continuer | Sauvegarder et continuer |

## Ce qui Sonne Naturel dans un SaaS Français

### Ton et Style

1. **Tutoiement** : Utilise « tu » de manière cohérente dans toute l'interface. Le tutoiement est le standard des SaaS modernes qui s'adressent à un public technique (développeurs, content managers).

2. **Messages concis** : Préfère les formulations directes et courtes :
   - ✅ « Élément créé avec succès ! »
   - ❌ « L'élément que tu as créé a bien été enregistré avec succès ! »

3. **Éviter le passif excessif** : Préfère la voix active quand c'est naturel :
   - ✅ « Impossible de sauvegarder l'élément »
   - ❌ « L'élément n'a pas pu être sauvegardé »

4. **Utiliser des verbes d'action** pour les boutons :
   - ✅ « Enregistrer », « Supprimer », « Publier »
   - ❌ « Sauvegarde », « Suppression », « Publication »

### Formulations Naturelles

| Anglais                      | Français naturel          |
| ---------------------------- | ------------------------- |
| Are you sure you want to...? | Tu veux vraiment... ?     |
| Successfully created         | Créé avec succès          |
| Failed to create             | Impossible de créer       |
| Please wait                  | Patiente un instant       |
| Loading...                   | Chargement...             |
| No items found               | Aucun élément trouvé      |
| Something went wrong         | Une erreur s'est produite |
| Try again                    | Réessayer                 |
| Learn more                   | En savoir plus            |
| Get started                  | Commencer                 |
| Sign in / Log in             | Se connecter              |
| Sign out / Log out           | Se déconnecter            |
| Sign up                      | S'inscrire                |

### Éviter les Anglicismes Inutiles

| ❌ Anglicisme | ✅ Français correct    |
| ------------ | --------------------- |
| Uploader     | Téléverser / Importer |
| Checker      | Vérifier              |
| Updater      | Mettre à jour         |
| Deleter      | Supprimer             |
| Saver        | Enregistrer           |

Mais conserver les termes techniques établis : **API**, **webhook**, **token**, **plugin**, **build**, **deploy**.

## Glossaire

```
"Add" → "Ajouter"
"API Token" → "Token d'API"
"Asset" → "Média"
"Block" → "Bloc"
"Build" → "Build" (ne pas traduire)
"Cancel" → "Annuler"
"Collection" → "Collection"
"Content" → "Contenu"
"Create" → "Créer"
"Custom" → "Personnalisé"
"Dashboard" → "Tableau de bord"
"DatoCMS Support" → "Support DatoCMS"
"Delete" → "Supprimer"
"Deploy" → "Déployer" / "Déploiement"
"Draft" → "Brouillon"
"Duplicate" → "Dupliquer"
"Edit" → "Modifier"
"Editor" → "Éditeur"
"Environment" → "Environnement"
"Error" → "Erreur"
"Field" → "Champ"
"File" → "Fichier"
"Filter" → "Filtre"
"Folder" → "Dossier"
"Image" → "Image"
"Information" → "Informations" (toujours au pluriel)
"Item" → "Élément"
"Locale" → "Langue" ou "Locale"
"Media Area" → "Espace médias" ou "Médiathèque"
"Menu item" → "Élément de menu"
"Model" → "Modèle"
"Permissions" → "Autorisations" ou "Permissions"
"Plugin" → "Plugin" (ne pas traduire)
"Preview" → "Aperçu"
"Private" → "Privé"
"Project" → "Projet"
"Publish" → "Publier"
"Record" → "Élément" ou "Enregistrement"
"Remove" → "Retirer"
"Role" → "Rôle"
"Save" → "Enregistrer" (jamais "Sauvegarder")
"Schema" → "Schéma"
"Search" → "Rechercher"
"Selected" → "Sélectionné(s)"
"Settings" → "Paramètres"
"Sidebar" → "Barre latérale"
"Success" → "Succès"
"Tag" → "Tag" (ne pas traduire)
"Title" → "Titre"
"Token" → "Token" (ne pas traduire)
"Unpublish" → "Dépublier"
"Update" → "Mettre à jour"
"Upload" → "Téléverser" ou "Importer"
"User" → "Utilisateur"
"Webhook" → "Webhook" (ne pas traduire)
```