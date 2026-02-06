# Guia de Tradução para Português Brasileiro do DatoCMS

Este guia define as regras para garantir consistência nas traduções em português brasileiro da interface do DatoCMS.

## Regras Fundamentais

- **"Você" formal** em toda a interface (nunca "tu" ou tratamento excessivamente informal)
- **Termos técnicos em inglês** (build, deploy, webhook, adapter, schema, hook, payload, sandbox)
- **Concordância verbal e nominal** adequada ao gênero e número
- **"por favor"** sempre duas palavras (nunca "porfavor")
- **Gerúndio brasileiro**: Use "está fazendo" (não "está a fazer" do português europeu)
- **Confirmações**: Use "Tem certeza" (não "Tem a certeza" do português europeu)

## Regras de Disambiguação

### Unpublish/Unpublishing

O termo é **traduzido** para português:

| Inglês       | Português                  |
| ------------ | -------------------------- |
| Unpublish    | Despublicar                |
| Unpublishing | Despublicação              |
| Unpublished  | Despublicado/Não publicado |

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
