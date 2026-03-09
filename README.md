# Telecom-X---Parte-2

# 📊 Telecom X – Parte 2: Previsão de Churn de Clientes

## 📌 Propósito do Projeto

Este projeto tem como objetivo **analisar dados de clientes da Telecom X para prever o churn (cancelamento de serviço)** utilizando técnicas de análise de dados e aprendizado de máquina.

A análise busca identificar **quais fatores influenciam a saída de clientes**, permitindo que a empresa desenvolva estratégias de retenção mais eficazes.

---

# 🎯 Objetivo Principal

Construir um modelo capaz de **prever a probabilidade de churn de clientes** com base em variáveis demográficas, de uso do serviço e de faturamento.

Com isso, a empresa pode:

* Identificar clientes com alto risco de cancelamento
* Criar campanhas de retenção direcionadas
* Melhorar a experiência do cliente

---

# 📂 Estrutura do Projeto

```
TelecomX-Churn-Analysis/
│
├── data/
│   ├── telecomx_dados_tratados.csv
│
├── notebooks/
│   └── TelecomX_Analise_Churn.ipynb
│
├── visualizations/
│   ├── churn_distribution.png
│   ├── correlation_heatmap.png
│
└── README.md
```

### Descrição dos Arquivos

* **data/** → contém os dados já tratados utilizados na modelagem.
* **notebooks/** → notebook principal com toda a análise.
* **visualizations/** → gráficos gerados durante a análise exploratória.
* **README.md** → documentação do projeto.

---

# 🧹 Preparação dos Dados

## 1️⃣ Classificação das Variáveis

As variáveis foram separadas em dois tipos principais:

### Variáveis Categóricas

Exemplos:

* gênero
* tipo de contrato
* método de pagamento
* presença de serviços adicionais
* churn (variável alvo)

### Variáveis Numéricas

Exemplos:

* tempo de contrato
* valor mensal
* valor total pago

---

## 2️⃣ Tratamento de Dados

As seguintes etapas foram realizadas:

* Remoção de valores ausentes
* Conversão de tipos de dados
* Padronização de variáveis categóricas

---

## 3️⃣ Codificação das Variáveis

Variáveis categóricas foram convertidas para formato numérico utilizando:

* **One-Hot Encoding**

Isso permite que os algoritmos de machine learning utilizem essas variáveis corretamente.

---

## 4️⃣ Normalização dos Dados

Variáveis numéricas foram normalizadas para evitar que variáveis com escalas maiores influenciem excessivamente o modelo.

Foi utilizada padronização para colocar os dados em escalas comparáveis.

---

## 5️⃣ Separação Treino e Teste

O conjunto de dados foi dividido em:

* **Treino:** 80%
* **Teste:** 20%

Essa divisão permite avaliar o desempenho do modelo em dados que ele **nunca viu antes**.

---

# 🤖 Modelagem

Foram testados modelos de classificação para prever churn.

As escolhas de modelagem foram baseadas em:

* Interpretabilidade do modelo
* Capacidade de generalização
* Desempenho em métricas como:

  * Accuracy
  * Precision
  * Recall
  * F1-score

O objetivo é identificar **clientes com maior probabilidade de cancelar o serviço**.

---

# 📊 Análise Exploratória de Dados (EDA)

Durante a análise exploratória, diversos insights importantes foram identificados.

### Exemplos de análises realizadas:

* Distribuição de clientes com e sem churn
* Correlação entre variáveis numéricas
* Comparação entre tipo de contrato e taxa de churn
* Impacto do valor mensal no cancelamento

### Exemplos de gráficos utilizados

* Gráficos de barras para distribuição de churn
* Heatmap de correlação
* Histogramas para variáveis numéricas
* Boxplots para identificar padrões de churn

### Insights Obtidos

Alguns padrões observados:

* Clientes com **contratos mensais** apresentam maior probabilidade de churn.
* Valores mensais mais altos estão associados a maior risco de cancelamento.
* Clientes com **maior tempo de contrato** tendem a permanecer mais na empresa.

---

# ▶️ Como Executar o Projeto

## 1️⃣ Clonar o Repositório

```bash
git clone https://github.com/seu-usuario/telecomx-churn-analysis.git
```

---

## 2️⃣ Instalar as Bibliotecas Necessárias

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

---

## 3️⃣ Executar o Notebook

Abra o notebook com:

```bash
jupyter notebook
```

Depois abra o arquivo:

```
TelecomX_Analise_Churn.ipynb
```

---

# 📈 Resultados Esperados

Ao executar o notebook você poderá:

* Explorar os dados da Telecom X
* Visualizar gráficos da análise exploratória
* Treinar modelos de previsão de churn
* Avaliar o desempenho dos modelos

---

# 👨‍💻 Autor

Projeto desenvolvido como parte de um desafio de **análise de dados e machine learning**.

---
