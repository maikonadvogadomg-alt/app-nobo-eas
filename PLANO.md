# PLANO DO PROJETO: Python Flask

> Gerado automaticamente pelo SK Code Editor em 25/04/2026, 11:17:22
> **128 arquivo(s)** | **~20.360 linhas de codigo**

---

## RESUMO EXECUTIVO

- **Tipo de aplicacao:** Aplicacao Web Frontend (React)
- **Frontend / Stack principal:** React, TypeScript

**Para rodar o projeto:**
```bash
# Abra index.html no Preview (botao Play)
```

---

## ESTRUTURA DE ARQUIVOS

```
Python Flask/
├── api-server/
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── dist/
│   │   ├── thread-stream-worker.mjs
│   │   └── thread-stream-worker.mjs.map
│   ├── src/
│   │   ├── lib/
│   │   │   ├── .gitkeep
│   │   │   └── logger.ts
│   │   ├── middlewares/
│   │   │   └── .gitkeep
│   │   ├── routes/
│   │   │   ├── ai-proxy.ts
│   │   │   ├── health.ts
│   │   │   ├── index.ts
│   │   │   └── terminal.ts
│   │   ├── app.ts
│   │   └── index.ts
│   ├── build.mjs
│   ├── package.json
│   └── tsconfig.json
├── mobile/
│   ├── .expo/
│   │   ├── types/
│   │   │   └── router.d.ts
│   │   ├── devices.json
│   │   └── README.md
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── app/
│   │   ├── (tabs)/
│   │   │   ├── _layout.tsx
│   │   │   ├── ai.tsx
│   │   │   ├── editor.tsx
│   │   │   ├── index.tsx
│   │   │   ├── settings.tsx
│   │   │   ├── tasks.tsx
│   │   │   └── terminal.tsx
│   │   ├── _layout.tsx
│   │   └── +not-found.tsx
│   ├── components/
│   │   ├── AIChat.tsx
│   │   ├── AIMemoryModal.tsx
│   │   ├── CheckpointsModal.tsx
│   │   ├── CodeEditor.tsx
│   │   ├── ErrorBoundary.tsx
│   │   ├── ErrorFallback.tsx
│   │   ├── FileSidebar.tsx
│   │   ├── FloatingAI.tsx
│   │   ├── KeyboardAwareScrollViewCompat.tsx
│   │   ├── LibrarySearch.tsx
│   │   ├── MessageRenderer.tsx
│   │   ├── ProjectPlanModal.tsx
│   │   ├── SystemStatus.tsx
│   │   └── Terminal.tsx
│   ├── constants/
│   │   └── colors.ts
│   ├── context/
│   │   └── AppContext.tsx
│   ├── hooks/
│   │   └── useColors.ts
│   ├── scripts/
│   │   └── build.js
│   ├── server/
│   │   ├── templates/
│   │   │   └── landing-page.html
│   │   └── serve.js
│   ├── utils/
│   │   ├── projectPlan.ts
│   │   └── zipUtils.ts
│   ├── .gitignore
│   ├── app.json
│   ├── babel.config.js
│   ├── eas.json
│   ├── expo-env.d.ts
│   ├── metro.config.js
│   ├── package.json
│   └── tsconfig.json
├── mockup-sandbox/
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── src/
│   │   ├── .generated/
│   │   │   └── mockup-components.ts
│   │   ├── components/
│   │   │   └── ui/
│   │   │       ├── accordion.tsx
│   │   │       ├── alert-dialog.tsx
│   │   │       ├── alert.tsx
│   │   │       ├── aspect-ratio.tsx
│   │   │       ├── avatar.tsx
│   │   │       ├── badge.tsx
│   │   │       ├── breadcrumb.tsx
│   │   │       ├── button-group.tsx
│   │   │       ├── button.tsx
│   │   │       ├── calendar.tsx
│   │   │       ├── card.tsx
│   │   │       ├── carousel.tsx
│   │   │       ├── chart.tsx
│   │   │       ├── checkbox.tsx
│   │   │       ├── collapsible.tsx
│   │   │       ├── command.tsx
│   │   │       ├── context-menu.tsx
│   │   │       ├── dialog.tsx
│   │   │       ├── drawer.tsx
│   │   │       ├── dropdown-menu.tsx
│   │   │       ├── empty.tsx
│   │   │       ├── field.tsx
│   │   │       ├── form.tsx
│   │   │       ├── hover-card.tsx
│   │   │       ├── input-group.tsx
│   │   │       ├── input-otp.tsx
│   │   │       ├── input.tsx
│   │   │       ├── item.tsx
│   │   │       ├── kbd.tsx
│   │   │       ├── label.tsx
│   │   │       ├── menubar.tsx
│   │   │       ├── navigation-menu.tsx
│   │   │       ├── pagination.tsx
│   │   │       ├── popover.tsx
│   │   │       ├── progress.tsx
│   │   │       ├── radio-group.tsx
│   │   │       ├── resizable.tsx
│   │   │       ├── scroll-area.tsx
│   │   │       ├── select.tsx
│   │   │       ├── separator.tsx
│   │   │       ├── sheet.tsx
│   │   │       ├── sidebar.tsx
│   │   │       ├── skeleton.tsx
│   │   │       ├── slider.tsx
│   │   │       ├── sonner.tsx
│   │   │       ├── spinner.tsx
│   │   │       ├── switch.tsx
│   │   │       ├── table.tsx
│   │   │       ├── tabs.tsx
│   │   │       ├── textarea.tsx
│   │   │       ├── toast.tsx
│   │   │       ├── toaster.tsx
│   │   │       ├── toggle-group.tsx
│   │   │       ├── toggle.tsx
│   │   │       └── tooltip.tsx
│   │   ├── hooks/
│   │   │   ├── use-mobile.tsx
│   │   │   └── use-toast.ts
│   │   ├── lib/
│   │   │   └── utils.ts
│   │   ├── App.tsx
│   │   ├── index.css
│   │   └── main.tsx
│   ├── components.json
│   ├── index.html
│   ├── mockupPreviewPlugin.ts
│   ├── package.json
│   ├── tsconfig.json
│   └── vite.config.ts
└── README.md
```

---

## STACK TECNOLOGICO DETECTADO

- **Frontend:** React, TypeScript

---

## ROTAS DA API (endpoints detectados automaticamente)

```
USE    /api  (em api-server/src/app.ts)
POST   /ai/chat  (em api-server/src/routes/ai-proxy.ts)
GET    /healthz  (em api-server/src/routes/health.ts)
POST   /terminal/exec  (em api-server/src/routes/terminal.ts)
POST   /terminal/write  (em api-server/src/routes/terminal.ts)
GET    /terminal/ls  (em api-server/src/routes/terminal.ts)
DELETE /terminal/session/:sessionId  (em api-server/src/routes/terminal.ts)
```

---

## VARIAVEIS DE AMBIENTE NECESSARIAS

Crie um arquivo `.env` na raiz com estas variaveis:

```env
LOG_LEVEL=seu_valor_aqui
PATH=seu_valor_aqui
BASE_PATH=seu_valor_aqui
REPLIT_INTERNAL_APP_DOMAIN=seu_valor_aqui
REPLIT_DEV_DOMAIN=seu_valor_aqui
EXPO_PUBLIC_DOMAIN=seu_valor_aqui
REPL_ID=seu_valor_aqui
EXPO_PUBLIC_REPL_ID=seu_valor_aqui
PORT=seu_valor_aqui
```

---

## ARQUIVOS PRINCIPAIS

- `api-server/src/app.ts` — Ponto de entrada do backend
- `api-server/src/index.ts` — Ponto de entrada do backend
- `api-server/src/routes/index.ts` — Ponto de entrada do backend
- `mobile/app/(tabs)/index.tsx` — Arquivo principal
- `mockup-sandbox/index.html` — Arquivo principal
- `mockup-sandbox/src/App.tsx` — Componente raiz do frontend
- `mockup-sandbox/src/main.tsx` — Arquivo principal

---

## GUIA COMPLETO — O QUE CADA PARTE DO PROJETO FAZ

> Esta secao explica, em linguagem simples, o que e para que serve cada pasta e cada arquivo.

### 📁 Raiz do Projeto (pasta principal)
> Arquivos de configuracao e pontos de entrada ficam aqui.

**`README.md`** _(1 linha)_
Documentacao principal do projeto. Explica o que o projeto faz e como rodar.

---

### 📁 `api-server/`
> Pasta 'api-server' — agrupamento de arquivos relacionados.

**`build.mjs`** _(126 linhas)_
Arquivo MJS — parte do projeto.

**`package.json`** _(34 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(21 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `mobile/`
> Pasta 'mobile' — agrupamento de arquivos relacionados.

**`.gitignore`** _(42 linhas)_
Lista de arquivos/pastas que o Git deve IGNORAR (nao versionar). Ex: node_modules, .env

**`app.json`** _(54 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`babel.config.js`** _(7 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`eas.json`** _(55 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`expo-env.d.ts`** _(3 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`metro.config.js`** _(4 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`package.json`** _(67 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(24 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `mockup-sandbox/`
> Pasta 'mockup-sandbox' — agrupamento de arquivos relacionados.

**`components.json`** _(22 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`index.html`** _(32 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`mockupPreviewPlugin.ts`** _(181 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`package.json`** _(75 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(17 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(73 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `api-server/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(33 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `api-server/dist/`
> Codigo compilado/gerado automaticamente — NAO edite diretamente.

**`thread-stream-worker.mjs`** _(229 linhas)_
Arquivo MJS — parte do projeto.

**`thread-stream-worker.mjs.map`** _(8 linhas)_
Arquivo MAP — parte do projeto.

---

### 📁 `api-server/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`app.ts`** _(35 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(26 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `mobile/.expo/`
> Pasta '.expo' — agrupamento de arquivos relacionados.

**`README.md`** _(14 linhas)_
Documentacao principal do projeto. Explica o que o projeto faz e como rodar.

**`devices.json`** _(4 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `mobile/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(24 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `mobile/app/`
> Pasta 'app' — agrupamento de arquivos relacionados.

**`+not-found.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`_layout.tsx`** _(68 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

---

### 📁 `mobile/components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`AIChat.tsx`** _(934 linhas)_
Componente de CHAT/MENSAGENS — interface de conversa em tempo real.

**`AIMemoryModal.tsx`** _(203 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`CheckpointsModal.tsx`** _(173 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`CodeEditor.tsx`** _(337 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`ErrorBoundary.tsx`** _(55 linhas)_
Componente de ERRO — exibido quando algo da errado, com mensagem explicativa.

**`ErrorFallback.tsx`** _(279 linhas)_
Componente de ERRO — exibido quando algo da errado, com mensagem explicativa.

**`FileSidebar.tsx`** _(303 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`FloatingAI.tsx`** _(897 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`KeyboardAwareScrollViewCompat.tsx`** _(30 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`LibrarySearch.tsx`** _(327 linhas)_
Componente de BUSCA — campo e logica para filtrar/encontrar conteudo.

**`MessageRenderer.tsx`** _(265 linhas)_
Componente de CHAT/MENSAGENS — interface de conversa em tempo real.

**`ProjectPlanModal.tsx`** _(369 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`SystemStatus.tsx`** _(327 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Terminal.tsx`** _(995 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `mobile/constants/`
> Pasta 'constants' — agrupamento de arquivos relacionados.

**`colors.ts`** _(98 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `mobile/context/`
> Gerenciamento de estado global — dados compartilhados entre telas.

**`AppContext.tsx`** _(1067 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

---

### 📁 `mobile/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`useColors.ts`** _(25 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'colors'.

---

### 📁 `mobile/scripts/`
> Pasta 'scripts' — agrupamento de arquivos relacionados.

**`build.js`** _(574 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `mobile/server/`
> Pasta 'server' — agrupamento de arquivos relacionados.

**`serve.js`** _(136 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `mobile/utils/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`projectPlan.ts`** _(208 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`zipUtils.ts`** _(166 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `mockup-sandbox/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(18 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `mockup-sandbox/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(147 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(158 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `api-server/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`.gitkeep`** _(1 linha)_
Arquivo GITKEEP — parte do projeto.

**`logger.ts`** _(21 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `api-server/src/middlewares/`
> Pasta 'middlewares' — agrupamento de arquivos relacionados.

**`.gitkeep`** _(1 linha)_
Arquivo GITKEEP — parte do projeto.

---

### 📁 `api-server/src/routes/`
> Definicao das URLs e navegacao do app.

**`ai-proxy.ts`** _(87 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`health.ts`** _(12 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(13 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`terminal.ts`** _(145 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `mobile/.expo/types/`
> Definicoes de tipos TypeScript — contratos de dados.

**`router.d.ts`** _(15 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

---

### 📁 `mobile/app/(tabs)/`
> Pasta '(tabs)' — agrupamento de arquivos relacionados.

**`_layout.tsx`** _(96 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

**`ai.tsx`** _(50 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`editor.tsx`** _(478 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`index.tsx`** _(1844 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

**`settings.tsx`** _(1125 linhas)_
Componente de CONFIGURACOES — tela onde o usuario ajusta preferencias do app.

**`tasks.tsx`** _(522 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`terminal.tsx`** _(54 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `mobile/server/templates/`
> Pasta 'templates' — agrupamento de arquivos relacionados.

**`landing-page.html`** _(461 linhas)_
Arquivo HTML — parte do projeto.

---

### 📁 `mockup-sandbox/src/.generated/`
> Pasta '.generated' — agrupamento de arquivos relacionados.

**`mockup-components.ts`** _(6 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `mockup-sandbox/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(190 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `mockup-sandbox/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `mockup-sandbox/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(56 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(51 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(38 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button-group.tsx`** _(84 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`button.tsx`** _(59 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(214 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(77 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(366 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(154 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(121 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(117 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(202 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`empty.tsx`** _(105 linhas)_
Componente de ESTADO VAZIO — exibido quando nao ha dados para mostrar (ex: 'Nenhum resultado encontrado').

**`field.tsx`** _(245 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`form.tsx`** _(177 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(28 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-group.tsx`** _(166 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(23 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`item.tsx`** _(194 linhas)_
Componente de ITEM — representa um elemento individual dentro de uma lista ou colecao.

**`kbd.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`label.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(255 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(160 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(715 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sonner.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`spinner.tsx`** _(17 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(121 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

## CONTEXTO PARA IA (copie e cole para continuar o projeto)

> Use este bloco para explicar o projeto para qualquer IA ou desenvolvedor:

```
Projeto: Python Flask
Tipo: Aplicacao Web Frontend (React)
Stack: React, TypeScript
Arquivos: 128 | Linhas: ~20.360
Rotas API: 7 endpoint(s) detectado(s)
Variaveis de ambiente necessarias: LOG_LEVEL, PATH, BASE_PATH, REPLIT_INTERNAL_APP_DOMAIN, REPLIT_DEV_DOMAIN, EXPO_PUBLIC_DOMAIN, REPL_ID, EXPO_PUBLIC_REPL_ID, PORT

Estrutura principal:
  README.md
  api-server/.replit-artifact/artifact.toml
  api-server/build.mjs
  api-server/dist/thread-stream-worker.mjs
  api-server/dist/thread-stream-worker.mjs.map
  api-server/package.json
  api-server/src/app.ts
  api-server/src/index.ts
  api-server/src/lib/.gitkeep
  api-server/src/lib/logger.ts
  api-server/src/middlewares/.gitkeep
  api-server/src/routes/ai-proxy.ts
  api-server/src/routes/health.ts
  api-server/src/routes/index.ts
  api-server/src/routes/terminal.ts
  api-server/tsconfig.json
  mobile/.expo/README.md
  mobile/.expo/devices.json
  mobile/.expo/types/router.d.ts
  mobile/.gitignore
  mobile/.replit-artifact/artifact.toml
  mobile/app.json
  mobile/app/(tabs)/_layout.tsx
  mobile/app/(tabs)/ai.tsx
  mobile/app/(tabs)/editor.tsx
  mobile/app/(tabs)/index.tsx
  mobile/app/(tabs)/settings.tsx
  mobile/app/(tabs)/tasks.tsx
  mobile/app/(tabs)/terminal.tsx
  mobile/app/+not-found.tsx
  mobile/app/_layout.tsx
  mobile/babel.config.js
  mobile/components/AIChat.tsx
  mobile/components/AIMemoryModal.tsx
  mobile/components/CheckpointsModal.tsx
  mobile/components/CodeEditor.tsx
  mobile/components/ErrorBoundary.tsx
  mobile/components/ErrorFallback.tsx
  mobile/components/FileSidebar.tsx
  mobile/components/FloatingAI.tsx
  mobile/components/KeyboardAwareScrollViewCompat.tsx
  mobile/components/LibrarySearch.tsx
  mobile/components/MessageRenderer.tsx
  mobile/components/ProjectPlanModal.tsx
  mobile/components/SystemStatus.tsx
  mobile/components/Terminal.tsx
  mobile/constants/colors.ts
  mobile/context/AppContext.tsx
  mobile/eas.json
  mobile/expo-env.d.ts
  mobile/hooks/useColors.ts
  mobile/metro.config.js
  mobile/package.json
  mobile/scripts/build.js
  mobile/server/serve.js
  mobile/server/templates/landing-page.html
  mobile/tsconfig.json
  mobile/utils/projectPlan.ts
  mobile/utils/zipUtils.ts
  mockup-sandbox/.replit-artifact/artifact.toml
  mockup-sandbox/components.json
  mockup-sandbox/index.html
  mockup-sandbox/mockupPreviewPlugin.ts
  mockup-sandbox/package.json
  mockup-sandbox/src/.generated/mockup-components.ts
  mockup-sandbox/src/App.tsx
  mockup-sandbox/src/components/ui/accordion.tsx
  mockup-sandbox/src/components/ui/alert-dialog.tsx
  mockup-sandbox/src/components/ui/alert.tsx
  mockup-sandbox/src/components/ui/aspect-ratio.tsx
  mockup-sandbox/src/components/ui/avatar.tsx
  mockup-sandbox/src/components/ui/badge.tsx
  mockup-sandbox/src/components/ui/breadcrumb.tsx
  mockup-sandbox/src/components/ui/button-group.tsx
  mockup-sandbox/src/components/ui/button.tsx
  mockup-sandbox/src/components/ui/calendar.tsx
  mockup-sandbox/src/components/ui/card.tsx
  mockup-sandbox/src/components/ui/carousel.tsx
  mockup-sandbox/src/components/ui/chart.tsx
  mockup-sandbox/src/components/ui/checkbox.tsx
  mockup-sandbox/src/components/ui/collapsible.tsx
  mockup-sandbox/src/components/ui/command.tsx
  mockup-sandbox/src/components/ui/context-menu.tsx
  mockup-sandbox/src/components/ui/dialog.tsx
  mockup-sandbox/src/components/ui/drawer.tsx
  mockup-sandbox/src/components/ui/dropdown-menu.tsx
  mockup-sandbox/src/components/ui/empty.tsx
  mockup-sandbox/src/components/ui/field.tsx
  mockup-sandbox/src/components/ui/form.tsx
  mockup-sandbox/src/components/ui/hover-card.tsx
  mockup-sandbox/src/components/ui/input-group.tsx
  mockup-sandbox/src/components/ui/input-otp.tsx
  mockup-sandbox/src/components/ui/input.tsx
  mockup-sandbox/src/components/ui/item.tsx
  mockup-sandbox/src/components/ui/kbd.tsx
  mockup-sandbox/src/components/ui/label.tsx
  mockup-sandbox/src/components/ui/menubar.tsx
  mockup-sandbox/src/components/ui/navigation-menu.tsx
  mockup-sandbox/src/components/ui/pagination.tsx
  mockup-sandbox/src/components/ui/popover.tsx
  mockup-sandbox/src/components/ui/progress.tsx
  mockup-sandbox/src/components/ui/radio-group.tsx
  mockup-sandbox/src/components/ui/resizable.tsx
  mockup-sandbox/src/components/ui/scroll-area.tsx
  mockup-sandbox/src/components/ui/select.tsx
  mockup-sandbox/src/components/ui/separator.tsx
  mockup-sandbox/src/components/ui/sheet.tsx
  mockup-sandbox/src/components/ui/sidebar.tsx
  mockup-sandbox/src/components/ui/skeleton.tsx
  mockup-sandbox/src/components/ui/slider.tsx
  mockup-sandbox/src/components/ui/sonner.tsx
  mockup-sandbox/src/components/ui/spinner.tsx
  mockup-sandbox/src/components/ui/switch.tsx
  mockup-sandbox/src/components/ui/table.tsx
  mockup-sandbox/src/components/ui/tabs.tsx
  mockup-sandbox/src/components/ui/textarea.tsx
  mockup-sandbox/src/components/ui/toast.tsx
  mockup-sandbox/src/components/ui/toaster.tsx
  mockup-sandbox/src/components/ui/toggle-group.tsx
  mockup-sandbox/src/components/ui/toggle.tsx
  mockup-sandbox/src/components/ui/tooltip.tsx
  mockup-sandbox/src/hooks/use-mobile.tsx
  mockup-sandbox/src/hooks/use-toast.ts
  mockup-sandbox/src/index.css
  mockup-sandbox/src/lib/utils.ts
  mockup-sandbox/src/main.tsx
  mockup-sandbox/tsconfig.json
  mockup-sandbox/vite.config.ts
```

---

*Plano gerado pelo SK Code Editor — 25/04/2026, 11:17:22*