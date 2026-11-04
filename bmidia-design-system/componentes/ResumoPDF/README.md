# ResumoPDF

Página A4 do resumo de reunião da BMidia: cabeçalho `brown` com logo bege, título em Playfair com a última palavra em itálico, e o corpo em seções.

## Blocos

| Bloco | Quando usar | Visual |
|---|---|---|
| Texto corrido | contexto, resumo, pauta | parágrafos 10.5pt |
| Números | resultados do período | cartões `brown`, valor em Hanken Bold `cream` |
| Metas | objetivos numéricos | cartões `off-white` com borda `brown`, valor `brown-deep` |
| Tópicos | decisões, pontos discutidos | lista numerada 01, 02… em Playfair itálico |
| Alertas | atenção, riscos, observações | faixa `alert-tint` com sublinhado `gold` |
| Ações | próximos passos | uma coluna por responsável (`brown-deep`, depois `olive`), checkbox e selo de prazo `gold` |

## Regras

- O cabeçalho só existe na primeira página; as demais têm margem de 16mm no topo e rodapé com `@BMIDIADIGITAIS` e paginação.
- Números e listas curtas não quebram entre páginas; títulos de seção nunca ficam sozinhos no pé da página.
- O consumidor fornece: cliente, título, data, participantes e as seções. O app *Resumos de reunião* monta tudo a partir de um texto colado.

Escrito à mão a partir de `app/engine.js` (funções `renderBlock` e `buildDoc`); a prévia é uma versão estática.
