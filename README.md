# Aura

Miniapp web standalone para PhizClip/Phiz.

## Estrutura

- `index.html`: app completo, auto-contido.
- `logo.png`: logo usado como referencia visual.

## Objetivo

Publicar o Aura como uma URL HTTPS publica e usar essa URL no template `Webview` do PhizClip Studio.

## Fluxo recomendado

1. Criar um repositorio separado so para o Aura.
2. Subir apenas estes arquivos.
3. Publicar em um host estatico confiavel.
4. Colar a URL final no `src` do `web-view` do projeto do PhizClip.
5. Testar no preview QR e depois enviar para revisao.

## Hospedagem recomendada

Opcao preferida: Cloudflare Pages

Motivos:

- HTTPS nativo.
- URL publica estavel.
- Deploy simples para site estatico.
- Nao depende de servidor rodando no Mac.
- Bom para um miniapp de arquivo unico.

Alternativa boa: GitHub Pages

- Simples e barato.
- Bom para projeto estatico separado.
- Menos flexivel que Cloudflare Pages, mas suficiente.

## Observacoes

- Nao usar tunnel temporario para submissao final.
- Nao usar link com autenticacao.
- Se o Phiz compartilhar thumbnail remota, a imagem precisa estar em URL publica tambem.
