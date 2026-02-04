# Průvodce českým překladem DatoCMS

Tento průvodce definuje pravidla pro zajištění konzistentních českých překladů rozhraní DatoCMS.

## Základní pravidla

- **Neformální tykání** v celém rozhraní (nikdy „vy" nebo vykání)
- **Technické pojmy zůstávají v angličtině** (build, deploy, webhook, adapter, schema, hook, payload, API, URL, SEO)
- **„prosím"** vždy malými písmeny, pokud není na začátku věty

## Pravidla pro disambiguaci

### Record/Item → Položka (DŮLEŽITÉ)

Anglické „record" nebo „item" se **vždy** překládá jako **„položka"**:

| ✅ Správně                      | ❌ Špatně                    |
| ------------------------------ | --------------------------- |
| Položka byla úspěšně vytvořena | Záznam byl úspěšně vytvořen |
| Nepodařilo se smazat položku   | Nepodařilo se smazat záznam |
| Nová položka                   | Nový záznam                 |
| Uložit položku                 | Uložit záznam               |

**Nikdy** nepoužívejte „záznam", „zápis" nebo „rekord" jako překlad pro „record".

### Asset → Médium (DŮLEŽITÉ)

Anglické „asset" se **vždy** překládá jako **„médium"** (množné číslo: **„média"**):

| ✅ Správně              | ❌ Špatně                |
| ---------------------- | ----------------------- |
| Nahrát médium          | Nahrát asset            |
| 3 média vybrána        | 3 assety vybrány        |
| Vlastní úložiště médií | Vlastní úložiště assetů |
| Knihovna médií         | Knihovna assetů         |

**Rod**: Střední → „toto médium", „tato média", „bez média"

**Nikdy** nepoužívejte „asset" v českém rozhraní.

### Publish/Unpublish (DŮLEŽITÉ)

Pro publikování a odpublikování používejte tyto konzistentní tvary:

- **„Publish"** → **„publikovat"** (sloveso) / **„publikace"** (podstatné jméno)
- **„Unpublish"** → **„odpublikovat"** (sloveso) / **„odpublikování"** (podstatné jméno)

| ✅ Správně                     | ❌ Špatně                       |
| ----------------------------- | ------------------------------ |
| Položka úspěšně publikována   | Položka úspěšně vypublikována  |
| Položka úspěšně odpublikována | Položka úspěšně odepublikována |
| Naplánovaná publikace         | Naplánované publikování        |
| Zrušit odpublikování          | Zrušit de-publikaci            |

**Nikdy** nepoužívejte „vypublikovat" pro publish — používejte pouze „publikovat".

### Expand/Collapse (DŮLEŽITÉ)

Pro rozbalování a sbalování UI prvků:

- **„Expand"** → **„Rozbalit"** (imperativ) / **„rozbalit"** (infinitiv)
- **„Collapse"** → **„Sbalit"** (imperativ) / **„sbalit"** (infinitiv)

| Anglicky     | Česky (imperativ) | Česky (infinitiv) |
| ------------ | ----------------- | ----------------- |
| Expand       | Rozbal            | rozbalit          |
| Expand all   | Rozbalit vše      | rozbalit vše      |
| Collapse     | Sbal              | sbalit            |
| Collapse all | Sbalit vše        | sbalit vše        |

**Nikdy** nepoužívejte „rozvinout/svinout" nebo „otevřít/zavřít" pro tyto akce.

### Block (množné číslo)

Množné číslo slova „block" je v češtině **„bloky"**:

| ✅ Správně                 | ❌ Špatně                   |
| ------------------------- | -------------------------- |
| Sbalit všechny bloky      | Sbalit všechny blocky      |
| 3 z 5 bloků vybráno       | 3 z 5 blocks vybráno       |
| Bloky úspěšně zkopírovány | Blocks úspěšně zkopírovány |

### Environment/Prostředí

Pojem **„environment"** se překládá jako **„prostředí"**:

| Anglicky              | Česky                 |
| --------------------- | --------------------- |
| Sandbox environment   | Sandbox prostředí     |
| Primary environment   | Primární prostředí    |
| All environments      | Všechna prostředí     |
| Environment settings  | Nastavení prostředí   |
| Switch to environment | Přepnout na prostředí |

**Rod**: Střední → „toto prostředí", „tato prostředí", „v tomto prostředí"

### Nadpisy (Headings)

- **„Heading"** (H1-H6 v textovém editoru) → **„Nadpis"**
- **„Title"** (pole názvu, název stránky) → **„Název"** nebo **„Titulek"**

| Anglicky    | Česky         |
| ----------- | ------------- |
| Heading 1   | Nadpis 1      |
| Heading 2   | Nadpis 2      |
| Title field | Pole názvu    |
| Page title  | Název stránky |

### Seznamy (Bulleted/Numbered)

- **Bulleted list** → **Odrážkový seznam** (nebo „Nečíslovaný seznam")
- **Numbered list** → **Číslovaný seznam**

### Titulky potvrzovacích dialogů

Pro titulky dialogů žádajících o potvrzení použijte **infinitiv** s otazníkem:

| Typ                | Příklad                 |
| ------------------ | ----------------------- |
| Potvrzovací dialog | „Smazat tuto položku?"  |
| Potvrzovací dialog | „Obnovit tuto verzi?"   |
| Potvrzovací dialog | „Odpublikovat položku?" |

Pro **akční tlačítka** použijte **imperativ**:

| Typ      | Příklad        |
| -------- | -------------- |
| Tlačítko | „Smazat"       |
| Tlačítko | „Obnovit"      |
| Tlačítko | „Odpublikovat" |

### Interpunkce ve zprávách

| Typ zprávy           | Interpunkce      | Příklad                         |
| -------------------- | ---------------- | ------------------------------- |
| **Chyba/Selhání**    | Vykřičník `!`    | „Nepodařilo se uložit položku!" |
| **Úspěch s akcí**    | Vykřičník `!`    | „Položka úspěšně uložena!"      |
| **Neutrální úspěch** | Žádná nebo tečka | „Položka úspěšně uložena"       |
| **Popis/Info**       | Tečka `.`        | „Toto pole je povinné."         |
| **UI label**         | Žádná            | „Uložit položku"                |

**Obecné pravidlo**: Chybové zprávy mají **vždy** `!` pro naléhavost.

### Vzor pro chybové zprávy

**Vždy** používejte vzor „Nepodařilo se + infinitiv":

| ✅ Správně            | ❌ Špatně            |
| -------------------- | ------------------- |
| Nepodařilo se uložit | Nelze uložit        |
| Nepodařilo se smazat | Nemohu smazat       |
| Nepodařilo se nahrát | Chyba při nahrávání |

## Co by bylo přirozenější v českém SaaS produktu

### Obecné doporučení pro přirozenější češtinu

1. **Kratší a přímější formulace**: České SaaS produkty často upřednostňují stručnost
   - Místo „Položka byla úspěšně vytvořena" → „Položka vytvořena"
   - Místo „Nepodařilo se uložit položku!" → „Uložení selhalo!"

2. **Moderní technický slovník**: Čeští uživatelé SaaS jsou zvyklí na anglicismy
   - „deployment" místo „nasazení" je běžně akceptováno
   - „sandbox" zůstává v angličtině (nesnaží se překládat jako „pískoviště")

3. **Konzistentní forma oslovení**: Tykání je správné pro moderní SaaS, ale mělo by být konzistentní
   - Všechny zprávy by měly používat 2. osobu jednotného čísla

4. **Přirozené české fráze pro akce**:
   - „Publikovat" je vhodnější než „Vypublikovat" (prefix „vy-" je nadbytečný)
   - „Smazat" je přirozenější než „Odstranit" pro destruktivní akce
   - „Zrušit" je vhodnější než „Stornovat" pro cancel

5. **Stavové zprávy by měly být stručné**:
   - „Publikováno" místo „Položka byla publikována"
   - „Uloženo" místo „Změny byly uloženy"

6. **Chybové zprávy by měly být jasné a akční**:
   - Vysvětlit, co se stalo
   - Navrhnout, co může uživatel udělat

## Glosář

```
"Add" → "Přidat"
"Asset" → "Médium" (množné číslo: "Média")
"Block" → "Blok" (množné číslo: "Bloky")
"Cancel" → "Zrušit"
"Collection" → "Kolekce" nebo "Sbírka"
"Create" → "Vytvořit"
"Creator" → "Autor"
"Custom asset storage" → "Vlastní úložiště médií"
"DatoCMS Support" → "Podpora DatoCMS"
"Delete" → "Smazat"
"Deploy" → "Deploy" (zůstává v angličtině)
"Dragging and dropping" → "Přetažením"
"Duplicate" → "Duplikovat"
"Edit" → "Upravit"
"Editor's Preferences" → "Předvolby editoru"
"Environment" → "Prostředí"
"Environment fast-fork" → "Fast-fork prostředí"
"Error reporter" → "Hlášení chyb"
"Field" → "Pole"
"File type" → "Typ souboru"
"Filter" → "Filtr"
"Information" → "Informace"
"Internet connection" → "Připojení k internetu"
"Item" → "Položka"
"Locales" → "Jazyky" nebo "Lokalizace"
"Media Area" → "Knihovna médií"
"Menu item" → "Položka menu"
"Model" → "Model"
"Permissions" → "Oprávnění"
"Platform" → "Platforma"
"Plugin" → "Plugin"
"Private" → "Soukromý"
"Project" → "Projekt"
"Publicly accessible" → "Veřejně přístupný"
"Publish" → "Publikovat"
"Read-only mode" → "Režim pouze pro čtení"
"Record" → "Položka"
"Remove" → "Odebrat"
"Restricted" → "Omezený"
"Save" → "Uložit"
"Scheduled maintenance" → "Plánovaná údržba"
"Selected" → "Vybráno"
"Selector" → "Selektor"
"Settings" → "Nastavení"
"Sidebar" → "Postranní panel"
"Tags" → "Tagy" nebo "Štítky"
"Unpublish" → "Odpublikovat"
"Update" → "Aktualizovat"
"Upload" → "Nahrát"
"Upload endpoint" → "Endpoint pro nahrávání"
"User account" → "Uživatelský účet"
"Webhook" → "Webhook" (zůstává v angličtině)
```