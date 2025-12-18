# Tech Store Sales — Pandas Study

Mini projeto de análise de vendas de uma loja. O notebook mostra a leitura da base e os cálculos usados para comparar categorias, identificar o produto mais vendido e encontrar a região com maior receita.

## O que está no notebook

`analise_vendas.ipynb` carrega `data/vendas.csv`, inspeciona a tabela e cria `receita_total` a partir de quantidade e preço unitário. Em seguida, faz os recortes e agrupamentos da análise.

As células mantêm os resultados intermediários para facilitar a conferência dos cálculos. É um exercício de Pandas, não um dashboard nem uma aplicação publicada.

## Como abrir

Na raiz do repositório:

```bash
pip install pandas notebook
jupyter notebook
```

Abra `analise_vendas.ipynb` e execute as células em ordem. Mantenha a pasta `data/` no mesmo lugar, porque a leitura usa um caminho relativo.

Referência de estudo: Rocketseat.

## Licença

Código e documentação autorais sob [MIT](license). Bases de dados, materiais de curso e outros conteúdos de terceiros mantêm seus termos próprios.
