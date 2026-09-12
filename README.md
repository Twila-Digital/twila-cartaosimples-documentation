# Documentação do Parcele+

Site de documentação da API do [Parcele+](https://www.cartaosimples.com.br), construído com [Mintlify](https://mintlify.com).

Publicado em produção a partir da branch `production`.

## Estrutura

- `docs.json` — navegação, tema e configuração do site
- `openapi.yaml` — especificação OpenAPI da API de integração, usada para gerar as páginas de referência
- `pages/` — conteúdo das páginas (MDX)

## Para IAs e agentes

O índice completo da documentação está disponível em [`/llms.txt`](https://docs.parcelemais.com.br/llms.txt). Qualquer página também pode ser lida como Markdown puro trocando a extensão da URL para `.md`.

## SDKs

- [.NET](https://github.com/Twila-Digital/twila-parcelemais-dotnet-sdk)

## Desenvolvimento local

Instale a CLI da Mintlify:

```bash
npm i -g mint
```

Na raiz deste repositório (onde está o `docs.json`):

```bash
mint dev
```

Acesse `http://localhost:3000`.

Para validar links quebrados:

```bash
mint broken-links
```

## Publicação

Alterações na branch `production` são publicadas automaticamente via o GitHub App da Mintlify.

## Contribuindo

Veja [CONTRIBUTING.md](CONTRIBUTING.md).
