# Guia de Tradução para Português Europeu do DatoCMS

Este guia define as regras para garantir consistência nas traduções em português europeu (pt-PT) da interface do DatoCMS.

## Regras Fundamentais

- **Tratamento formal impessoal** em toda a interface (evitar "você", preferir construções impessoais ou infinitivo)
- **Termos técnicos em inglês** (build, deploy, webhook, adapter, schema, hook, payload, sandbox)
- **Concordância verbal e nominal** adequada ao género e número
- **"por favor"** sempre duas palavras (nunca "porfavor")
- **Gerúndio europeu**: Use "está a fazer" (nunca "está fazendo")
- **Confirmações**: Use "Tem a certeza" (nunca "Tem certeza")
- **Grafia portuguesa**: "registo" (não "registro"), "facto" (não "fato")

## Vocabulário Padrão

| Inglês     | Português Europeu |
| ---------- | ----------------- |
| File       | Ficheiro          |
| Save       | Guardar           |
| User       | Utilizador        |
| Share      | Partilhar         |
| Shared     | Partilhado        |
| Record     | Registo           |
| Screen     | Ecrã              |
| Delete     | Eliminar / Apagar |
| Settings   | Definições        |
| Download   | Descarregar       |
| Connection | Ligação           |

## Linguagem sem género

O português é uma língua com género gramatical. Quando o texto se dirige à pessoa que utiliza a interface (cujo género é desconhecido), evitar adjetivos e particípios que exijam concordância de género. Preferir reformulações neutras assentes em formas verbais.

Estratégias:

- **Preferir formas verbais** ("Pretende…?", "Quer…?", "Deseja…?", "Tem de…") em vez de adjetivos de estado ("Está seguro?", "Está ligado?", "Está autenticado?").
- **Boas-vindas**: evitar "Bem-vindo" (masculino); usar a forma neutra "Boas-vindas".

| ✅ Neutro                                          | ❌ Com marca de género                              |
| ------------------------------------------------- | -------------------------------------------------- |
| "Tem a certeza que quer eliminar este registo?"   | "Tem a certeza de que está seguro de o eliminar?"  |
| "Boas-vindas!" / "Boas-vindas a bordo!"           | "Bem-vindo!" / "Bem-vindo a bordo!"                |
| "Deseja continuar?" / "Como deseja proceder?"     | "Está pronto para continuar?"                      |
| "Tem de iniciar sessão" / "É necessário autenticar-se" | "Tem de estar autenticado"                    |

A construção dominante na interface já é neutra ("Tem a certeza que quer…?", "Deseja continuar?"); mantê-la. As boas-vindas com género são a exceção a corrigir: ver as chaves `completeRegistration.password`, `noAuth.completeRegistration.create.success` e `noAuth.signIn.create.success`, todas com "Bem-vindo".

**IMPORTANTE**: esta regra aplica-se apenas a texto que se refere à pessoa utilizadora. Particípios e adjetivos que se referem a objetos (registo, asset, ambiente) mantêm a concordância gramatical normal com o substantivo: "Registo publicado", "Despublicação agendada", "Ambiente eliminado".

## Regras de Disambiguação

### Unpublish/Unpublishing

O termo é **traduzido** para português. Preferir "despublicar" para consistência:

| Inglês       | Português                      |
| ------------ | ------------------------------ |
| Unpublish    | Despublicar                    |
| Unpublishing | Despublicação                  |
| Unpublished  | Despublicado / Não publicado   |

### Environment/Ambiente

O termo é **traduzido** para português:

| Inglês                | Português                 |
| --------------------- | ------------------------- |
| Current environment   | Ambiente atual            |
| Switch to environment | Mudar para o ambiente     |
| Environment settings  | Definições de ambiente    |

### Títulos de Diálogos de Confirmação

Para títulos de diálogos que pedem confirmação, usar o **infinitivo** com ponto de interrogação:

| Tipo                   | Exemplo                         |
| ---------------------- | ------------------------------- |
| Diálogo de confirmação | "Eliminar registo?"             |
| Diálogo de confirmação | "Cancelar publicação agendada?" |
| Diálogo de confirmação | "Despublicar registos filhos?"  |

Para **botões de ação**, usar o **infinitivo** (não imperativo):

| Tipo  | Exemplo       |
| ----- | ------------- |
| Botão | "Publicar"    |
| Botão | "Eliminar"    |
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

| Tipo de mensagem     | Pontuação               | Exemplo                                |
| -------------------- | ----------------------- | -------------------------------------- |
| **Erro/Falha**       | Ponto de exclamação `!` | "Não foi possível guardar o registo!"  |
| **Sucesso com ação** | Ponto de exclamação `!` | "Registo guardado com sucesso!"        |
| **Sucesso neutro**   | Sem pontuação ou ponto  | "Registo atualizado com sucesso"       |
| **Descrição/Info**   | Ponto `.`               | "Este campo é obrigatório."            |
| **Label de UI**      | Sem pontuação           | "Guardar registo"                      |

**Regra geral**: Mensagens de erro têm **sempre** `!` para urgência. Mensagens de sucesso podem ter `!` para ênfase ou ser neutras.

### Padrão para Mensagens de Erro

Usar **sempre** o padrão "Não foi possível + infinitivo":

| ✅ Correto                  | ❌ Incorreto          |
| -------------------------- | -------------------- |
| Não foi possível guardar   | Impossível guardar   |
| Não foi possível eliminar  | Não posso eliminar   |
| Não foi possível carregar  | Erro no carregamento |

### Expand/Collapse

Para ações de expansão e recolhimento de elementos de UI:

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

- **"Delete"** (exclusão permanente) → **"Eliminar"** ou **"Apagar"**
- **"Remove"** (remoção de referência) → **"Remover"**

Manter consistência dentro do mesmo contexto.

### Agendamento (Schedule / Scheduling)

Para publicações e despublicações diferidas no tempo, usar **SEMPRE** uma única família coerente:

- **agendar** (verbo)
- **agendado / agendada** (adjetivo)
- **agendamento** (substantivo: "a schedule")

**PROIBIDAS** as variantes concorrentes **programar / programação / programado / programada** neste contexto. A interface mistura atualmente as duas famílias; o padrão a adotar é **agendar / agendamento / agendado**.

Exceção: a colocação fixa "scheduled maintenance" mantém-se "manutenção programada" (ver glossário). Não faz parte da funcionalidade de agendamento de registos.

Nunca traduzir "scheduled" como "automática" nem "futura". As palavras "automática" e "futura" só aparecem quando o inglês diz mesmo "automatic" (ex.: "stop automatic publication") ou "future" (ex.: "Future publication").

Um único **agendamento** abrange **tanto a publicação como a despublicação**: títulos genéricos não devem assumir um contexto exclusivo de publicação.

| Inglês                  | ✅ Correto                  | ❌ Evitar                   |
| ----------------------- | -------------------------- | -------------------------- |
| to schedule (verbo)     | Agendar                    | Programar                  |
| scheduled (adjetivo)    | Agendado / Agendada        | Programado / Programada    |
| a schedule (substantivo)| Agendamento                | Programação                |
| Add new schedule        | Adicionar novo agendamento | Adicionar nova programação |
| Scheduled publishing at | Publicação agendada em     | Publicação programada em   |
| Scheduled unpublishing at| Despublicação agendada em | Despublicação programada em|
| Publishing schedule     | Agendamento de publicação  | Programação de publicação  |

**Cancelar um agendamento**: usar o mesmo verbo, **cancelar**, no título do diálogo, no toast de sucesso e no erro, para que a confirmação e o resultado final coincidam.

| Inglês                                        | ✅ Português                                    |
| --------------------------------------------- | ---------------------------------------------- |
| Cancel scheduled publication?                 | Cancelar publicação agendada?                  |
| Scheduled publication successfully cancelled! | Agendamento da publicação cancelado com sucesso! |
| Couldn't cancel scheduled publication!        | Não foi possível cancelar a publicação agendada! |
| Yes, stop automatic publication               | Sim, parar a publicação automática             |

Exceções de espelhamento do inglês: o botão genérico "Cancel" continua "Cancelar"; "stop" traduz-se por "parar" quando o inglês diz mesmo stop; "automatic/automatically" traduz-se por "automática/automaticamente".

As chaves que ainda usam a família errada (programar/programação/programada) e que devem passar para agendar/agendamento/agendada estão listadas em "Inconsistências Atuais a Corrigir", ponto 4.

### Estados do registo (Record states)

Os estados seguem o inglês **literalmente**; não interpretar. Em particular, "Not published" **NÃO** deve tornar-se "Rascunho": a regra de manter "draft/rascunho" só se aplica quando o inglês diz mesmo "draft".

| Inglês                          | Português                                |
| ------------------------------- | ---------------------------------------- |
| Published                       | Publicado                                |
| Published (unsaved changes)     | Publicado (alterações não guardadas)     |
| Not published                   | Não publicado                            |
| Not published (unsaved changes) | Não publicado (alterações não guardadas) |
| New record                      | Novo registo                             |
| Unpublished changes             | Alterações não publicadas                |

Consistência nativa: "unsaved changes" surge traduzido de duas formas, "alterações por guardar" em `item.status.draft.dirty` e "alterações não guardadas" em `item.status.published.dirty` e `item.status.new.dirty`. Uniformizar em **"alterações não guardadas"**.

## Inconsistências Atuais a Corrigir

As seguintes inconsistências foram identificadas nas traduções atuais:

### 1. Grafia brasileira "registro" em vez de "registo"

| Chave | Atual | Correto |
| ----- | ----- | ------- |
| `editor.item.scheduleUnpublishing.success` | "Registro programado..." | "Registo programado..." |
| `form.scheduleUnpublishing.date` | "Despublicar este registro em" | "Despublicar este registo em" |
| `genericError.PUBLISHED_REFERENCES` | "...o registro, já que outros registros..." | "...o registo, já que outros registos..." |
| `messages.confirm.askForRecursiveTreeUnpublish.title` | "Despublicar os registros filhos?" | "Despublicar os registos filhos?" |
| `messages.confirm.askForRecursiveTreeUnpublish.unpublishRecursively` | "...todos os registros filhos" | "...todos os registos filhos" |
| `messages.confirm.deleteScheduledUnpublishing.question` | "Este registro já não será..." | "Este registo já não será..." |

### 2. "compartilhado" em vez de "partilhado"

| Chave | Atual | Correto |
| ----- | ----- | ------- |
| `menuItem.itemTypeFilter` | "Aplicar filtro compartilhado salvo" | "Aplicar filtro partilhado guardado" |

### 3. Uso de "Você" em vez de construção impessoal

| Chave | Atual | Correto |
| ----- | ----- | ------- |
| `tabularItemsList.row.sortingDisabled` | "Você não pode reordenar..." | "Não é possível reordenar..." |
| `versions.restore.disabledCurrentVersion` | "Você não pode reverter..." | "Não é possível reverter..." |

### 4. "programada/programação" em vez de "agendada/agendamento"

A funcionalidade de agendamento mistura duas famílias de termos para "scheduled" (ver "Agendamento (Schedule / Scheduling)"). O padrão é **agendar / agendamento / agendado**; corrigir as chaves que ainda usam programar/programação/programada. Manter "manutenção programada" apenas para "scheduled maintenance".

| Chave | Atual | Correto |
| ----- | ----- | ------- |
| `editor.item.destroyScheduledUnpublishing.success` | "Despublicação programada cancelada com sucesso!" | "Despublicação agendada cancelada com sucesso!" |
| `editor.item.scheduleUnpublishing.success` | "Registo programado para despublicação com sucesso!" | "Registo agendado para despublicação com sucesso!" |
| `form.scheduleUnpublishing.button.default` | "Programar despublicação" | "Agendar despublicação" |
| `filter.meta.unpublishing_scheduled_at` | "Despublicação programada em" | "Despublicação agendada em" |
| `itemTable.metaCol._publication_scheduled_at` | "Publicação programada em" | "Publicação agendada em" |
| `itemTable.metaCol._unpublishing_scheduled_at` | "Despublicação programada em" | "Despublicação agendada em" |
| `messages.confirm.deleteScheduledUnpublishing.title` | "Cancelar a despublicação programada?" | "Cancelar a despublicação agendada?" |
| `newSchedule.title` | "Adicionar nova programação" | "Adicionar novo agendamento" |
| `schedule.title` | "Programação de publicação" | "Agendamento de publicação" |
| `schedule.noSchedule` | "Nenhuma programação de publicação definida" | "Nenhum agendamento de publicação definido" |

## Recomendações para SaaS em Português Europeu

Para uma experiência mais natural num produto SaaS:

### Tom e Formalidade

- **Usar tratamento formal mas acessível**: Evitar "você" direto, mas não ser excessivamente formal
- **Preferir construções impessoais**: "Não é possível fazer X" em vez de "Você não pode fazer X"
- **Usar infinitivo para instruções**: "Clicar para continuar" em vez de "Clique para continuar"

### Terminologia Técnica

- **Manter termos ingleses quando universais**: build, deploy, webhook, API, token, schema
- **Traduzir termos com equivalente claro**: settings → definições, upload → carregar/upload

### Mensagens de Sistema

- **Ser conciso e direto**: Evitar verbosidade desnecessária
- **Usar voz ativa**: "O registo foi guardado" em vez de construções passivas complexas
- **Feedback claro**: "Guardado com sucesso!" é preferível a "A operação de guardar foi concluída com êxito"

### Contrações Naturais

Em português europeu, as contrações são frequentes e naturais:

| Evitar  | Preferir |
| ------- | -------- |
| "em o"  | "no"     |
| "em a"  | "na"     |
| "de o"  | "do"     |
| "a o"   | "ao"     |
| "em uma"| "numa"   |

### Labels de UI

- **Curtos e descritivos**: "Guardar" em vez de "Guardar alterações"
- **Consistentes**: Usar sempre o mesmo termo para a mesma ação
- **Sem pontuação final**: Botões e labels não levam ponto final

## Glossário

```
"Add" → "Adicionar"
"Asset" → "Asset" (manter em inglês)
"Block" → "Bloco"
"Build trigger" → "Build trigger" (manter em inglês)
"Custom asset storage" → "Armazenamento de assets personalizado"
"DatoCMS Support" → "Suporte DatoCMS"
"DatoCMS-hosted assets" → "Assets alojados pelo DatoCMS"
"Delete" → "Eliminar" ou "Apagar"
"Delete asset collection" → "Eliminar coleção de assets"
"direct download URL" → "URL de descarregamento direto"
"dragging and dropping" → "arrastar e largar"
"Editor's Preferences" → "Preferências do editor"
"Environment fast-fork" → "Fast-fork do ambiente"
"Error reporter" → "Relatório de erros"
"Facebook video" → "Vídeo do Facebook"
"Field appearance plugin" → "Plugin de aparência do campo"
"File" → "Ficheiro"
"File type" → "Tipo de ficheiro"
"information" → "informações"
"internet connection" → "ligação à internet"
"item" → "registo"
"locales" → "idiomas"
"Menu item" → "Item de menu"
"Permissions" → "Permissões"
"platform" → "plataforma"
"private" → "privado"
"project" → "projeto"
"publicly accessible" → "acessível publicamente"
"Read-only mode" → "Modo só de leitura"
"record" → "registo"
"Remove" → "Remover"
"restricted" → "restrito"
"Save" → "Guardar"
"scheduled maintenance" → "manutenção programada"
"Selected" → "Selecionados"
"selected" → "selecionado"
"selector" → "seletor"
"Settings" → "Definições"
"Share" → "Partilhar"
"Shared" → "Partilhado"
"sidebar" → "barra lateral"
"tags" → "etiquetas" ou "tags"
"Upload" → "Carregar" ou "Upload"
"Upload endpoint" → "Endpoint de upload"
"User" → "Utilizador"
"User account" → "Conta de utilizador"
"video platform" → "plataforma de vídeo"
"video provider" → "fornecedor de vídeo"
"Vimeo URL" → "URL do Vimeo"
"YouTube URL" → "URL do YouTube"
```
