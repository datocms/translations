# Leitfaden für die deutsche Übersetzung von DatoCMS

Dieser Leitfaden definiert die Regeln für eine konsistente deutsche Übersetzung der DatoCMS-Oberfläche.

## Grundregeln

- **Informelles "du"** durchgehend verwenden (niemals "Sie")
- **Technische Begriffe bleiben auf Englisch** (build, build trigger, deploy, webhook, adapter, schema, hook, payload, environment)
- **"bitte"** immer klein, außer am Satzanfang

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
