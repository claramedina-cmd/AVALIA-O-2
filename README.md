# Machine Learning Aplicado à Administração

## 📊 Análise Estratégica da Concentração no Comércio Global de Bens Criativos

Este repositório apresenta a **Avaliação 1 (A1)** da disciplina de **Machine Learning aplicado à Administração**, desenvolvida em Python e Google Colab a partir do dataset **OpenFCS**, relacionado ao comércio internacional de bens criativos.

O projeto utiliza técnicas de **análise de dados, Python, pandas, NumPy e SQL com DuckDB** para explorar padrões do comércio global, com foco na estrutura competitiva e na concentração entre economias, parceiros comerciais e domínios criativos.

---

## 🎯 Objetivo

O objetivo da análise é transformar dados de comércio internacional em informações úteis para **Inteligência de Mercado**, identificando padrões e relações entre:
- Economias;
- Parceiros comerciais;
- Domínios de bens criativos;
- Anos analisados;
- Valores de comércio em milhões de dólares.

A análise parte do dado bruto e utiliza ferramentas de tratamento, exploração e consulta de dados para responder às questões propostas na avaliação.

---

## 📚 Base de Dados

O projeto utiliza o **OpenFCS Dataset**, baseado no acervo de comércio internacional de bens criativos.

**Fonte:** Monteiro & Dubeux (2026)  
**Dataset:** OpenFCS v1.0.0  
**Licença:** CC-BY-4.0  
**DOI:** https://doi.org/10.5281/zenodo.21211053

---

## 🗂️ Tratamento dos Dados

Na primeira etapa do notebook, os dados são baixados e organizados a partir dos arquivos:
- `trade_edges.csv`
- `entities.csv`
- `products_crosswalk.csv`

O dataset original contém aproximadamente **2,2 milhões de registros** em `trade_edges.csv`. Para a análise, é aplicado o filtro de resolução `cer7`, resultando em uma tabela com **1.026.400 linhas**.

A tabela principal utilizada no projeto é a `edges7`, que contém informações como:

| Variável | Descrição |
|---|---|
| `economy` | Economia de origem |
| `partner` | Parceiro comercial |
| `product` | Produto ou categoria de bem criativo |
| `year` | Ano do registro |
| `value_usd_millions` | Valor do comércio em milhões de dólares |
| `flow` | Tipo de fluxo comercial |
| `cer_code` | Código do produto |
| `fcs_domain` | Domínio criativo |
| `mapping_status` | Status do mapeamento |

---

## 🛠️ Tecnologias Utilizadas

- **Python 3**
- **Google Colab**
- **Pandas** — manipulação e análise dos dados
- **NumPy** — operações numéricas
- **DuckDB** — consultas SQL e análise de dados
- **SQL** — consultas e agregações
- **Machine Learning / Inteligência Artificial** — apoio à exploração e interpretação dos dados

---

## 🔎 Principais Etapas da Análise

1. **Download e preparação dos dados**
2. **Leitura e organização das tabelas**
3. **Filtragem da resolução de sete domínios**
4. **Exploração das estruturas e variáveis**
5. **Consultas utilizando DuckDB e SQL**
6. **Agregação dos valores de comércio**
7. **Análise de economias e parceiros comerciais**
8. **Análise por domínio criativo**
9. **Interpretação dos resultados sob a perspectiva de Inteligência de Mercado**
10. **Modelagem conceitual em esquema estrela para análise dos dados**

---

## 🧠 Inteligência de Mercado

A análise busca responder perguntas de negócio a partir dos dados, como a identificação dos principais parceiros comerciais de uma economia dentro de determinado domínio criativo.

Para isso, o projeto considera uma estrutura de dados em que:
- A **tabela fato** concentra as medidas quantitativas, como o valor comercializado;
- As **dimensões** fornecem informações de contexto, como tempo, economia, parceiro e domínio criativo.

Essa estrutura facilita consultas, filtros e agregações para apoiar análises estratégicas.

---

## 🤖 Uso de Inteligência Artificial

Durante o desenvolvimento, ferramentas de Inteligência Artificial podem ser utilizadas como apoio à compreensão de conceitos, revisão de sintaxe, desenvolvimento de código e interpretação dos resultados.

O uso de IA segue a orientação da avaliação de que qualquer utilização deve ser declarada no próprio notebook, mantendo a responsabilidade do aluno pela compreensão e explicação das soluções apresentadas.

---

## 📓 Notebook

O principal arquivo do projeto é:

**[Cópia_de_avaliacao_1_ml_administracao.ipynb](./C%C3%B3pia_de_avaliacao_1_ml_administracao.ipynb)**

O notebook pode ser executado diretamente no **Google Colab**, permitindo reproduzir as etapas de preparação, consulta e análise dos dados.

---

## ▶️ Como Executar

### Google Colab

1. Abra o arquivo `.ipynb` disponível neste repositório.
2. Abra-o no Google Colab.
3. Execute as células na ordem apresentada.
4. Aguarde o download e processamento do dataset OpenFCS.
5. Execute as consultas e análises propostas na avaliação.

### Ambiente local

É necessário ter Python instalado e as principais bibliotecas utilizadas no notebook.

```bash
pip install pandas numpy duckdb requests
```

Depois, o notebook pode ser aberto com Jupyter:

```bash
jupyter notebook
```

---

## 📌 Resultado Esperado

Ao final da execução, o notebook permite analisar a estrutura do comércio internacional de bens criativos e utilizar os dados para responder às questões propostas na avaliação, relacionando **programação, análise de dados, SQL e Inteligência de Mercado**.

---

## 👩‍💻 Autoria

**Clara Medina**

Projeto acadêmico desenvolvido para a disciplina de **Machine Learning aplicado à Administração**.