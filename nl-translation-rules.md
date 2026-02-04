# Handleiding voor Nederlandse Vertalingen van DatoCMS

Deze handleiding definieert de regels om consistentie te waarborgen in de Nederlandse vertalingen van de DatoCMS-interface.

## Basisregels

- **Informeel "je/jij"** door de hele interface (nooit "u")
- **Technische termen in het Engels houden**: build, build trigger, deploy, webhook, adapter, schema, hook, payload, token, plugin, API, SEO, URL, asset
- **"Asset"** blijft **altijd** in het Engels (niet vertalen als "bestand" of "media")
- **"Save"** vertalen als **"Opslaan"** (nooit "Bewaren")
- **Geen spatie voor leestekens** `!`, `?`, `:`, `;` (dit is correct Nederlands, anders dan Frans)
- **Mannelijk standaard**: wanneer het geslacht niet duidelijk is, gebruik mannelijk ("Aangemaakt" niet "Aangemaakt(e)")

## Regels voor Verduidelijking

### Bijgewerkt vs Geüpdatet (BELANGRIJK)

Gebruik **altijd** "bijgewerkt" of "bijwerken". Vermijd de anglicismen "geüpdatet", "geupdate" of "updaten".

| ✅ Correct               | ❌ Fout                |
| ----------------------- | --------------------- |
| Item bijgewerkt         | Item geüpdatet        |
| Item bijwerken mislukt! | Item updaten mislukt! |
| Bijgewerkt op           | Geüpdatet op          |
| Filter bijwerken        | Filter updaten        |

### Inconsistenties om te Corrigeren

De huidige vertalingen bevatten inconsistenties die gecorrigeerd moeten worden:

| Huidige (Fout)              | Correcte Vertaling        |
| --------------------------- | ------------------------- |
| `Item updaten mislukt!`     | `Item bijwerken mislukt!` |
| `Menu-items geupdate`       | `Menu-items bijgewerkt`   |
| `Geupdate content`          | `Bijgewerkte content`     |
| `gallerij` (meerdere keren) | `galerij` (één l)         |

### Depubliceren (Unpublish)

In het Nederlands gebruiken we **"depubliceren"** (werkwoord) en **"depublicatie"** (zelfstandig naamwoord):

| Engels                   | Nederlands            |
| ------------------------ | --------------------- |
| Unpublish                | Depubliceren          |
| Unpublishing             | Depublicatie          |
| Couldn't unpublish       | Depubliceren mislukt! |
| Successfully unpublished | Gedepubliceerd        |

### Titels van Bevestigingsdialogen

Voor titels van dialoogvensters die bevestiging vragen, gebruik de **infinitief** met vraagteken:

| Type                | Voorbeeld             |
| ------------------- | --------------------- |
| Bevestigingsdialoog | Item verwijderen?     |
| Bevestigingsdialoog | Versie herstellen?    |
| Bevestigingsdialoog | Publicatie annuleren? |

Voor **actieknoppen**, gebruik de **infinitief**:

| Type | Voorbeeld    |
| ---- | ------------ |
| Knop | Verwijderen  |
| Knop | Depubliceren |
| Knop | Opslaan      |

### Heading vs Titel

- **"Heading"** (H1-H6 in teksteditor) → **"Heading"** (Heading 1, Heading 2, etc.) — we behouden de Engelse term omdat dit de standaard HTML-terminologie is die ontwikkelaars kennen.
- **"Title"** (titelveld, paginatitel) → **"Titel"**

| Engels      | Nederlands  |
| ----------- | ----------- |
| Heading 1   | Heading 1   |
| Heading 2   | Heading 2   |
| Title field | Titelveld   |
| Page title  | Paginatitel |

### Leestekens in Berichten

| Type bericht          | Leesteken        | Voorbeeld                  |
| --------------------- | ---------------- | -------------------------- |
| **Fout/Mislukt**      | Uitroepteken `!` | Item opslaan mislukt!      |
| **Succes met actie**  | Uitroepteken `!` | Item succesvol aangemaakt! |
| **Succes neutraal**   | Geen of punt     | Item opgeslagen            |
| **Beschrijving/Info** | Punt `.`         | Dit veld is verplicht.     |
| **UI-label**          | Geen             | Item opslaan               |

### Patronen voor Foutmeldingen

Gebruik **consistent** het patroon "... mislukt!" of "Kon ... niet ...":

| ✅ Correct                  | ❌ Fout                  |
| -------------------------- | ----------------------- |
| Item opslaan mislukt!      | Fout bij opslaan        |
| Kon item niet verwijderen! | Error: item verwijderen |
| Bestand uploaden mislukt!  | Upload gefaald          |

### Uitvouwen/Invouwen

- **"Expand"** → **"Uitvouwen"** of **"Uitklappen"**
- **"Collapse"** → **"Invouwen"** of **"Inklappen"**

| Engels       | Nederlands      |
| ------------ | --------------- |
| Expand       | Uitvouwen       |
| Expand all   | Alles uitvouwen |
| Collapse     | Invouwen        |
| Collapse all | Alles invouwen  |

### Record (BELANGRIJK)

Gebruik **altijd** "record" voor content-eenheden, in zowel gebruikersgerichte als technische contexten. Gebruik **nooit** "item" als vertaling van "record".

| Engels            | Nederlands            |
| ----------------- | --------------------- |
| Record            | Record                |
| Create new record | Nieuw record aanmaken |
| No records found  | Geen records gevonden |

### Galerij (BELANGRIJK)

Het Nederlandse woord "galerij" wordt geschreven met **één l**:

| ✅ Correct     | ❌ Fout         |
| ------------- | -------------- |
| Media-galerij | Media-gallerij |
| Uit galerij   | Uit gallerij   |

## Wat Natuurlijk Aanvoelt in een Nederlands SaaS-product

### Toon en Stijl

1. **Informeel "je"**: Gebruik consistent "je" door de hele interface. Dit is de standaard voor moderne SaaS-producten.

2. **Directe berichten**: Geef voorkeur aan korte, duidelijke formuleringen:
   - ✅ "Item aangemaakt!"
   - ❌ "Het item dat je hebt aangemaakt is succesvol opgeslagen!"

3. **Vermijd passief waar mogelijk**: Geef voorkeur aan actieve formuleringen:
   - ✅ "Kon item niet opslaan!"
   - ❌ "Het item kon niet worden opgeslagen!"

4. **Actiegerichte knoppen**: Gebruik werkwoorden voor knoppen:
   - ✅ "Opslaan", "Verwijderen", "Publiceren"
   - ❌ "Opslag", "Verwijdering", "Publicatie"

### Natuurlijke Formuleringen

| Engels                       | Natuurlijk Nederlands    |
| ---------------------------- | ------------------------ |
| Are you sure you want to...? | Weet je zeker dat je...? |
| Successfully created         | Aangemaakt               |
| Failed to create             | Aanmaken mislukt!        |
| Please wait                  | Even geduld...           |
| Loading...                   | Laden...                 |
| No items found               | Geen items gevonden      |
| Something went wrong         | Er ging iets mis         |
| Try again                    | Probeer opnieuw          |
| Learn more                   | Meer informatie          |
| Get started                  | Aan de slag              |
| Sign in / Log in             | Inloggen                 |
| Sign out / Log out           | Uitloggen                |
| Sign up                      | Registreren              |

### Vermijd Onnodige Anglicismen

| ❌ Anglicisme | ✅ Correct Nederlands    |
| ------------ | ----------------------- |
| Uploaden     | Uploaden (geaccepteerd) |
| Deleten      | Verwijderen             |
| Saven        | Opslaan                 |
| Editen       | Bewerken                |
| Updaten      | Bijwerken               |

"Checken" is geaccepteerd als informeel alternatief voor "controleren" — het past bij de informele toon van de interface.

Maar behoud gevestigde technische termen: **API**, **webhook**, **token**, **plugin**, **build**, **deploy**, **asset**.

## Woordenlijst

```
"Add" → "Toevoegen"
"API Token" → "API-token"
"Asset" → "Asset" (niet vertalen)
"Block" → "Blok"
"Build" → "Build" (niet vertalen)
"Cancel" → "Annuleren"
"Check" → "Checken" of "Controleren"
"Collection" → "Collectie"
"Content" → "Content" of "Inhoud"
"Create" → "Aanmaken"
"Custom" → "Aangepast"
"Dashboard" → "Dashboard"
"DatoCMS Support" → "DatoCMS Support"
"Delete" → "Verwijderen"
"Deploy" → "Deployen" / "Deployment"
"Draft" → "Concept"
"Duplicate" → "Dupliceren"
"Edit" → "Bewerken"
"Editor" → "Editor"
"Environment" → "Environment" of "Omgeving"
"Error" → "Fout"
"Field" → "Veld"
"File" → "Bestand"
"Filter" → "Filter"
"Folder" → "Map"
"Gallery" → "Galerij" (één l!)
"Heading" → "Heading" (niet vertalen)
"Image" → "Afbeelding"
"Information" → "Informatie"
"Item" → "Record" (voor content-eenheden; "menu-item" blijft "menu-item")
"Locale" → "Taal" of "Lokalisatie"
"Media Area" → "Media-galerij"
"Menu item" → "Menu-item"
"Model" → "Model"
"Permissions" → "Rechten" of "Permissies"
"Plugin" → "Plugin" (niet vertalen)
"Preview" → "Voorbeeld"
"Private" → "Privé"
"Project" → "Project"
"Publish" → "Publiceren"
"Record" → "Record"
"Remove" → "Verwijderen"
"Role" → "Rol"
"Save" → "Opslaan" (nooit "Bewaren")
"Schema" → "Schema"
"Search" → "Zoeken"
"Selected" → "Geselecteerd"
"Settings" → "Instellingen"
"Sidebar" → "Zijbalk"
"Success" → "Gelukt" of "Succesvol"
"Tag" → "Tag" (niet vertalen)
"Title" → "Titel"
"Token" → "Token" (niet vertalen)
"Unpublish" → "Depubliceren"
"Update" → "Bijwerken" (NIET "updaten")
"Upload" → "Uploaden"
"User" → "Gebruiker"
"Webhook" → "Webhook" (niet vertalen)
```