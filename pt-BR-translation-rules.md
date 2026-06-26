# Guia de Tradução para Português Brasileiro do DatoCMS

Este guia define as regras para garantir consistência nas traduções em português brasileiro da interface do DatoCMS.

## Regras Fundamentais

- **"Você" formal** em toda a interface (nunca "tu" ou tratamento excessivamente informal)
- **Termos técnicos em inglês** (build, deploy, webhook, adapter, schema, hook, payload, sandbox)
- **Concordância verbal e nominal** adequada ao gênero e número
- **"por favor"** sempre duas palavras (nunca "porfavor")
- **Gerúndio brasileiro**: Use "está fazendo" (não "está a fazer" do português europeu)
- **Confirmações**: Use "Tem certeza" (não "Tem a certeza" do português europeu)

## Linguagem sem gênero

O português brasileiro tem flexão de gênero, mas quando um texto se dirige ao **usuário** (cujo gênero é desconhecido), evite particípios e adjetivos que exijam concordância de gênero (por exemplo "bem-vindo", "conectado", "logado", "pronto", "certo"). Prefira reformulações neutras, normalmente com formas verbais.

Observação sobre "Tem certeza": em pt-BR "certeza" é um substantivo, então "Tem certeza de que deseja…?" **não** força gênero e continua aceitável (ver Regras Fundamentais). O problema de gênero só aparece com particípios e adjetivos que concordam com o usuário. Sempre que possível, ainda assim prefira a forma verbal direta ("Deseja…?", "Quer…?").

| ✅ Neutro                            | ❌ Gênero forçado                     |
| ----------------------------------- | ------------------------------------ |
| "Boas-vindas!"                      | "Seja bem-vindo!"                    |
| "Que bom ter você por aqui!"        | "Bem-vindo!"                         |
| "Acesso realizado com sucesso!"     | "Conectado com sucesso, seja bem-vindo!" |
| "Deseja continuar?"                 | "Você está certo de que quer continuar?" |
| "Você precisa fazer login"          | "Você precisa estar logado"          |

**Estratégias**: prefira formas verbais ("Deseja…?", "Quer…?", "Você precisa…") em vez de adjetivos de estado ("Você está pronto/conectado/certo"). Para mensagens de boas-vindas, evite "Bem-vindo" e use formas neutras ("Boas-vindas", "Que bom ter você por aqui").

**IMPORTANTE**: esta regra vale **apenas** para texto que se refere ao usuário. Particípios e adjetivos que se referem a **objetos** (registro, arquivo, ambiente) mantêm a concordância de gênero normal: "registro publicado", "arquivo removido", "ambiente excluído".

## Regras de Disambiguação

### Unpublish/Unpublishing

O termo é **traduzido** para português:

| Inglês       | Português                  |
| ------------ | -------------------------- |
| Unpublish    | Despublicar                |
| Unpublishing | Despublicação              |
| Unpublished  | Despublicado/Não publicado |

### Agendamento (Schedule / Scheduling) (IMPORTANTE)

Para publicações e despublicações diferidas no tempo, use **sempre uma única família coerente**: **agendar / agendado / agendamento**. São **proibidas** as variantes concorrentes "programar / programado / programação" nesse contexto. **Nunca** traduza "scheduled" como "automática" ou "futura".

Exceção: "scheduled maintenance" continua sendo "manutenção programada", pois é um termo fixo já estabelecido fora do contexto de agendamento de registros.

| Inglês                  | ✅ Correto                     | ❌ Incorreto                    |
| ----------------------- | ----------------------------- | ------------------------------ |
| to schedule (verbo)     | agendar                       | programar                      |
| scheduled (… para)      | agendada para                 | programada para                |
| schedule (o plano)      | agendamento                   | programação                    |
| Add new schedule        | Adicionar novo agendamento    | Adicionar nova programação     |
| Scheduled publishing at | Publicação agendada para      | Publicação programada para     |
| Scheduled unpublishing at | Despublicação agendada para | Despublicação programada para  |

Um "agendamento" (a regra diferida única) cobre **tanto a publicação quanto a despublicação**: títulos genéricos não devem assumir um contexto exclusivo de publicação.

**Cancelar um agendamento**: use **sempre o mesmo verbo "cancelar"** em todos os pontos (título do diálogo, toast de sucesso e erro), para que confirmação e mensagem final usem o mesmo verbo. Exceções de espelhamento: o botão genérico "Cancelar"; "parar" quando o inglês realmente diz "stop" (por exemplo "stop automatic publication"); "automática/automaticamente".

| Inglês                                       | ✅ Correto                                       |
| -------------------------------------------- | ---------------------------------------------- |
| Cancel scheduled publication?                | Cancelar publicação agendada?                  |
| Scheduled publication successfully cancelled! | Agendamento da publicação cancelada com sucesso! |
| Couldn't cancel scheduled publication!       | Não foi possível cancelar o agendamento da publicação! |
| Yes, stop automatic publication              | Sim, parar publicação automática               |

### Estados do registro (Record states)

Os estados seguem o inglês **literalmente** (não interprete):

| Inglês                      | Português                       |
| --------------------------- | ------------------------------- |
| Published                   | Publicado                       |
| Published (unsaved changes) | Publicado (alterações não salvas) |
| Not published               | Não publicado                   |
| Unpublished changes         | Alterações não publicadas       |

**"Not published" não pode virar "Rascunho"**: a regra de manter "Rascunho" vale apenas quando o inglês realmente diz "Draft" (por exemplo "item.shortStatus.draft").

### Environment/Ambiente

O termo é **traduzido** para português:

| Inglês                | Português                 |
| --------------------- | ------------------------- |
| Current environment   | Ambiente atual            |
| Switch to environment | Mudar para o ambiente     |
| Environment settings  | Configurações de ambiente |

### Títulos de Diálogos de Confirmação

Para títulos de diálogos que pedem confirmação, usar o **infinitivo** com ponto de interrogação:

| Tipo                   | Exemplo                         |
| ---------------------- | ------------------------------- |
| Diálogo de confirmação | "Remover registro?"             |
| Diálogo de confirmação | "Cancelar publicação agendada?" |
| Diálogo de confirmação | "Despublicar registros filhos?" |

Para **botões de ação**, usar o **infinitivo** (não imperativo):

| Tipo  | Exemplo       |
| ----- | ------------- |
| Botão | "Publicar"    |
| Botão | "Remover"     |
| Botão | "Despublicar" |

### Heading vs Título

- **"Heading"** (H1-H6 em editor de texto) → **"Cabeçalho"**
- **"Title"** (campo título, título de página) → **"Título"**

| Inglês      | Português        |
| ----------- | ---------------- |
| Heading 1   | Cabeçalho 1      |
| Heading 2   | Cabeçalho 2      |
| Title field | Campo título     |
| Page title  | Título da página |

### Pontuação nas Mensagens

| Tipo de mensagem     | Pontuação               | Exemplo                               |
| -------------------- | ----------------------- | ------------------------------------- |
| **Erro/Falha**       | Ponto de exclamação `!` | "Não foi possível salvar o registro!" |
| **Sucesso com ação** | Ponto de exclamação `!` | "Registro salvo com sucesso!"         |
| **Sucesso neutro**   | Sem pontuação ou ponto  | "Registro atualizado com sucesso"     |
| **Descrição/Info**   | Ponto `.`               | "Este campo é obrigatório."           |
| **Label de UI**      | Sem pontuação           | "Salvar registro"                     |

**Regra geral**: Mensagens de erro têm **sempre** `!` para urgência. Mensagens de sucesso podem ter `!` para ênfase ou ser neutras.

### Padrão para Mensagens de Erro

Usar **sempre** o padrão "Não foi possível + infinitivo":

| ✅ Correto                 | ❌ Incorreto          |
| ------------------------- | -------------------- |
| Não foi possível salvar   | Impossível salvar    |
| Não foi possível remover  | Não posso remover    |
| Não foi possível carregar | Erro no carregamento |

### Expand/Collapse

Para ações de expansão e recolhimento de elementos de UI:

- **"Expand"** → **"Expandir"**
- **"Collapse"** → **"Recolher"**

| Inglês       | Português     |
| ------------ | ------------- |
| Expand       | Expandir      |
| Expand all   | Expandir tudo |
| Collapse     | Recolher      |
| Collapse all | Recolher tudo |

**Nunca traduzir** "collapse" como "comprimir", "fechar" ou "minimizar".

### Listas (Bulleted/Numbered)

- **Bulleted list** → **Lista de pontos** (não "Lista com marcadores")
- **Numbered list** → **Lista numérica** (não "Lista numerada")

### Delete vs Remove

- **"Delete"** (exclusão permanente) → **"Excluir"** ou **"Remover"**
- **"Remove"** (remoção de referência) → **"Remover"**

Ambos os termos são aceitáveis, mas manter consistência dentro do mesmo contexto.

## Glossário

```
"Add" → "Adicionar"
"Block" → "Bloco"
"Build trigger" → "Build trigger" (manter em inglês)
"Custom asset storage" → "Armazenamento de assets personalizado"
"DatoCMS Support" → "Suporte DatoCMS"
"DatoCMS-hosted assets" → "Assets hospedados pelo DatoCMS"
"Delete asset collection" → "Excluir coleção de assets"
"direct download URL" → "URL de download direto"
"dragging and dropping" → "arrastar e soltar"
"Editor's Preferences" → "Preferências do editor"
"Environment fast-fork" → "Fast-fork do ambiente"
"Error reporter" → "Relatório de erros"
"Facebook video" → "Vídeo do Facebook"
"Field appearance plugin" → "Plugin de aparência do campo"
"File type" → "Tipo de arquivo"
"information" → "informações"
"internet connection" → "conexão com a internet"
"item" → "registro"
"locales" → "idiomas"
"Menu item" → "Item de menu"
"Permissions" → "Permissões"
"platform" → "plataforma"
"private" → "privado"
"project" → "projeto"
"publicly accessible" → "acessível publicamente"
"Read-only mode" → "Modo somente leitura"
"restricted" → "restrito"
"scheduled maintenance" → "manutenção programada"
"Selected" → "Selecionados"
"selected" → "selecionado"
"selector" → "seletor"
"sidebar" → "barra lateral"
"tags" → "marcadores" ou "tags"
"Upload endpoint" → "Endpoint de upload"
"User account" → "Conta de usuário"
"video platform" → "plataforma de vídeo"
"video provider" → "provedor de vídeo"
"Vimeo URL" → "URL do Vimeo"
"YouTube URL" → "URL do YouTube"
```
