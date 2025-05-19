
# 📊 Análise de Evasão de Clientes (Churn)

Este projeto tem como objetivo analisar dados de clientes de uma empresa de telecomunicações e identificar padrões associados à evasão de clientes (churn), utilizando técnicas de análise exploratória de dados e visualização.

---

## 🧭 Objetivo

Entender o comportamento de cancelamento de clientes (churn), identificar variáveis mais associadas à evasão e gerar insights acionáveis que possam ajudar a reduzir o churn.

---

## 📥 Dados

O conjunto de dados foi fornecido no formato JSON, com múltiplas colunas aninhadas (como `customer`, `phone`, `internet`, `account`) e inclui informações sobre:

- Perfil demográfico do cliente
- Serviços contratados
- Informações contratuais e de pagamento
- Valor faturado mensal e total

---

## 🧹 Limpeza e Pré-processamento

- Normalização de colunas aninhadas usando `pd.json_normalize`
- Conversão de valores "Yes"/"No" em `1` e `0`
- Tratamento de valores vazios e conversão de tipos (`float`, `int`)
- Criação de variáveis derivadas:
  - `Contas_Diarias`: gasto mensal dividido por 30
  - `Total_Servicos`: soma de todos os serviços contratados

---

## 📊 Análise Exploratória

- Visualização da distribuição de churn (pizza e barras)
- Comparação de churn por variáveis categóricas:
  - Gênero
  - Tipo de contrato
  - Forma de pagamento
  - Tipo de internet
- Estatísticas descritivas: média, mediana, desvio padrão, assimetria e curtose
- Correlação entre variáveis numéricas com `Churn`

---

## 🔍 Principais Insights

- Contratos do tipo `Month-to-month` têm maior evasão
- Pagamentos por `Electronic check` estão associados a mais cancelamentos
- Clientes com menos serviços contratados são mais propensos ao churn
- Valor diário da conta (Contas_Diarias) mostra correlação leve com churn

---

## ✅ Recomendações

1. Criar incentivos para planos anuais ou bienais
2. Melhorar a experiência dos clientes que usam pagamento eletrônico
3. Oferecer pacotes promocionais para incentivar múltiplos serviços
4. Usar essas análises para treinar modelos preditivos de churn

---

## 📁 Execução

Todo o projeto foi desenvolvido e documentado em um [Jupyter Notebook](./Relatorio_Final_Churn.ipynb), com visualizações interativas utilizando `Plotly`.

---

## 📌 Autor

Ricardo Bueno — Projeto de Data Science com foco em retenção de clientes e aprendizado prático com análise de dados reais Alura ONE.
