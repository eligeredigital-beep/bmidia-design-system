# BMidia Digitais — Design System + Skill para IA

Identidade visual completa da **BMidia Digitais**, a agência de tráfego pago para confeitarias, empacotada para funcionar dentro da sua IA: **Claude, ChatGPT, Gemini, Cursor, Copilot e outras**. Com ela instalada, qualquer pessoa da equipe pede "faz um carrossel da BMidia sobre…" ou "monta o resumo da reunião com o cliente X" e a IA já entrega na paleta, nas fontes e com os logos oficiais, sem precisar explicar a marca toda vez.

> **Nome da marca: BMidia, sem S.** Handle: `@BMIDIADIGITAIS`. Assinatura: *A revolução do tráfego pago na confeitaria!*

---

## ⬇️ Downloads

| Arquivo | Para quem | Link |
|---|---|---|
| **Skill completa** | Claude (app e Claude Code), ChatGPT Business/Enterprise | **[bmidia-design-system.zip](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-design-system.zip)** |
| **Skill leve** (sem fontes) | Gemini, ou se a skill completa der erro de upload | **[bmidia-skill-leve.zip](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-skill-leve.zip)** |
| **Pacote para outras IAs** | ChatGPT Free/Plus/Pro (Projetos e GPTs), Gems e qualquer IA sem skills | **[bmidia-pacote-outras-ias.zip](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-pacote-outras-ias.zip)** |
| **Projeto completo** | Tudo: skill, logos, ícones, fontes, tokens, componentes e documentação | **[Baixar o repositório inteiro](https://github.com/eligeredigital-beep/bmidia-design-system/archive/refs/heads/main.zip)** |

Arquivos soltos: [Logos](bmidia-design-system/assets/Logos) · [Ícone "bm"](bmidia-design-system/assets/Icone) · [Arcos e patterns](bmidia-design-system/assets/Elementos) · [Fontes](bmidia-design-system/fonts) · [Instruções para colar](outras-ias/instrucoes-para-colar.md)

> 🔒 **O repositório é privado.** Os links só funcionam para quem foi convidado e está logado no GitHub. Peça acesso ao Riziel.
>
> **Outra forma de baixar tudo:** no topo desta página, clique no botão verde **`<> Code` → Download ZIP**.
>
> **Baixar um arquivo só:** abra o arquivo aqui no GitHub e clique no ícone de download (**⤓ Download raw file**) no canto superior direito.

---

## 🧭 Qual é o meu caso?

| Eu uso… | Baixe | Vá para |
|---|---|---|
| **Claude** (site, app ou celular) | Skill completa | [Claude](#claude-claudeai-app-desktop-e-celular) |
| **Claude Code** | Repositório | [Claude Code](#claude-code) |
| **ChatGPT Business, Enterprise, Edu** | Skill completa | [ChatGPT com Skills](#chatgpt--planos-business-enterprise-edu-e-healthcare-skills) |
| **ChatGPT Free, Plus ou Pro** | Pacote para outras IAs | [ChatGPT Projetos](#chatgpt--free-plus-e-pro-projetos) ou [GPT personalizado](#chatgpt--gpt-personalizado-plus-ou-superior) |
| **Gemini** (conta pessoal Google) | Skill leve | [Gemini Skills](#gemini--skills-contas-pessoais) |
| **Gemini** (conta de empresa/escola) | Pacote para outras IAs | [Gemini Gems](#gemini--gems-contas-workspace) |
| **Cursor** | Repositório | [Cursor](#cursor) |
| **GitHub Copilot** (VS Code / CLI) | Repositório | [Copilot](#github-copilot) |
| **Codex (OpenAI CLI)** | Repositório | [Codex](#codex-cli) |
| **Outra IA** (Perplexity, Grok, DeepSeek…) | Pacote para outras IAs | [Qualquer outra IA](#qualquer-outra-ia) |

---

## O que é esta skill

Uma **skill** é uma pasta com um arquivo `SKILL.md` (instruções) e os arquivos de apoio (logos, fontes, tokens). A IA lê a skill **automaticamente** sempre que o pedido tem a ver com ela, no caso, qualquer peça da BMidia. Você não precisa chamá-la pelo nome. O formato é aberto e hoje funciona no Claude, ChatGPT, Gemini, Cursor, Copilot e Codex.

Ela ensina à IA:

- **Conceito e voz:** propósito, atributos, manifesto, assinatura, "números primeiro", títulos em dois tons.
- **Cores:** a paleta oficial do guia de marca (Studio Sagi) e as complementares, com os pares de contraste aprovados.
- **Tipografia:** Nearo Rounded + Montserrat para a marca; HK Grotesk, Helvetica e Montserrat nas redes; escalas para carrossel 1080×1350, apresentações e PDF A4.
- **Logo e ícone:** qual versão usar em cada fundo, respiro e o que nunca fazer.
- **Elementos:** arcos, patterns, layouts de carrossel, faixa de métrica, pill de CTA.
- **Componente Resumo de reunião (PDF A4):** cabeçalho, números, metas, tópicos, alertas e colunas de ações.

Nas IAs que não aceitam skills, o **pacote para outras IAs** traz as mesmas regras em um texto pronto para colar (`instrucoes-para-colar.md`) e 17 arquivos para anexar (logos, ícones e arcos em PNG, `tokens.json` e o guia da marca).

---

## Como instalar em cada IA

### Claude (claude.ai, app desktop e celular)

1. Baixe a **[skill completa](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-design-system.zip)**. Não descompacte.
2. Confirme que **execução de código** está ligada em **Configurações → Capacidades** (Free, Pro, Max e Ultra; no Team já vem ligada).
3. Vá em **Personalizar (Customize) → Skills**.
4. Clique em **+** → **Criar skill** → **Enviar uma skill (Upload a skill)** e selecione o `.zip`.
5. A skill **bmidia-design-system** aparece na lista; deixe o botão ativado.

> Team/Enterprise: o dono da organização pode ter desativado skills criadas por usuários. Guia oficial: [Usar skills no Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

### Claude Code

```bash
git clone https://github.com/eligeredigital-beep/bmidia-design-system.git
mkdir -p ~/.claude/skills
cp -r bmidia-design-system/bmidia-design-system ~/.claude/skills/
```

No Windows (PowerShell):

```powershell
git clone https://github.com/eligeredigital-beep/bmidia-design-system.git
New-Item -ItemType Directory -Force "$HOME\.claude\skills" | Out-Null
Copy-Item -Recurse bmidia-design-system\bmidia-design-system "$HOME\.claude\skills\"
```

Só para um projeto: copie a pasta para `.claude/skills/` dentro do projeto.

### ChatGPT — planos Business, Enterprise, Edu e Healthcare (Skills)

1. Baixe a **[skill completa](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-design-system.zip)**.
2. No ChatGPT, na barra lateral, clique em **Plugins**.
3. No topo, troque a chave de **Plugins** para **Skills**.
4. Clique em **+** ao lado da busca → **Enviar do computador (Upload from your computer)** e escolha o `.zip`.
5. A skill aparece em **Instaladas** ou **Criadas por mim**.

> Se der erro no upload, tente a **[skill leve](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-skill-leve.zip)**. Se a aba **Skills** não aparecer, o administrador do workspace precisa liberar em **Permissões e funções**. Planos Free, Plus e Pro ainda não têm Skills: use os Projetos abaixo.

### ChatGPT — Free, Plus e Pro (Projetos)

Funciona em qualquer plano. Tudo o que você conversar dentro do projeto segue a marca.

1. Baixe e **descompacte** o **[pacote para outras IAs](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-pacote-outras-ias.zip)**.
2. No ChatGPT, na barra lateral, clique em **Novo projeto** e dê o nome **BMidia**.
3. Dentro do projeto, abra **Instruções** (ou o menu **⋯ → Configurações do projeto**), cole todo o conteúdo de `instrucoes-para-colar.md` e salve.
4. Clique em **Adicionar arquivos** e envie os arquivos da pasta `arquivos-para-anexar`. Se o seu plano tiver limite menor de arquivos, priorize `guia-da-marca.md`, `tokens.json` e os 5 logos.
5. Sempre abra as conversas da BMidia **dentro desse projeto**.

### ChatGPT — GPT personalizado (Plus ou superior)

Bom para compartilhar com a equipe por link.

1. Baixe e **descompacte** o **[pacote para outras IAs](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-pacote-outras-ias.zip)**.
2. No ChatGPT, vá em **GPTs → Criar** e abra a aba **Configurar**.
3. **Nome:** BMidia Design. **Descrição:** Cria peças na identidade da BMidia Digitais.
4. **Instruções:** cole todo o conteúdo de `instrucoes-para-colar.md`.
5. **Conhecimento:** envie os 17 arquivos de `arquivos-para-anexar` (cabe no limite de 20).
6. Em **Recursos**, ative **Interpretador de código** e **Geração de imagens**.
7. Clique em **Criar** e escolha **Qualquer pessoa com o link**. Envie o link para a equipe.

### Gemini — Skills (contas pessoais)

Desde setembro de 2026 o Gemini tem skills, e em novembro de 2026 elas substituem os Gems nas contas pessoais. Não precisa de assinatura.

1. Baixe a **[skill leve](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-skill-leve.zip)**. Não descompacte.
2. Em [gemini.google.com](https://gemini.google.com), abra **Configurações → Skills**.
3. Clique em **Enviar (Upload)** e selecione o `.zip`.
4. Ative a skill. Para usar, basta mencionar a BMidia no pedido ou digitar `/bmidia-design-system` no chat.

> Faça o envio pelo site (no celular e no app de Mac, skills com arquivos não podem ser editadas). Conta de empresa/escola ainda não tem skills: use os Gems abaixo.

### Gemini — Gems (contas Workspace)

1. Baixe e **descompacte** o **[pacote para outras IAs](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-pacote-outras-ias.zip)**.
2. Em [gemini.google.com](https://gemini.google.com), abra a barra lateral → **Gems** → **Novo Gem**.
3. **Nome:** BMidia Design. **Instruções:** cole todo o conteúdo de `instrucoes-para-colar.md`.
4. Em **Conhecimento**, clique em **Adicionar arquivos** e envie os arquivos de `arquivos-para-anexar`.
5. Clique em **Salvar**.

> Os Gems de contas Workspace business serão convertidos em skills em março de 2027; nesse momento, use a skill leve.

### Cursor

```bash
git clone https://github.com/eligeredigital-beep/bmidia-design-system.git
mkdir -p ~/.cursor/skills
cp -r bmidia-design-system/bmidia-design-system ~/.cursor/skills/
```

Windows: copie a pasta `bmidia-design-system` para `C:\Users\SEU_USUARIO\.cursor\skills\`. Só para um projeto: `.cursor/skills/` dentro do projeto. Confira em **Customize → Skills**. O Cursor também lê skills de `~/.claude/skills/`; se você já instalou para o Claude Code, ele aparece sozinho.

### GitHub Copilot

Pessoal (todos os projetos): copie a pasta para `~/.copilot/skills/`. Por projeto: copie para `.github/skills/` dentro do repositório.

```bash
git clone https://github.com/eligeredigital-beep/bmidia-design-system.git
mkdir -p ~/.copilot/skills
cp -r bmidia-design-system/bmidia-design-system ~/.copilot/skills/
```

### Codex CLI

```bash
git clone https://github.com/eligeredigital-beep/bmidia-design-system.git
mkdir -p ~/.codex/skills
cp -r bmidia-design-system/bmidia-design-system ~/.codex/skills/
```

Windows: `%USERPROFILE%\.codex\skills\bmidia-design-system`.

### Qualquer outra IA

Perplexity (Spaces), Grok, DeepSeek, Copilot da Microsoft e outras:

1. Baixe e descompacte o **[pacote para outras IAs](https://github.com/eligeredigital-beep/bmidia-design-system/raw/main/dist/bmidia-pacote-outras-ias.zip)**.
2. Se a IA tiver **instruções personalizadas, espaço ou projeto**, cole lá o `instrucoes-para-colar.md` e anexe os arquivos.
3. Se não tiver, no começo de cada conversa cole o texto de `instrucoes-para-colar.md` e anexe pelo menos `guia-da-marca.md` e o logo que for usar.

### Atualizar para a versão mais nova

Baixe o arquivo de novo pelo link da sua IA, apague a versão antiga e envie a nova. Em quem usa pasta (Claude Code, Cursor, Copilot, Codex), rode `git pull` e copie a pasta outra vez.

---

## Como usar

Não precisa chamar a skill pelo nome: basta mencionar a **BMidia** no pedido. Exemplos para copiar:

| Quero… | Peça assim |
|---|---|
| Carrossel de Instagram | *"Cria um carrossel da BMidia de 6 slides sobre por que confeitaria precisa de tráfego pago no Natal."* |
| Resumo de reunião em PDF | *"Monta o resumo da reunião de hoje com a Doce Ateliê no padrão BMidia"* + cole suas anotações |
| Apresentação | *"Faz uma apresentação institucional da BMidia para prospecção de confeitarias."* |
| Post de case | *"Post de case no estilo BMidia: cliente faturou R$ 30 mil/mês com tráfego pago."* |
| Tirar dúvida da marca | *"Quais cores e fontes eu uso num story da BMidia?"* |

A IA aplica a paleta, as fontes, o logo certo para cada fundo, o handle `@BMIDIADIGITAIS` no rodapé e confere o checklist da marca antes de entregar.

**Dica:** se o resultado sair fora do padrão, diga *"siga o design system da BMidia"* que ela relê as regras.

### Usando os arquivos sem IA

- **Canva / Figma / Illustrator:** importe os logos de `assets/Logos`, os ícones e elementos (SVG) e instale as fontes da pasta `fonts/` (dois cliques no arquivo → Instalar).
- **Web / HTML:** linke o `tokens.css` (mantendo a pasta `fonts/` ao lado) e use as variáveis: `background: var(--brown); color: var(--cream); font-family: var(--font-marca);`
- **Ver os componentes:** abra `componentes/ResumoPDF/preview.html` ou `componentes/Cover/preview.html` no navegador.

---

## O que tem no projeto

```
bmidia-design-system/          ← a skill (esta pasta é o que se instala)
├── SKILL.md                   ← instruções que a IA segue
├── tokens.css                 ← @font-face + variáveis CSS + classes de tipografia
├── tokens.json                ← os mesmos tokens, com regras de uso e contraste
├── assets/
│   ├── Logos/                 ← wordmark "Bmidia" em PNG (bege, branco, marrom, marrom-escuro, preto-oliva)
│   ├── Icone/                 ← ícone "bm" em SVG (8 versões)
│   └── Elementos/             ← 6 arcos + 6 patterns em SVG
├── fonts/                     ← Nearo Rounded, Montserrat, Hanken Grotesk, Playfair Display
├── componentes/               ← prévias HTML do Resumo PDF e da capa
└── docs/                      ← guia da marca completo
outras-ias/
├── instrucoes-para-colar.md   ← as regras da skill em texto para colar (ChatGPT, Gems, outras)
└── arquivos-para-anexar/      ← 17 arquivos: logos, ícones e arcos em PNG + tokens.json + guia
dist/
├── bmidia-design-system.zip   ← skill completa
├── bmidia-skill-leve.zip      ← skill sem fontes e prévias (Gemini)
└── bmidia-pacote-outras-ias.zip
```

## Paleta oficial

| Token | HEX | Uso |
|---|---|---|
| verde-profundo | `#283C3A` | fundos fortes, ícone verde |
| olive | `#6D6A38` | capas, impressos |
| beige | `#CABDAA` | logo, ícone, arcos, filetes |
| linho | `#E3DFD4` | fundos neutros |
| brown | `#876047` | fundo de marca principal |
| grafite | `#2F2D2E` | texto escuro, fundos dramáticos |

Complementares: cream `#FFF8EF` · off-white `#F7F6F1` · brown-deep `#662900` · brown-text `#94430D` · sand `#DFD2C1` · dark `#1B1B13` · gold `#DFB956` · red `#CD2438` (uma palavra por peça).

Guia completo: [docs/guia-da-marca.md](bmidia-design-system/docs/guia-da-marca.md)

---

## Problemas comuns

| Problema | Solução |
|---|---|
| Link de download dá **404** | O repositório é privado: entre no GitHub com a conta que foi convidada. |
| **Erro no upload** da skill | Envie o `.zip` sem descompactar. No Claude, ligue a execução de código. Se persistir, use a skill leve. |
| Não aparece **Skills** | Claude Team/Enterprise e ChatGPT Business/Enterprise: peça ao administrador. ChatGPT Free/Plus/Pro: use Projetos ou GPT. |
| A IA não usou a identidade | Mencione "BMidia" no pedido ou diga "siga o design system da BMidia". |
| Fonte aparece diferente no Canva/Figma | Instale as fontes da pasta `fonts/` e reabra o programa. |

---

## Fonte e créditos

Guia de marca BMidia (Studio Sagi), incorporado em 30/10/2026. Mantido por Eligere Digital.

**Uso interno da BMidia.** Logos e identidade visual são da BMidia Digitais. As fontes seguem as licenças dos seus autores: Montserrat, Hanken Grotesk e Playfair Display são livres (SIL OFL); verifique a licença da Nearo Rounded antes de redistribuir fora da equipe.
