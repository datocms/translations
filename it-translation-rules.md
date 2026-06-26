# Guida alla Traduzione Italiana di DatoCMS

Questa guida definisce le regole per garantire coerenza nelle traduzioni italiane dell'interfaccia DatoCMS.

## Regole Fondamentali

- **Informal "tu"** throughout (mai "Lei" o "Voi")
- **Technical terms stay in English** (build, build trigger, deploy, webhook, adapter, schema, hook, payload, environment)
- **Past participles agree with noun gender** ("creata" for singular feminine, "create" for plural)
- **"per favore"** sempre due parole (mai "perfavore")
- **Elisione obbligatoria** prima di vocale: "l'asset", "l'environment"
- **"scraping"** è maschile → "completato", non "completata"

## Linguaggio Senza Genere (IMPORTANTE)

Quando il testo si rivolge all'**utente** (di cui non conosciamo il genere), evitare aggettivi e participi passati che richiedono accordo di genere. Riformulare con costruzioni verbali neutre.

| ✅ Corretto (senza genere)         | ❌ Sbagliato (con genere)        |
| --------------------------------- | ------------------------------- |
| Vuoi davvero eliminare…?          | Sei sicuro di voler eliminare…? |
| Iniziamo! / Tutto pronto!         | Benvenuto!                      |
| Conferma di voler procedere       | Sei certo di voler procedere    |
| Devi effettuare l'accesso         | Devi essere loggato             |

**Strategie**:

- Preferire forme verbali: "Vuoi…?", "Confermi…?", "Devi…" invece di "Sei sicuro/pronto/connesso".
- Per i messaggi di benvenuto evitare "Benvenuto/Benvenuta": preferire forme neutre e naturali come "Iniziamo!", "Tutto pronto!", "Buon lavoro!", "Ci siamo!". "Ti diamo il benvenuto" è corretto ma più formale.
- Riformulare attorno all'azione, non allo stato dell'utente.

**Importante**: questa regola riguarda **solo** il testo riferito all'utente. I participi e gli aggettivi riferiti a **oggetti** (record, asset, environment) mantengono il normale accordo di genere grammaticale (vedi "Past participles agree with noun gender").

## Regole di Disambiguazione

### Unpublish/Unpublishing (IMPORTANTE)

Il termine resta **sempre** in inglese. L'articolo "l'" è **obbligatorio**:

| ✅ Corretto                    | ❌ Sbagliato             |
| ----------------------------- | ----------------------- |
| Effettua **l'unpublish**      | Effettua unpublish      |
| Effettua **l'unpublishing**   | Effettua unpublishing   |
| effettuare **l'unpublish** di | effettuare unpublish di |

**Mai tradurre** come "spubblicare", "rimuovere pubblicazione", o "convertire in bozza".

**Regola dello specchio (IMPORTANTE)**: il suffisso italiano segue **sempre** quello inglese, 1:1. Mai mischiare le due forme per la stessa stringa inglese.

- inglese `unpublish` (verbo) → **`l'unpublish`** ("Effettua l'unpublish", "effettuare l'unpublish di…", "Unpublish at a specific date" → "Effettua l'unpublish a una data…")
- inglese `unpublishing` (sostantivo/gerundio) → **`l'unpublishing`** ("Schedule unpublishing" → "Programma l'unpublishing", "Scheduled unpublishing" → "unpublishing programmato")

### Draft (IMPORTANTE)

Il termine **"draft"** resta **sempre** in inglese. **Mai tradurre** come "bozza".

| ✅ Corretto           | ❌ Sbagliato         |
| -------------------- | ------------------- |
| Draft creato         | Bozza creata        |
| draft non validi     | bozze non valide    |
| impostato come draft | impostato come bozza |
| modalità draft       | modalità bozza      |

**Genere**: maschile → "il draft", "i draft", "creato come draft"

### Publish (IMPORTANTE)

A differenza di `unpublish`, **`publish` si traduce** con il verbo nativo italiano (l'asimmetria è voluta ed è corretta).

| Inglese                              | ✅ Corretto              |
| ------------------------------------ | ----------------------- |
| Publish / to publish                 | Pubblica / pubblicare   |
| Published (stato)                    | Pubblicato              |
| publication, publishing (sostantivo) | pubblicazione           |
| Unpublished changes                  | Modifiche non pubblicate |

### Schedule / Scheduling (IMPORTANTE)

Per pubblicazioni e unpublishing differiti nel tempo, usare **sempre** la famiglia **programmare / programmato / programma**. **Vietati**: `pianificare`/`pianificazione`, `schedulare`/`schedulazione`. **Mai** tradurre `scheduled` come "automatica" o "futura".

| Inglese                   | ✅ Corretto                   | ❌ Sbagliato                             |
| ------------------------- | ---------------------------- | --------------------------------------- |
| to schedule (verbo)       | programmare                  | pianificare, schedulare                 |
| scheduled (aggettivo)     | programmato / programmata    | automatico/a, futuro/a, pianificato/a   |
| schedule (il piano)       | programma di pubblicazione   | pianificazione, schedulazione           |
| Add new schedule          | Programma una nuova azione   | Aggiungi nuova pianificazione, Programma pubblicazione futura |
| Scheduled publishing at   | Pubblicazione programmata il | Futura pubblicazione il                 |
| Scheduled unpublishing at | Unpublishing programmato il  | Futuro unpublishing il                  |

Una "schedule" (la singola regola differita) copre **sia publish che unpublish**: per i titoli generici non assumere mai il solo contesto di pubblicazione.

**Annullare una schedulazione**: `cancel` → **`annullare` / `annullata`** ovunque (titoli, toast di successo, errori), così il dialog di conferma e la toast finale usano lo stesso verbo. Eccezioni di mirroring: `Cancel` (bottone generico) → "Annulla"; `stop` (dove l'inglese lo usa davvero, es. "stop automatic publication") → "interrompi"; `automatic`/`automatically` → "automatico"/"automaticamente".

| Inglese                                | ✅ Corretto                                        |
| -------------------------------------- | ------------------------------------------------- |
| Cancel scheduled publication?          | Annullare la pubblicazione programmata?           |
| Scheduled publication … cancelled!     | Pubblicazione programmata annullata con successo! |
| Couldn't cancel scheduled publication! | Non è stato possibile annullare la pubblicazione programmata! |
| Yes, stop automatic publication        | Sì, interrompi la pubblicazione automatica        |

### Stati del Record

Gli stati seguono **letteralmente** l'inglese (non interpretare):

| Inglese                     | ✅ Corretto                         |
| --------------------------- | ---------------------------------- |
| Published                   | Pubblicato                         |
| Published (unsaved changes) | Pubblicato (modifiche non salvate) |
| Not published               | Non pubblicato                     |
| Unpublished changes         | Modifiche non pubblicate           |

Nota: `Not published` → **"Non pubblicato"** (non "Draft"); la regola "draft resta inglese" vale solo quando l'inglese dice davvero `draft`.

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
"Sales team" → "Sales team"
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