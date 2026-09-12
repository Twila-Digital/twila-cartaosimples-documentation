# Instruções para agentes neste projeto

## Sobre este projeto

- Documentação da API de integração do Parcele+ (crédito e parcelamento no momento da compra), construída em [Mintlify](https://mintlify.com)
- Páginas são arquivos MDX com front-matter YAML
- Configuração de navegação em `docs.json`
- Páginas de referência de endpoints usam `openapi:` no front-matter e puxam descrição/parâmetros de `openapi.yaml` — não duplique essa informação manualmente na página
- Rode `mint dev` para pré-visualizar localmente e `mint broken-links` para checar links

## Terminologia

- "Parcele+" (sem espaço antes do `+`), não "Parcele +" ou "ParceleMais" em texto visível para o leitor — "ParceleMais" é usado apenas em identificadores técnicos (nome do SDK, `PackageId`, etc.)
- "pedido", não "compra" ou "transação"
- "parceiro", não "cliente da API" ou "merchant" — "cliente" é reservado para o cliente final do parceiro (`Customer`)
- "CDC" (crédito direto ao consumidor) é o nome do fluxo principal do produto
- Todo o conteúdo das páginas é em português do Brasil

## Estilo

- Use voz ativa e segunda pessoa ("você")
- Frases curtas — uma ideia por frase
- Sentence case em títulos
- Nomes de arquivo, comandos, caminhos e identificadores de código em `code formatting`
- Campos JSON de listas paginadas usam `itens` (não `items`) — reflete o nome do campo na API real

## Limites de conteúdo

- Documenta apenas a API de integração pública (`WebIntegration`), voltada a parceiros — não documenta endpoints internos de backoffice/admin
- SDKs oficiais ficam na aba "SDKs"; ao adicionar um novo SDK, inclua link para o repositório no GitHub e, se aplicável, para o pacote publicado
