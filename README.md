# Tópicos Especiais em TI — Exemplos Reais de Machine Learning com Dados do Kaggle

Este repositório reúne **4 exemplos práticos de Ciência de Dados e Machine Learning**, cada um
aplicado a um **dataset real do Kaggle**, cobrindo as principais técnicas fundamentais da área:

| # | Pasta | Técnica | Dataset (Kaggle) |
|---|-------|---------|-------------------|
| 1 | [`01-clusterizacao-segmentacao-clientes`](01-clusterizacao-segmentacao-clientes) | Clusterização (K-Means) | [Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) |
| 2 | [`02-regressao-linear-expectativa-vida`](02-regressao-linear-expectativa-vida) | Regressão Linear | [Life Expectancy (WHO)](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who) |
| 3 | [`03-classificacao-naive-bayes-diabetes`](03-classificacao-naive-bayes-diabetes) | Classificação (Naive Bayes) | [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) |
| 4 | [`04-classificacao-logistica-insuficiencia-cardiaca`](04-classificacao-logistica-insuficiencia-cardiaca) | Classificação (Regressão Logística) | [Heart Failure Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction) |

## Estrutura de cada pasta

Cada pasta contém:
- Um notebook Jupyter (`.ipynb`) já executado, com todo o código, gráficos e resultados;
- O arquivo `.csv` com os dados reais utilizados.

## Como executar

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook
```

Depois é só abrir o notebook desejado e rodar as células (`Kernel > Restart & Run All`).

## Resumo dos resultados

- **Segmentação de clientes:** o método do cotovelo e o Silhouette Score confirmaram **K = 5**
  como o número ideal de clusters (Silhouette Score ≈ 0.55), revelando 5 perfis distintos de
  clientes por renda e comportamento de gasto.
- **Regressão Linear (Expectativa de Vida):** modelo atingiu **R² ≈ 0.81** (RMSE ≈ 3.8 anos),
  mostrando que Mortalidade Adulta e HIV/AIDS reduzem a previsão, enquanto Escolaridade e
  Índice de Composição de Renda a aumentam.
- **Diabetes (Naive Bayes):** modelo GaussianNB, após tratamento de dados ausentes disfarçados
  de zero, atingiu **~72% de acurácia** na previsão de diagnóstico.
- **Insuficiência Cardíaca (Regressão Logística):** modelo atingiu **~85% de acurácia** e boa
  área sob a curva ROC (AUC), com ST_Slope, ChestPainType e ExerciseAngina entre as variáveis
  mais influentes.

## Autoria

Jose Gustavo Martinho Araujo de Almeida

Projeto desenvolvido para a disciplina de **Tópicos Especiais em TI**, com exemplos reais
utilizando datasets públicos do [Kaggle](https://www.kaggle.com/datasets).
