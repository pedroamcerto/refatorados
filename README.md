# Refatorados · Gênesis

Página da célula **Refatorados** para acompanhar a jornada de leitura do livro de Gênesis.

Todo dia, a partir de **14 de maio de 2026**, a página mostra automaticamente qual capítulo deve ser lido e quais dois membros são responsáveis por trazer o resumo na célula. A escala é determinística — todo mundo que acessar no mesmo dia vê a mesma coisa.

## Como funciona

- **1 capítulo por dia** durante 50 dias (Gênesis tem 50 capítulos)
- **2 membros por dia** sorteados com rodízio justo: a cada 4 dias, cada membro apresentou exatamente uma vez
- O sorteio usa um seed fixo (`20260514`), então não depende de banco de dados nem servidor — é puro HTML + JS

## Estrutura

```
refatorados/
└── index.html   # página completa, sem dependências externas
```

## Como rodar localmente

Basta abrir o `index.html` no navegador. Não precisa de servidor.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (ex: `refatorados`)
2. Suba o `index.html` para a branch `main`
3. Vá em **Settings → Pages → Source** e selecione `main / root`
4. Pronto — a página fica disponível em `https://<seu-usuario>.github.io/refatorados/`

## Membros atuais

- Fabiano
- Pedro Certo
- Pedro
- Vinicius Gardim
- Bruna
- Gabriel
- Carlos
- Lorran Santos

Para adicionar membros, basta editar o array `MEMBERS` no `index.html`. e a escala se recalcula automaticamente.
