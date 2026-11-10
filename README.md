# CAECO.extensão

Site do Centro Acadêmico de Economia (CAECO) da UFC com os projetos de extensão da FEAAC, os editais com vaga para Economia e os links oficiais da UFC.

Site estático: `index.html` + `logo-caeco.png`. Sem build. Tema escuro com efeito de vidro (glassmorphism); as cores ficam nas variáveis CSS em `:root`.

## Como atualizar a lista

Edite o array `PROJETOS` no final do `index.html`. Cada item usa a função `P(nome, cats, depto, tipo, status, info, links, desc)`.

- `cats`: `vaga` (edital com vaga para Economia), `eco` (DTE/DEA), `ativo` (lista 2025), `evento`, `hist` (antes de 2025)
- Fonte da lista: https://feaac.ufc.br/pt/projeto-de-extensao/ (conferida em 09/11/2026)

## Prazos dos editais

No `index.html`, logo abaixo da lista `PROJETOS`, fica o objeto `PRAZOS`. Cada linha usa o nome exato da ação e as datas no formato `AAAA-MM-DD`:

```js
"Nome da ação":{ini:"2027-03-15",fim:"2027-03-18",obs:"texto opcional"},
```

O site calcula sozinho se as inscrições estão abertas ("faltam X dias"), se vão abrir ou se encerraram, e coloca os abertos primeiro no filtro de editais.

## Botão "Sugerir correção"

Preencha `WHATSAPP` (só números, com 55 + DDD, ex.: `5585999999999`). Enquanto estiver vazio, o botão não aparece.

## Links diretos para filtros

- `/#vagas`: editais com vaga para Economia
- `/#economia`: departamentos de Economia (DTE/DEA)
- `/#2025`: lista de 2025
- `/#eventos`: seminários e eventos
- `/#antigos`: registrados antes de 2025

O botão "Copiar link deste filtro", acima da lista, copia o link do filtro aberto.

## Prévia de link e visitas

- `og.png` (1200×630) é a imagem que aparece ao compartilhar o link no WhatsApp/Instagram.
- A contagem de visitas usa o Vercel Web Analytics. Ela precisa estar ligada no painel da Vercel: projeto > Analytics > Enable.

