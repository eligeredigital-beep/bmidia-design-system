# BMidia Digitais — Design System + Skill para o Claude

Identidade visual completa da **BMidia Digitais**, a agência de tráfego pago para confeitarias, empacotada como uma **skill do Claude**. Com ela instalada, qualquer pessoa da equipe pede "faz um carrossel da BMidia sobre…" ou "monta o resumo da reunião com o cliente X" e o Claude já entrega na paleta, nas fontes e com os logos oficiais, sem precisar explicar a marca toda vez.

> **Nome da marca: BMidia, sem S.** Handle: `@BMIDIADIGITAIS`. Assinatura: *A revolução do tráfego pago na confeitaria!*

---

## O que é uma skill

Uma skill é uma pasta com um arquivo `SKILL.md` (instruções) e os arquivos de apoio (logos, fontes, tokens). O Claude lê a skill automaticamente sempre que o pedido tem a ver com ela, no caso, qualquer peça da BMidia.

Esta skill ensina ao Claude:

- **Conceito e voz:** propósito, atributos, manifesto, assinatura, "números primeiro", títulos em dois tons.
- **Cores:** a paleta oficial do guia de marca (Studio Sagi) e as complementares, com os pares de contraste aprovados.
- **Tipografia:** Nearo Rounded + Montserrat para a marca; HK Grotesk, Helvetica e Montserrat nas redes; escalas para carrossel 1080×1350, apresentações e PDF A4.
- **Logo e ícone:** qual versão usar em cada fundo, respiro e o que nunca fazer.
- **Elementos:** arcos, patterns, layouts de carrossel, faixa de métrica, pill de CTA.
- **Componente Resumo de reunião (PDF A4):** cabeçalho, números, metas, tópicos, alertas e colunas de ações.

## O que tem aqui

```
bmidia-design-system/          ← a skill (esta pasta é o que se instala)
├── SKILL.md                   ← instruções que o Claude segue
├── tokens.css                 ← @font-face + variáveis CSS (cores, fontes, espaços, cantos) + classes de tipografia
├── tokens.json                ← os mesmos tokens, com regras de uso e contraste
├── assets/
│   ├── Logos/                 ← wordmark "Bmidia" em PNG (bege, branco, marrom, marrom-escuro, preto-oliva)
│   ├── Icone/                 ← ícone "bm" em SVG (8 versões)
│   └── Elementos/             ← 6 arcos + 6 patterns em SVG
├── fonts/                     ← Nearo Rounded, Montserrat, Hanken Grotesk, Playfair Display
├── componentes/
│   ├── ResumoPDF/             ← prévia HTML do resumo de reunião A4
│   └── Cover/                 ← prévia HTML de capa
└── docs/
    ├── guia-da-marca.md       ← guia completo em texto
    └── historico-carrossel-tayna.md
dist/
└── bmidia-design-system.zip   ← a skill pronta para enviar no Claude.ai
```

---

## Como instalar

### Opção 1 — Claude.ai (app web, desktop ou celular)

1. Baixe **[`dist/bmidia-design-system.zip`](dist/bmidia-design-system.zip)** (abra o arquivo e clique em *Download raw file*). Não descompacte.
2. Confirme que **execução de código** está ligada em **Configurações → Capacidades** (planos Free, Pro, Max e Ultra; no Team já vem ligada).
3. Vá em **Personalizar (Customize) → Skills**.
4. Clique em **+** → **Criar skill (Create skill)** → **Enviar uma skill (Upload a skill)** e selecione o `.zip`.
5. A skill **bmidia-design-system** aparece na lista; deixe o botão ativado.

> Team/Enterprise: o dono da organização pode ter desativado skills criadas por usuários. No Enterprise, ele precisa habilitar execução de código e skills em **Configurações da organização → Plugins e skills**. Guia oficial: [Usar skills no Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

### Opção 2 — Claude Code (terminal)

Skill pessoal (vale em todos os seus projetos):

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

Só para um projeto: copie a pasta `bmidia-design-system/` para `.claude/skills/` dentro do projeto.

### Opção 3 — API do Claude

Envie a pasta `bmidia-design-system/` pela API de Skills e referencie o `skill_id` nas requisições. Documentação: https://docs.claude.com

### Atualizar

Baixe o `.zip` novo e envie de novo (Claude.ai), ou rode `git pull` e copie a pasta outra vez (Claude Code).

---

## Como usar

Não precisa chamar a skill pelo nome: basta mencionar a BMidia no pedido. Exemplos:

- *"Cria um carrossel da BMidia de 6 slides sobre por que confeitaria precisa de tráfego pago no Natal."*
- *"Monta o resumo da reunião de hoje com a Doce Ateliê no padrão BMidia"* (cole as anotações da reunião).
- *"Faz uma apresentação institucional da BMidia para prospecção."*
- *"Post de case: cliente faturou R$ 30 mil/mês, no estilo BMidia."*
- *"Quais cores e fontes eu uso num story da BMidia?"*

O Claude vai aplicar a paleta, as fontes, o logo certo para cada fundo, o handle `@BMIDIADIGITAIS` no rodapé e o checklist da marca antes de entregar.

### Usando os arquivos sem o Claude

- **Web / HTML:** linke o `tokens.css` (mantendo a pasta `fonts/` ao lado) e use as variáveis: `background: var(--brown); color: var(--cream); font-family: var(--font-marca);`
- **Canva / Figma / Illustrator:** importe os logos de `assets/Logos`, os ícones e elementos (SVG) e instale as fontes de `fonts/`. Os HEX da paleta estão na tabela abaixo.

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

---

## Fonte e créditos

Guia de marca BMidia (Studio Sagi), incorporado em 30/10/2026, e o design system "BMidia Digitais" mantido no Claude. Mantido por Eligere Digital.

**Uso interno da BMidia.** Logos e identidade visual são da BMidia Digitais. As fontes seguem as licenças dos seus autores: Montserrat, Hanken Grotesk e Playfair Display são livres (SIL OFL); verifique a licença da Nearo Rounded antes de redistribuir fora da equipe.
