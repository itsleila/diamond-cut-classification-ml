# 💎 Diamond Cut Classification com Machine Learning

Este projeto tem como objetivo desenvolver e comparar diferentes modelos de **Machine Learning** para classificar a **qualidade do corte de diamantes (`cut`)**, utilizando um conjunto de dados público com características físicas e qualitativas das gemas.

O trabalho envolve todas as etapas de um **pipeline completo de ciência de dados**, incluindo:

- Pré-processamento
- Engenharia de atributos
- Treinamento de modelos
- Otimização de hiperparâmetros
- Avaliação de desempenho
- Interpretabilidade com LIME

## Objetivo

Construir modelos capazes de **classificar corretamente a qualidade do corte do diamante (`cut`)**, comparando o desempenho de diferentes algoritmos:

- Decision Tree
- Random Forest
- XGBoost
- Support Vector Machine (SVM)

Além disso, aplicar técnicas de:

- **Otimização de hiperparâmetros (GridSearch)**
- **Interpretabilidade com LIME**
- **Análise de importância das variáveis (Feature Importance)**

## 🗂 Dataset

Base de dados utilizada:  
**CDC Behavioral Risk Factor Surveillance – Diamonds Dataset**
Link direto: [diamonds.csv](https://raw.githubusercontent.com/cassiusf/datasets/main/diamonds.csv)

### Características da base:

- **53.940 observações**
- **10 variáveis**

## Pipeline do Projeto

1. Carregamento dos dados diretamente do GitHub
2. Limpeza e pré-processamento

- Criação de variáveis dummy (`clarity` e `color`)
- Recodificação da variável alvo (`cut`)
- Normalização dos dados
- Separação treino/teste (75% / 25%)

3. Treinamento dos modelos:
   - Decision Tree
   - Random Forest
   - XGBoost
   - SVM
4. Avaliação com:
   - Matriz de confusão
   - Classification Report
5. GridSearch para:
   - Random Forest
   - SVM
6. Interpretação:
   - Feature Importance
   - LIME

## Tecnologias Utilizadas

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- LIME

## Modelos Avaliados

| Modelo        | Descrição                   |
| ------------- | --------------------------- |
| Decision Tree | Árvore de decisão simples   |
| Random Forest | Ensemble de árvores         |
| XGBoost       | Gradient Boosting otimizado |
| SVM           | Support Vector Machine      |

### Avaliação

Os modelos foram avaliados utilizando:

- **Matriz de Confusão**
- **Relatório de Classificação**
  - Acurácia
  - Precisão
  - Recall
  - F1-score

A métrica principal utilizada para otimização foi **acurácia**.

### Resultados

O modelo XGBoost, utilizando os parâmetros padrão, apresentou o melhor desempenho geral, atingindo 80% de acurácia, além de excelente equilíbrio entre precisão e recall nas diferentes classes.
