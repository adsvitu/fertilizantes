# RCM Fertilizantes — Landing Page

LP de captura de leads para a **RCM Fertilizantes** — fabricante de fertilizante orgânico de casco e chifre bovino.

## Stack
- HTML + CSS + Vanilla JS (self-contained)
- GTM `GTM-5X6D3NV5` (head + noscript)
- n8n webhook → Google Sheets + notificação WhatsApp

## Estrutura
```
/
├── index.html                    ← LP principal
├── politica-de-privacidade.html  ← Política LGPD
├── logo.png                      ← Logo RCM
├── hero.png                      ← Imagem hero (lavoura)
└── directives/
    └── 01_main_directive.md      ← Documentação do projeto (DEO)
```

## Configuração antes de publicar

1. **Webhook n8n** — substituir em `index.html`:
   ```js
   const WEBHOOK_URL = 'https://n8n.seudominio.com.br/webhook/rcm-fertilizantes';
   ```

2. **WhatsApp** — substituir `5500000000000` pelo número real da RCM em 3 lugares no HTML.

3. **Workflow n8n** — importar `../n8n_auto/n8n/exports/RCM_FERTILIZANTES.json` no painel n8n.

## SEO
- Keyword principal: `fertilizante de casco e chifre bovino`
- MAPA RN 000828-1
