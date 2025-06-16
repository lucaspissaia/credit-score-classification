# 📊 Credit Score Classification - Projeto de Machine Learning

Este projeto foi desenvolvido como parte do módulo de Machine Learning do MBA em Data Science & AI da FIAP, em parceria com a Quantum Finance.

## Desafio

O objetivo era construir um modelo de classificação de score de crédito usando dados reais disponibilizados no Kaggle (https://www.kaggle.com/datasets/parisrohan/credit-score-classification)).

A ideia é aplicar técnicas de tratamento de dados, engenharia de variáveis e machine learning para prever a categoria de score de crédito de novos clientes: `Good`, `Standard` ou `Poor`.

---

## Tecnologias e Ferramentas

- PySpark e Pandas para ingestão e tratamento de dados
- Winsorização, One-Hot Encoding, remoção de multicolinearidade
- Modelos supervisionados: `Random Forest`, `XGBoost` e `LightGBM`
- `StandardScaler`, `GridSearchCV`, `classification_report` do scikit-learn

---

## Etapas principais do projeto

1. **Importação e configuração**
2. **Leitura e limpeza de dados com PySpark**
3. **Tratamento da coluna `Credit_History_Age`**
4. **Análise e execução de One-Hot Encoding**
5. **Winsorização e matriz de correlação**
6. **Modelagem com RandomForest, XGBoost, LightGBM**
7. **Conversão para Pandas e refino com `StandardScaler` e `GridSearchCV`**
8. **Validação e aplicação em novo conjunto de dados**

---

## Resultados

**Melhor modelo:** `Random Forest`  
- Acurácia: **79%**
- Recall por classe:
  - Good: 0.74
  - Poor: 0.82
  - Standard: 0.80

**Outros modelos:**
- XGBoost: acurácia 75%
- LightGBM: acurácia 77%

Apesar do desequilíbrio entre classes, o Random Forest mostrou-se mais equilibrado, com bom desempenho geral.

---

## Aplicação prática

O modelo pode apoiar decisões reais de crédito na Quantum Finance, como:

- Análise de risco e inadimplência
- Segmentação por score de crédito
- Otimização de concessão de crédito e juros personalizados

---

## Equipe

- Lucas Huber Pissaia  
- Erika Koyanagui  
- Fabio Asnis  
- Matheus Raeski  

---

## Acesse o notebook no Colab

[🔗 Notebook no Google Colab](https://colab.research.google.com/drive/1RYIIZ2knT8HGol7it99PO4bwtMAQk0PL)

---

*Projeto desenvolvido como parte do MBA em Data Science & AI - FIAP - 2025*
