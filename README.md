# CAECO.extensão

Site do Centro Acadêmico de Economia (CAECO) da UFC com os projetos de extensão da FEAAC, os editais com vaga para Economia e os links oficiais da UFC.

Site estático: `index.html` + `logo-caeco.png`. Sem build.

## Como atualizar a lista

Edite o array `PROJETOS` no final do `index.html`. Cada item usa a função `P(nome, cats, depto, tipo, status, info, links, desc)`.

- `cats`: `vaga` (edital com vaga para Economia), `eco` (DTE/DEA), `ativo` (lista 2025), `evento`, `hist` (antes de 2025)
- Fonte da lista: https://feaac.ufc.br/pt/projeto-de-extensao/ (conferida em 09/11/2026)
