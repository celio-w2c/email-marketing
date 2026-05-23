# COP · Email Marketing

Repositório de templates HTML de email marketing do **COP International**, publicados via GitHub Pages para importação direta no **RD Station Marketing**.

## URL pública

**Index navegável:** https://celio-w2c.github.io/email-marketing/

## Emails disponíveis

| # | Email | URL pública (RD Station) |
|---|---|---|
| 01 | A Operação Começou | https://celio-w2c.github.io/email-marketing/cop-email-marketing-01.html |
| 02 | Briefing Semanal · Segurança Pública | https://celio-w2c.github.io/email-marketing/cop-email-marketing-02-briefing-semanal.html |

## Como importar no RD Station

1. Copie a URL pública do email desejado (acima ou via `index.html`).
2. No RD Station Marketing, vá em **Relacionar → Email → Novo email**.
3. Selecione o editor **HTML** → opção **"Importar de URL"**.
4. Cole a URL e clique em importar — o RD faz o fetch do HTML.
5. Os merge tags `%mensagem-link-descadastro%` e `%mensagem-link-preferencias%` são substituídos automaticamente pelo RD.
6. Configure remetente, assunto, segmentação e dispare.

## Características técnicas

- **Design system COP** aplicado (paleta black/yellow, Barlow Condensed, hazard stripes, tactical grid)
- **Tabela-based layout** com largura 600px (padrão email)
- **Responsivo mobile** via media query @ 620px
- **Outlook compatível** com VML bulletproof buttons + fallback SVG → texto
- **Dark mode aware** via `prefers-color-scheme`
- **Sob 50 KB** cada (limite de clip do Gmail: 102 KB)
- **Logo SVG inline** — zero requisições externas para imagens
- **Google Fonts** via `<link>` único com fallback gracioso para Arial Black / Arial

## Estrutura

```
.
├── index.html                                    # Landing page navegável
├── cop-email-marketing-01.html                   # Email 01
├── cop-email-marketing-02-briefing-semanal.html  # Email 02
└── README.md
```

## Setup do GitHub Pages

Pages servido a partir da branch `main` (raiz). Configurar em:
**Settings → Pages → Source: Deploy from a branch → Branch: main / (root)**.
