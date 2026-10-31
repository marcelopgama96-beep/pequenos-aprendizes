# Pequenos Aprendizes

Cópia da página de vendas original, com o mesmo conteúdo, layout responsivo, efeitos e quatro botões de compra.

## Publicar

O site é estático: publique esta pasta em GitHub Pages (branch `main`, pasta `/ (root)`), Netlify, Vercel ou outro servidor estático. O arquivo de entrada é `index.html`. Não requer instalação ou build para publicar.

## Compra

Todos os botões encaminham ao checkout original:
https://pay.hotmart.com/H108180859P?off=rkvpy6ps&hotfeature=51

O pagamento e a entrega do PDF são realizados pela Hotmart. O repositório não processa pagamentos nem contém o PDF vendido. O checkout respondeu HTTP 200 na verificação; nenhuma transação foi efetuada.

## Recursos e manutenção

Imagens e CSS estão em `assets/`. A fonte Outfit é carregada pelo Google Fonts, com alternativa sans-serif. O CSS já foi gerado para produção. Para regenerá-lo após mudar classes:

```sh
npx --yes --package=tailwindcss@3.4.17 tailwindcss -i styles.input.css -o assets/styles.css --minify
```

Foram retirados apenas o redirecionamento HTTPS imposto pela hospedagem original e os scripts de analytics/launcher específicos da Hotmart Host. Os links de pagamento e seus parâmetros foram preservados.

Origem: https://marcelopgama96.hotmart.host/pequenos-aprendizes-kit-com-1-000-atividades-para-educacao-infantil-em-pdf-896266b9-46ad-42a1-8ea9-28873f2d08eb
