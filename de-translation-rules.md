# Leitfaden für die deutsche Übersetzung von DatoCMS

Dieser Leitfaden definiert die Regeln für eine konsistente deutsche Übersetzung der DatoCMS-Oberfläche.

## Grundregeln

- **Informelles "du"** durchgehend verwenden (niemals "Sie")
- **Technische Begriffe bleiben auf Englisch** (build, build trigger, deploy, webhook, adapter, schema, hook, payload, environment)
- **"bitte"** immer klein, außer am Satzanfang

## Geschlechtsneutrale Sprache

Das Deutsche ist eine Sprache mit grammatischem Geschlecht, und das Geschlecht der angesprochenen Person ist unbekannt. Bei Texten, die sich **an die nutzende Person richten**, daher geschlechtsneutrale Formulierungen bevorzugen.

**Strategien:**

- **Direkte Ansprache mit "du"** ist der sicherste neutrale Weg: Prädikative Partizipien und Adjektive flektieren in der du-Form nicht ("Du bist angemeldet" gilt für jedes Geschlecht).
- **Keine geschlechtsmarkierten Rollenbezeichnungen** für die angesprochene Person (Benutzer/Benutzerin, Administrator, Mitarbeiter). Stattdessen umformulieren oder direkt mit "du" ansprechen.
- **Keine nominalisierten Partizipien** ("der Eingeladene", "ein Angemeldeter"); stattdessen verbale Formen verwenden ("Du wurdest eingeladen", "Du bist angemeldet").
- **Keine Gendersonderzeichen** (Nutzer*innen, NutzerInnen, Nutzer:innen) in der Oberfläche; stattdessen echte neutrale Umformulierung.

| ✅ Korrekt                          | ❌ Falsch                              |
| ----------------------------------- | ------------------------------------- |
| Du bist angemeldet                  | Du bist ein angemeldeter Benutzer     |
| Du wurdest zum Projekt eingeladen   | Du bist der Eingeladene des Projekts  |
| Du musst angemeldet sein            | Du musst ein angemeldeter Nutzer sein |
| Willkommen an Bord!                 | Willkommen, lieber Nutzer!            |

**WICHTIG:** Dies gilt **nur** für Texte, die sich auf die nutzende Person beziehen. Partizipien und Adjektive, die sich auf **Objekte** beziehen (Datensatz, Asset, Umgebung), behalten ihre normale grammatische Geschlechtsübereinstimmung: "Datensatz erfolgreich gelöscht", "Veröffentlicht", "diese Umgebung".

## Disambiguierungsregeln

### Record/Datensatz (WICHTIG)

Das englische "record" oder "item" wird **immer** als **"Datensatz"** übersetzt:

| ✅ Korrekt                              | ❌ Falsch                            |
| -------------------------------------- | ----------------------------------- |
| Datensatz erfolgreich erstellt         | Eintrag erfolgreich erstellt        |
| Datensatz konnte nicht gelöscht werden | Platte konnte nicht gelöscht werden |
| Neuer Datensatz                        | Neue Aufnahme                       |
| Datensatz speichern                    | Eintrag speichern                   |

**Niemals** "Platte", "Aufnahme" oder "Eintrag" als Übersetzung für "record" verwenden.

### Unpublish/Unveröffentlichen (WICHTIG)

Der Begriff wird **immer** als **"unveröffentlichen"** (Verb) oder **"Unveröffentlichung"** (Substantiv) übersetzt:

| ✅ Korrekt                   | ❌ Falsch                      |
| --------------------------- | ----------------------------- |
| Datensatz unveröffentlichen | Datensatz unpublizieren       |
| Unveröffentlichung          | Veröffentlichung zurückziehen |
| Geplante Unveröffentlichung | Geplante Unpublizierung       |
| unveröffentlicht            | Ent-Veröffentlichung          |

**Niemals** "unpublizieren", "Unpublizierung", "Veröffentlichung zurückziehen", "aus der Veröffentlichung entfernen" oder "Ent-Veröffentlichung" verwenden.

### Geplante Veröffentlichung (Schedule/Scheduling) (WICHTIG)

Für zeitlich verschobene Veröffentlichungen und Unveröffentlichungen **immer** eine einzige konsistente Wortfamilie verwenden. Konkurrierende Varianten sind **verboten**.

- **"to schedule"** (Verb) → **"planen"** ("zur Veröffentlichung planen", "für die Unveröffentlichung planen"). Niemals "terminieren", "schedulen" oder das alleinstehende "festlegen".
- **"scheduled"** (Adjektiv) → **"geplant/geplante"**. **Niemals** "automatisch" oder "zukünftig" als Übersetzung für "scheduled".
- **"a schedule"** (die Planung selbst) → **"Planung"**. Niemals "Zeitplan" oder "Terminplan".

| Englisch                | ✅ Korrekt                              | ❌ Falsch                              |
| ----------------------- | -------------------------------------- | ------------------------------------- |
| to schedule (Verb)      | zur Veröffentlichung planen            | zur Veröffentlichung terminieren      |
| scheduled (Adjektiv)    | Geplante Veröffentlichung              | Automatische Veröffentlichung         |
| a schedule (Substantiv) | Planung                                | Zeitplan                              |
| Add new schedule        | Neue Planung hinzufügen                | Neuen Zeitplan hinzufügen             |
| Scheduled publishing at | Geplante Veröffentlichung am           | Zukünftige Veröffentlichung am        |
| Scheduled unpublishing at | Geplante Unveröffentlichung am       | Automatische Unveröffentlichung am    |

Eine "Planung" (die einzelne zeitversetzte Regel) umfasst **sowohl Veröffentlichung als auch Unveröffentlichung**: generische Titel dürfen keinen reinen Veröffentlichungskontext voraussetzen.

**Abbrechen einer Planung:** durchgehend **denselben** Verbstamm **"abbrechen"** verwenden, damit Bestätigungsdialog, Erfolgsmeldung und Fehlermeldung übereinstimmen. **Niemals** "absagen" oder "stornieren" für diesen Vorgang verwenden.

| Englisch                                      | ✅ Korrekt                                          |
| --------------------------------------------- | -------------------------------------------------- |
| Cancel scheduled publication?                 | Geplante Veröffentlichung abbrechen?               |
| Scheduled publication successfully cancelled! | Geplante Veröffentlichung erfolgreich abgebrochen! |
| Couldn't cancel scheduled publication!        | Geplante Veröffentlichung konnte nicht abgebrochen werden! |
| Yes, stop automatic publication               | Ja, automatische Veröffentlichung stoppen          |

**Spiegelungs-Ausnahmen:** Die generische Schaltfläche "Cancel" bleibt "Abbrechen"; wo das Englische tatsächlich "stop" sagt, wird "stoppen" verwendet ("automatische Veröffentlichung stoppen"); "automatic/automatically" wird zu "automatisch".

### Datensatz-Status (Record states)

Die Statusbezeichnungen folgen dem Englischen **wörtlich** (nicht interpretieren):

| Englisch                    | Deutsch                                       |
| --------------------------- | --------------------------------------------- |
| Published                   | Veröffentlicht                                |
| Published (unsaved changes) | Veröffentlicht (nicht gespeicherte Änderungen) |
| Not published               | Nicht veröffentlicht                          |
| Unpublished changes         | Unveröffentlichte Änderungen                  |

**WICHTIG:** "Not published" darf **niemals** zu "Entwurf" (Draft) werden. Die Regel "Draft bleibt Entwurf" gilt **nur**, wenn das Englische wirklich "draft" sagt.

### Expand/Collapse (WICHTIG)

Für das Erweitern und Zusammenklappen von UI-Elementen:

- **"Expand"** → **"Ausklappen"** (Imperativ) / **"ausklappen"** (Infinitiv)
- **"Collapse"** → **"Einklappen"** (Imperativ) / **"einklappen"** (Infinitiv)

| Englisch     | Deutsch (Imperativ) | Deutsch (Infinitiv) |
| ------------ | ------------------- | ------------------- |
| Expand       | Ausklappen          | ausklappen          |
| Expand all   | Alle ausklappen     | alle ausklappen     |
| Collapse     | Einklappen          | einklappen          |
| Collapse all | Alle einklappen     | alle einklappen     |

**Niemals** "zusammenklappen" oder "erweitern" für diese Aktionen verwenden.

### Block (Plural)

Der Plural von "Block" ist im Deutschen **"Blöcke"**:

| ✅ Korrekt                  | ❌ Falsch                   |
| -------------------------- | -------------------------- |
| Alle Blöcke ausklappen     | Alle Blocks ausklappen     |
| 3 von 5 Blöcken ausgewählt | 3 von 5 Blocks ausgewählt  |
| Blöcke erfolgreich kopiert | Blocks erfolgreich kopiert |

### Environment/Umgebung

Der Begriff **"environment"** wird als **"Umgebung"** übersetzt. Dies entspricht der etablierten deutschen Software-Terminologie.

| Englisch              | Deutsch                |
| --------------------- | ---------------------- |
| Sandbox environment   | Sandbox-Umgebung       |
| Primary environment   | Primäre Umgebung       |
| All environments      | Alle Umgebungen        |
| Environment settings  | Umgebungseinstellungen |
| Switch to environment | Zur Umgebung wechseln  |

**Genus**: Feminin → "die Umgebung", "die Umgebungen", "diese Umgebung"

### Titel bei Bestätigungsdialogen

Für Titel von Bestätigungsdialogen den **Infinitiv** mit Fragezeichen verwenden:

| Typ                | Beispiel                          |
| ------------------ | --------------------------------- |
| Bestätigungsdialog | "Diesen Datensatz löschen?"       |
| Bestätigungsdialog | "Diese Version wiederherstellen?" |
| Bestätigungsdialog | "Datensatz unveröffentlichen?"    |

Für **Aktionsschaltflächen** den **Imperativ** verwenden:

| Typ          | Beispiel            |
| ------------ | ------------------- |
| Schaltfläche | "Löschen"           |
| Schaltfläche | "Wiederherstellen"  |
| Schaltfläche | "Unveröffentlichen" |

### Überschriften (Headings)

- **"Heading"** (H1-H6 im Texteditor) → **"Überschrift"**
- **"Title"** (Titelfeld, Seitentitel) → **"Titel"**

| Englisch    | Deutsch       |
| ----------- | ------------- |
| Heading 1   | Überschrift 1 |
| Heading 2   | Überschrift 2 |
| Title field | Titelfeld     |
| Page title  | Seitentitel   |

### Listen (Bulleted/Numbered)

- **Bulleted list** → **Aufzählungsliste** (nicht "Aufzählung" allein)
- **Numbered list** → **Nummerierte Liste**

### Zeichensetzung in Meldungen

| Nachrichtentyp        | Zeichensetzung     | Beispiel                                         |
| --------------------- | ------------------ | ------------------------------------------------ |
| **Fehler**            | Ausrufezeichen `!` | "Der Datensatz konnte nicht gespeichert werden!" |
| **Erfolg mit Aktion** | Ausrufezeichen `!` | "Datensatz erfolgreich gespeichert!"             |
| **Neutraler Erfolg**  | Keine oder Punkt   | "Datensatz erfolgreich gespeichert"              |
| **Beschreibung/Info** | Punkt `.`          | "Dieses Feld ist erforderlich."                  |
| **UI-Label**          | Keine              | "Datensatz speichern"                            |

**Grundregel**: Fehlermeldungen haben **immer** `!` für Dringlichkeit.

### Muster für Fehlermeldungen

**Immer** das Muster "konnte nicht + Infinitiv" verwenden:

| ✅ Korrekt                                 | ❌ Falsch                              |
| ----------------------------------------- | ------------------------------------- |
| Datensatz konnte nicht gespeichert werden | Ich konnte die Platte nicht speichern |
| Datensatz konnte nicht gelöscht werden    | Unmöglich zu löschen                  |
| Datei konnte nicht hochgeladen werden     | Fehler beim Hochladen                 |

**Niemals** "Ich konnte nicht..." oder umgangssprachliche Formulierungen verwenden.

## Glossar

```
"Add" → "Hinzufügen"
"Block" → "Block" (Plural: "Blöcke")
"Custom asset storage" → "Benutzerdefinierter Asset-Speicher"
"DatoCMS Support" → "DatoCMS-Support"
"DatoCMS-hosted assets" → "Von DatoCMS gehostete Assets"
"Delete asset collection" → "Asset-Sammlung löschen"
"direct download URL" → "Direkte Download-URL"
"dragging and dropping" → "per Drag-and-Drop"
"Editor's Preferences" → "Editor-Einstellungen"
"Environment fast-fork" → "Environment-Fast-Fork"
"Error reporter" → "Fehlerreporter"
"Field appearance plugin" → "Felddarstellungs-Plugin"
"File type" → "Dateityp"
"information" → "Informationen"
"internet connection" → "Internetverbindung"
"item" → "Datensatz"
"locales" → "Sprachen"
"Menu item" → "Menüpunkt"
"Permissions" → "Berechtigungen"
"platform" → "Plattform"
"private" → "privat"
"project" → "Projekt"
"publicly accessible" → "öffentlich zugänglich"
"Read-only mode" → "Nur-Lese-Modus"
"record" → "Datensatz"
"restricted" → "eingeschränkt"
"scheduled maintenance" → "Geplante Wartung"
"Selected" → "Ausgewählt"
"selector" → "Selektor"
"sidebar" → "Seitenleiste"
"tags" → "Tags"
"Upload endpoint" → "Upload-Endpunkt"
"User account" → "Benutzerkonto"
```
