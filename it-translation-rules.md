# Guida alla Traduzione Italiana di DatoCMS

Questa guida definisce le regole per garantire coerenza nelle traduzioni italiane dell'interfaccia DatoCMS.

## Regole Fondamentali

- **Informal "tu"** throughout (mai "Lei" o "Voi")
- **Technical terms stay in English** (build, deploy, webhook, adapter, schema, hook, payload, environment)
- **Past participles agree with noun gender** ("creata" for singular feminine, "create" for plural)
- **"per favore"** sempre due parole (mai "perfavore")
- **Elisione obbligatoria** prima di vocale: "l'item", "l'asset", "l'environment" (mai "il item")
- **"scraping"** è maschile → "completato", non "completata"

## Regole di Disambiguazione

### 1. Unpublish/Unpublishing (IMPORTANTE)

Il termine resta **sempre** in inglese. L'articolo "l'" è **obbligatorio**:

| ✅ Corretto | ❌ Sbagliato |
|-------------|--------------|
| Effettua **l'unpublish** | Effettua unpublish |
| Effettua **l'unpublishing** | Effettua unpublishing |
| effettuare **l'unpublish** di | effettuare unpublish di |

**Mai tradurre** come "spubblicare", "rimuovere pubblicazione", o "convertire in bozza".

### 2. Titoli delle Dialog di Conferma

Per i titoli delle dialog che chiedono conferma, usare l'**infinitivo** con punto interrogativo:

| Tipo | Esempio |
|------|---------|
| Dialog di conferma | "Eliminare questo record?" |
| Dialog di conferma | "Ripristinare questa versione?" |
| Dialog di conferma | "Effettuare l'unpublish dei record figli?" |

Per i **pulsanti di azione**, usare l'**imperativo**:

| Tipo | Esempio |
|------|---------|
| Pulsante | "Elimina" |
| Pulsante | "Ripristina" |
| Pulsante | "Effettua l'unpublish" |

### 3. Heading vs Titolo

- **"Heading"** (H1-H6 in editor di testo) → **"Intestazione"**
- **"Title"** (campo titolo, titolo pagina) → **"Titolo"**

| Inglese | Italiano |
|---------|----------|
| Heading 1 | Intestazione H1 |
| Heading 2 | Intestazione H2 |
| Title field | Campo titolo |
| Page title | Titolo pagina |

### 4. Punteggiatura nei Messaggi

| Tipo di messaggio | Punteggiatura | Esempio |
|-------------------|---------------|---------|
| **Errore/Fallimento** | Punto esclamativo `!` | "Non è stato possibile salvare il record!" |
| **Successo con azione** | Punto esclamativo `!` | "Record salvato con successo!" |
| **Successo neutro** | Nessuna o punto | "Record salvato con successo" |
| **Descrizione/Info** | Punto `.` | "Questo campo è obbligatorio." |
| **Label UI** | Nessuna | "Salva record" |

**Regola generale**: I messaggi di errore hanno **sempre** `!` per urgenza. I messaggi di successo possono avere `!` per enfasi o essere neutri.

### 5. Pattern per Messaggi di Errore

Usare **sempre** il pattern "Non è stato possibile + infinito":

| ✅ Corretto | ❌ Sbagliato |
|-------------|--------------|
| Non è stato possibile salvare | Impossibile salvare |
| Non è stato possibile eliminare | Non posso eliminare |
| Non è stato possibile caricare | Errore nel caricamento |

### 6. Liste (Bulleted/Numbered)

- **Bulleted list** → **Elenco puntato** (non "Lista a punti")
- **Numbered list** → **Elenco numerato** (non "Lista numerata")

### 7. Environment (IMPORTANTE)

Il termine **"environment"** resta **sempre** in inglese. **Mai tradurre** come "ambiente" o "ambienti".

| ✅ Corretto | ❌ Sbagliato |
|-------------|--------------|
| environment sandbox | ambiente sandbox |
| l'environment primario | l'ambiente primario |
| tutti gli environment | tutti gli ambienti |
| nessun environment | nessun ambiente |

**Genere**: maschile → "l'environment", "gli environment", "questo environment"

## Glossary

"Menu item" -> "Voce di menù"
"Clear selection" → "Deseleziona tutto"
"Asset collection" → "Raccolta asset"
"Build trigger" → "Build trigger"
"Crawler log" → "Log del crawler"
"Event type" → "Tipo di evento"
"Event date" → "Data evento"
"Update details" → "Dettagli aggiornamento"
"Draft" → "Draft"
"Asset" → "Asset"
"Collection" → "Raccolta"
"Permissions" → "Permessi"
"URL" → "URL"
"File type" → "Tipo di file"
"Custom asset storage" → "Asset storage personalizzato"
"DatoCMS-hosted assets" → "Asset ospitati da DatoCMS"
"Upload endpoint" → "Endpoint di caricamento"
"Ad blocker" → "Ad blocker"
"VPN" → "VPN"
"Error reporter" → "Reporter di errori"
"Rollbar Error ID" → "ID errore Rollbar"
"DatoCMS Support" → "Supporto DatoCMS"
"User account" → "Account utente"
"Read-only mode" → "Modalità di sola lettura"
"Environment" → "Environment" (maschile, non tradurre)
"Environment fast-fork" → "Fast-fork dell'environment"
"Record" → "Record"
"Field appearance plugin" → "Plugin di apparenza del campo"
"assets" → "asset"
"collection" → "raccolta"
"tags" → "tag"
"URL" → "URL"
"CDN" → "CDN"
"environment" → "environment"
"read-only mode" → "modalità di sola lettura"
"fast-fork" → "fast-fork"
"locales" → "lingue"
"Editor's Preferences" → "Preferenze dell'editor"
"selector" → "selettore"
"avatar" → "avatar"
"records" → "record"
"project" → "progetto"
"scheduled maintenance" → "manutenzione programmata"
"All assets" → "Tutti gli asset"
"Assign to collection" → "Assegna a raccolta"
"Move to collection" → "Sposta in raccolta"
"Not in a collection" → "Non in una raccolta"
"Add tags" → "Aggiungi tag"
"Create the first collection" → "Crea la prima raccolta"
"Organize your media assets" → "Organizza i tuoi asset multimediali"
"Cancel" → "Annulla"
"Create a new URL" → "Crea un nuovo URL"
"Keep original URL" → "Mantieni URL originale"
"How should we handle the URL?" → "Come dovremmo gestire l'URL?"
"Yes, delete" → "Sì, elimina"
"Delete asset collection" → "Elimina raccolta asset"
"Apply this choice to all duplicate files" → "Applica questa scelta a tutti i file duplicati"
"Your account cannot access any project environment" → "Il tuo account non può accedere a nessun environment del progetto"
"Find results in" → "Trova risultati in"
"Search" → "Cerca"
"Missing" → "Mancante"
"Outdated" → "Obsoleto"
"Published" → "Pubblicato"
"Still published" → "Ancora pubblicato"
"Current locales status" → "Stato lingue correnti"
"In-sync" → "Sincronizzato"
"Not in-sync" → "Non sincronizzato"
"collapse" → "comprimere"
"item" → "elemento"
"selected" → "selezionato"
"Move" → "Sposta"
"collection" → "raccolta"
"asset" → "asset"
"asset collection" → "raccolta asset"
"Collection" → "Raccolta"
"dragging and dropping" → "trascinandoli"
"sidebar" → "barra laterale"
"Add" → "Aggiungi"
"Save" → "Salva"
"Delete" → "Elimina"
"Edit" → "Modifica"
"Label" → "Etichetta"
"Edit collection" → "Modifica raccolta"
"Facebook video" → "video di Facebook"
"information" → "informazioni"
"internet connection" → "connessione a internet"
"video" → "video"
"platform" → "piattaforma"
"URL" → "URL"
"publicly accessible" → "accessibile pubblicamente"
"private" → "privato"
"restricted" → "limitato"
"video platform" → "piattaforma video"
"YouTube" → "YouTube"
"Vimeo" → "Vimeo"
"Facebook" → "Facebook"
"video provider" → "provider video"
"Vimeo URL" → "URL di Vimeo"
"YouTube URL" → "URL di YouTube"
"direct download URL" → "URL di download diretto"
"Editor" → "Editor"
"Published at" → "Pubblicato il"
"In-sync" → "Sincronizzato"
"Not in-sync" → "Non sincronizzato"
"Collapse" → "Comprimi"
"Copy" → "Copia"
"Duplicate" → "Duplica"
"Add new block below" → "Aggiungi nuovo blocco sotto"
"Add new block above" → "Aggiungi nuovo blocco sopra"
"Move" → "Sposta"
"Move to the bottom" → "Sposta in fondo"
"Move down" → "Sposta giù"
"Move to the top" → "Sposta in cima"
"Move up" → "Sposta su"
"Paste to the bottom" → "Incolla in fondo"
"Paste below this block" → "Incolla sotto questo blocco"
"Paste to the top" → "Incolla in cima"
"Paste above this block" → "Incolla sopra questo blocco"
"Expand" → "Espandi"
"Save preferences" → "Salva preferenze"
"Add Inline Block" → "Aggiungi blocco inline"
"Mixed" → "Misto"
"Bulleted list" → "Elenco puntato"
"Insert" → "Inserisci"
"Numbered list" → "Elenco numerato"
"Thematic break" → "Interruzione tematica"
"Block" → "Blocco"
"Selected" → "Selezionati"