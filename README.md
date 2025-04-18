# 🩺 Previsão de Gastos com Saúde utilizando Regressão Linear Múltipla

Este projeto tem como objetivo utilizar **Regressão Linear Múltipla** para prever o gasto anual de pacientes com planos de saúde, com base em variáveis demográficas e comportamentais.  
A análise foi realizada sobre um **dataset público**, amplamente utilizado em estudos introdutórios de Machine Learning.

---

## 📚 Objetivo

- Explorar o impacto de variáveis como **idade**, **IMC**, **número de filhos**, **hábito de fumar** e **região** nos custos com saúde.
- Avaliar a capacidade de um modelo linear em **prever os gastos** com base nesses fatores.

---

## 🧪 Metodologia

1. Importação e análise inicial do dataset
2. Transformação de variáveis categóricas binárias (`smoker`, `sex`)
3. Aplicação de **One-Hot Encoding** na variável `region`
4. Separação do dataset em **treino (80%) e teste (20%)**
5. Treinamento com **Regressão Linear Múltipla**
6. Geração de previsões com os dados de teste
7. Avaliação do modelo com métricas: **R²**, **RMSE** e **MAE**
8. Comparação entre valores reais e previstos
9. Análise dos coeficientes das variáveis

---

## 📈 Principais Insights

- 🔥 **Fumar tem um impacto brutal**: o fumante que menos gastou ainda superou a **média dos não fumantes**.
- 📊 O **fator “fumante” foi o mais relevante** na regressão, com coeficiente mais alto que idade, IMC ou filhos.
- 📉 O **IMC mostrou alguma correlação** com os custos, mas isoladamente não explica gastos elevados.
- ✅ O modelo alcançou um **R² superior a 0.80**, mostrando bom poder preditivo.

---

## 🖼️ Imagens do Projeto

![Captura de tela 2025-04-18 163429](https://github.com/user-attachments/assets/977573fc-aa19-45fa-90c9-7e9c51c98427)

---

## ⚙️ Tecnologias utilizadas

- Python
- Pandas, NumPy, Matplotlib
- Scikit-learn (Regressão Linear, OneHotEncoder, ColumnTransformer)

---

## 🚀 Conclusão

Este projeto demonstrou como a regressão linear múltipla pode ser aplicada para identificar padrões de gastos em saúde com base em variáveis simples.  
Mais do que prever, a análise serviu para revelar **padrões ocultos e impactos concretos de hábitos como o tabagismo nos custos pessoais.**

---

## 📂 Dataset

Disponível publicamente em: [Kaggle - Insurance Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)

---

## 🧑‍💻 Autor

Luis Kempe – [linkedin.com/in/luiskempe](https://linkedin.com/in/luiskempe)

