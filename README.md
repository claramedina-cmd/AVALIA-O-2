# 📈 Análise de Ações Brasileiras com Python

Este projeto realiza uma análise exploratória de dados de ações brasileiras utilizando Python e a biblioteca `yfinance`. O objetivo é coletar dados históricos de empresas listadas na B3 e analisar informações como abertura, fechamento, máximas, mínimas e volume de negociação.

As empresas analisadas no projeto são:

* Vale S.A. (`VALE3.SA`)
* Ambev S.A. (`ABEV3.SA`)
* Itaú Unibanco (`ITUB4.SA`)
* Banco do Brasil (`BBAS3.SA`)

---

# 🚀 Tecnologias Utilizadas

O projeto foi desenvolvido em Python utilizando as seguintes bibliotecas:

```python
pip install yfinance pandas matplotlib seaborn
```

Bibliotecas utilizadas:

* `yfinance` → download de dados financeiros
* `pandas` → manipulação de dados
* `matplotlib` → visualização gráfica
* `seaborn` → estilização dos gráficos

---

# 📂 Estrutura do Projeto

O notebook está dividido em seções de análise para cada empresa:

## 1. Análise Vale

Ticker utilizado:

```python
VALE3.SA
```

Período analisado:

```python
2023-01-01 até 2026-05-14
```

Etapas realizadas:

* Download dos dados históricos
* Organização das colunas
* Visualização das primeiras linhas
* Visualização das últimas linhas
* Análise de preços e volume

---

## 2. Análise Ambev

Ticker utilizado:

```python
ABEV3.SA
```

Período analisado:

```python
2023-01-01 até 2026-05-14
```

Etapas realizadas:

* Download dos dados históricos
* Organização das colunas
* Visualização das primeiras linhas
* Visualização das últimas linhas
* Análise de preços e volume

---

## 3. Análise Itaú

Ticker utilizado:

```python
ITUB4.SA
```

Período analisado:

```python
2023-01-01 até 2026-05-14
```

Etapas realizadas:

* Download dos dados históricos
* Organização das colunas
* Visualização das primeiras linhas
* Visualização das últimas linhas
* Análise de preços e volume

---

## 4. Análise Banco do Brasil

Ticker utilizado:

```python
BBAS3.SA
```

Período analisado:

```python
2023-01-01 até 2026-05-14
```

Etapas realizadas:

* Download dos dados históricos
* Organização das colunas
* Visualização das primeiras linhas
* Visualização das últimas linhas
* Análise de preços e volume

---

# 📊 Exemplo de Código

```python
import yfinance as yf
import pandas as pd

# Definição do ticker
ticker = "VALE3.SA"

# Download dos dados
_df = yf.download(ticker, start="2023-01-01", end="2026-05-14")

# Renomeando colunas
_df.columns = ['Abertura', 'Máxima', 'Mínima', 'Fechamento', 'Volume']

# Exibindo dados
print(_df.head())
```

---

# 📌 Objetivo do Projeto

Este projeto foi desenvolvido com fins acadêmicos e educacionais, permitindo:

* Aprender análise de dados financeiros
* Trabalhar com dados históricos da bolsa de valores
* Desenvolver habilidades em Python para mercado financeiro
* Explorar visualização e manipulação de dados

---

# ▶️ Como Executar

1. Clone este repositório:

```bash
git clone <URL_DO_REPOSITORIO>
```

2. Instale as dependências:

```bash
pip install yfinance pandas matplotlib seaborn
```

3. Abra o notebook:

```bash
jupyter notebook
```

4. Execute as células do notebook.

---

# 📈 Possíveis Melhorias

Algumas melhorias futuras para o projeto:

* Adicionar gráficos interativos
* Comparar desempenho entre ações
* Calcular médias móveis
* Implementar indicadores técnicos
* Criar dashboards financeiros
* Automatizar atualização dos dados

---

# 👩‍💻 Autoria

Projeto desenvolvido para estudos de análise de dados financeiros utilizando Python e dados da B3.
