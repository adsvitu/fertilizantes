# Diretivo Principal — RCM Fertilizantes LP

## Objetivo
Landing page de captura de leads para a RCM Fertilizantes.
Produto: Fertilizante de casco e chifre bovino.
Público: Produtor rural e revendedor agrícola.

## Entregável
- `index.html` — LP completa (self-contained, HTML/CSS/JS)
- `hero.png` — Imagem de lavoura (gerada via IA)

## Estrutura de Blocos
1. Navbar — Logo + âncoras + CTA
2. Hero — Headline + bullets + CTA
3. Dor — Card diagnóstico + callout verde
4. Solução — 4 cards brancos em grid
5. Benefícios — 4 cards verdes em grid
6. Produto — Parágrafo + pills de atributos
7. Autoridade — 4 metric cards
8. Formulário — Conversão principal (nome, whatsapp, cultura, mensagem)
9. FAQ — Accordion (4 perguntas)
10. Footer — Logo + texto + WhatsApp

## Integração de Formulário (PENDENTE)
O formulário está preparado para webhook.
Substituir `WEBHOOK_URL` no JS por:
- n8n webhook (preferido — já usado em outros projetos)
- Make/Zapier
- Google Sheets via Apps Script

Campos enviados:
```json
{
  "nome": "string",
  "whatsapp": "string",
  "cultura": "graos|pastagem|hortalicas|frutiferas|outro",
  "mensagem": "string",
  "origem": "LP RCM Fertilizantes",
  "timestamp": "ISO 8601"
}
```

## WhatsApp
Substituir `5500000000000` pelo número real da RCM em:
- `wa-float` (botão flutuante)
- `footer-wa` (link do footer)
- `lead-form` (redirecionamento pós-envio)

## SEO
- Palavra-chave principal: "fertilizante de casco e chifre bovino"
- Title: ✅ presente
- Meta description: ✅ presente
- H1/H2 com KW: ✅ presente
- KW no corpo: ✅ ≥2x

## Aprendizados / Observações
- Imagem hero em `hero.png` — pode ser trocada por foto real do produto/lavoura
- Design system: verde #2E7D32 / #1B5E20, tipografia Poppins + Inter
- Mobile first, botão flutuante WhatsApp fixo
- Toast de confirmação no envio do formulário
- Após envio, abre WhatsApp com mensagem contextualizada
