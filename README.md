# Tech Store Sales — EDA End-to-End (Pandas)

> **End-to-end EDA of Tech Store sales using Pandas: data validation, cleaning, revenue and quantity analysis, monthly trends, category and region breakdowns, and top-selling products—all in a Jupyter Notebook. Made with 💜 by Rocketseat.**

Este repositório contém um **mini projeto de treinamento de EDA (Exploratory Data Analysis)** em cima de uma base de **vendas de uma loja (Tech Store)**, totalmente executado em um **Jupyter Notebook** com foco em boas práticas de análise: entendimento da base, validação, preparação de dados e geração de insights de negócio.

---

## O que você encontra aqui

No notebook `analise_vendas.ipynb`, você vai passar por etapas típicas de um EDA de vendas:

- **Leitura e inspeção inicial** do dataset (`info()`, `head()`, `shape`)
- **Validação e ajustes de tipos** (ex.: colunas numéricas e datas)
- **Criação de métrica de negócio**: `receita_total = quantidade * preco_unitario`
- **Análises por receita e por quantidade**
- **Cortes por categoria e região**
- **Identificação de destaques** (ex.: produto mais vendido, região com maior receita)

---

## Estrutura do projeto

```text
.
├── analise_vendas.ipynb
└── data/
    └── vendas.csv
```

---

## Dataset

Arquivo: `data/vendas.csv`  
Tamanho: **100 linhas × 7 colunas** (conforme `df.info()` / `df.shape` no notebook)

**Colunas:**
- `data` (string no CSV) — data da venda (ex.: `2025-12-09`)
- `produto` (string) — nome do produto
- `categoria` (string) — categoria (ex.: Eletrônicos, Móveis, Periféricos, Vestuário)
- `quantidade` (int) — quantidade vendida
- `preco_unitario` (int) — preço por unidade
- `cliente` (string) — cliente
- `regiao` (string) — região (ex.: Sudeste, Sul, Norte, Nordeste, Centro-Oeste)

**Métrica criada no EDA:**
- `receita_total` — `quantidade * preco_unitario`

---

## Exemplos de insights gerados (com a base atual)

- **Produto mais vendido (por quantidade):** `Sofá Q`
- **Região com maior receita:** `Sudeste` (ex.: `245605`)

> Observação: os resultados acima vêm da execução do notebook com o CSV incluído no repositório.

---

## Como executar

### 1) Pré-requisitos
- Python **3.10+** (recomendado: 3.12+)
- Jupyter Notebook / JupyterLab

### 2) Setup rápido

```bash
# (opcional) criar e ativar venv
python -m venv .venv

# Windows
.venv\Scripts\activate

# Linux/Mac
source .venv/bin/activate
```

```bash
pip install -U pip
pip install pandas jupyter
```

### 3) Rodar o notebook

```bash
jupyter notebook
```

Abra o arquivo: `analise_vendas.ipynb`

---

## Notas importantes

- O notebook lê o CSV usando o caminho relativo:
  ```python
  pd.read_csv("./data/vendas.csv")
  ```
  Então mantenha a pasta `data/` no mesmo nível do notebook.

- Projeto com foco em **aprendizado** e **prática de EDA** (base pequena e controlada).

---

## Próximos upgrades (ideias)

- Padronizar parse de datas (`pd.to_datetime`) e criar colunas de ano/mês
- Formatação de moeda e visualizações mais completas (ex.: `matplotlib` com labels e títulos)
- Export de tabelas agregadas (CSV) para consumo em Power BI / Tableau
- `requirements.txt` e/ou `pyproject.toml` para reprodutibilidade

---

## Créditos

Made with 💜 by Rocketseat.
