# Guida alla Traduzione Italiana di DatoCMS

Questa guida definisce le regole per garantire coerenza nelle traduzioni italiane dell'interfaccia DatoCMS.

## Regole Fondamentali

- **Informal "tu"** throughout (mai "Lei" o "Voi")
- **Technical terms stay in English** (build, deploy, webhook, adapter, schema, hook, payload, environment)
- **Past participles agree with noun gender** ("creata" for singular feminine, "create" for plural)
- **"per favore"** sempre due parole (mai "perfavore")
- **Elisione obbligatoria** prima di vocale: "l'asset", "l'environment"
- **"scraping"** è maschile → "completato", non "completata"

## Regole di Disambiguazione

### Unpublish/Unpublishing (IMPORTANTE)

Il termine resta **sempre** in inglese. L'articolo "l'" è **obbligatorio**:

| ✅ Corretto                    | ❌ Sbagliato             |
| ----------------------------- | ----------------------- |
| Effettua **l'unpublish**      | Effettua unpublish      |
| Effettua **l'unpublishing**   | Effettua unpublishing   |
| effettuare **l'unpublish** di | effettuare unpublish di |

**Mai tradurre** come "spubblicare", "rimuovere pubblicazione", o "convertire in bozza".

### Titoli delle Dialog di Conferma

Per i titoli delle dialog che chiedono conferma, usare l'**infinitivo** con punto interrogativo:

| Tipo               | Esempio                                    |
| ------------------ | ------------------------------------------ |
| Dialog di conferma | "Eliminare questo record?"                 |
| Dialog di conferma | "Ripristinare questa versione?"            |
| Dialog di conferma | "Effettuare l'unpublish dei record figli?" |

Per i **pulsanti di azione**, usare l'**imperativo**:

| Tipo     | Esempio                |
| -------- | ---------------------- |
| Pulsante | "Elimina"              |
| Pulsante | "Ripristina"           |
| Pulsante | "Effettua l'unpublish" |

### Heading vs Titolo

- **"Heading"** (H1-H6 in editor di testo) → **"Intestazione"**
- **"Title"** (campo titolo, titolo pagina) → **"Titolo"**

| Inglese     | Italiano        |
| ----------- | --------------- |
| Heading 1   | Intestazione H1 |
| Heading 2   | Intestazione H2 |
| Title field | Campo titolo    |
| Page title  | Titolo pagina   |

### Punteggiatura nei Messaggi

| Tipo di messaggio       | Punteggiatura         | Esempio                                    |
| ----------------------- | --------------------- | ------------------------------------------ |
| **Errore/Fallimento**   | Punto esclamativo `!` | "Non è stato possibile salvare il record!" |
| **Successo con azione** | Punto esclamativo `!` | "Record salvato con successo!"             |
| **Successo neutro**     | Nessuna o punto       | "Record salvato con successo"              |
| **Descrizione/Info**    | Punto `.`             | "Questo campo è obbligatorio."             |
| **Label UI**            | Nessuna               | "Salva record"                             |

**Regola generale**: I messaggi di errore hanno **sempre** `!` per urgenza. I messaggi di successo possono avere `!` per enfasi o essere neutri.

### Pattern per Messaggi di Errore

Usare **sempre** il pattern "Non è stato possibile + infinito":

| ✅ Corretto                      | ❌ Sbagliato            |
| ------------------------------- | ---------------------- |
| Non è stato possibile salvare   | Impossibile salvare    |
| Non è stato possibile eliminare | Non posso eliminare    |
| Non è stato possibile caricare  | Errore nel caricamento |

### Expand/Collapse (IMPORTANTE)

Per le azioni di espansione e compressione di elementi UI:

- **"Expand"** → **"Espandi"** (imperativo) / **"espandere"** (infinitivo)
- **"Collapse"** → **"Collassa"** (imperativo) / **"collassare"** (infinitivo)

| Inglese      | Italiano (imperativo) | Italiano (infinitivo) |
| ------------ | --------------------- | --------------------- |
| Expand       | Espandi               | espandere             |
| Expand all   | Espandi tutti         | espandere tutti       |
| Collapse     | Collassa              | collassare            |
| Collapse all | Collassa tutti        | collassare tutti      |

**Mai tradurre** "collapse" come "comprimi/comprimere" o "chiudi/chiudere".

### Liste (Bulleted/Numbered)

- **Bulleted list** → **Elenco puntato** (non "Lista a punti")
- **Numbered list** → **Elenco numerato** (non "Lista numerata")

### Environment (IMPORTANTE)

Il termine **"environment"** resta **sempre** in inglese. **Mai tradurre** come "ambiente" o "ambienti".

| ✅ Corretto             | ❌ Sbagliato         |
| ---------------------- | ------------------- |
| environment sandbox    | ambiente sandbox    |
| l'environment primario | l'ambiente primario |
| tutti gli environment  | tutti gli ambienti  |
| nessun environment     | nessun ambiente     |

**Genere**: maschile → "l'environment", "gli environment", "questo environment"

## Glossary

```
"Add" → "Aggiungi"
"Block" → "Blocco"
"Custom asset storage" → "Asset storage personalizzato"
"DatoCMS Support" → "Supporto DatoCMS"
"DatoCMS-hosted assets" → "Asset ospitati da DatoCMS"
"Delete asset collection" → "Elimina raccolta asset"
"direct download URL" → "URL di download diretto"
"dragging and dropping" → "trascinandoli"
"Editor's Preferences" → "Preferenze dell'editor"
"Environment fast-fork" → "Fast-fork dell'environment"
"Error reporter" → "Reporter di errori"
"Facebook video" → "video di Facebook"
"Field appearance plugin" → "Plugin di apparenza del campo"
"File type" → "Tipo di file"
"information" → "informazioni"
"internet connection" → "connessione a internet"
"item" → "record"
"locales" → "lingue"
"Menu item" → "Voce di menù"
"Permissions" → "Permessi"
"platform" → "piattaforma"
"private" → "privato"
"project" → "progetto"
"publicly accessible" → "accessibile pubblicamente"
"Read-only mode" → "Modalità di sola lettura"
"restricted" → "limitato"
"Rollbar Error ID" → "ID errore Rollbar"
"scheduled maintenance" → "manutenzione programmata"
"Selected" → "Selezionati"
"selected" → "selezionato"
"selector" → "selettore"
"sidebar" → "barra laterale"
"tags" → "tag"
"Upload endpoint" → "Endpoint di caricamento"
"User account" → "Account utente"
"video platform" → "piattaforma video"
"video provider" → "provider video"
"Vimeo URL" → "URL di Vimeo"
"YouTube URL" → "URL di YouTube"
```