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

### 📉 Gráfico: Previsão vs Valor Real (Regressão Linear)

Este gráfico de dispersão compara os valores **previstos pelo modelo de regressão linear** (eixo Y) com os **valores reais observados** no conjunto de teste (eixo X).  
A linha vermelha pontilhada representa a **linha ideal de previsão perfeita** — onde previsão e realidade seriam idênticas.

🔎 **Quanto mais próximos os pontos estiverem dessa linha, melhor a performance do modelo.**

📊 Neste caso, o modelo obteve um bom desempenho, com as previsões concentradas em torno da linha, especialmente nas faixas de menor gasto.  
Em valores mais altos, há uma leve tendência de subestimativa — algo esperado em modelos lineares aplicados a dados com grande variabilidade nos extremos.

![Captura de tela 2025-04-18 163429](https://github.com/user-attachments/assets/977573fc-aa19-45fa-90c9-7e9c51c98427)

### 📊 Gráfico: Dispersão entre IMC e Gastos com Saúde

Este gráfico mostra a relação entre o **Índice de Massa Corporal (IMC)** dos pacientes (eixo X) e os **gastos anuais com plano de saúde** (eixo Y).

📌 Embora exista uma concentração de maiores gastos em pacientes com IMC acima de 30, a dispersão é ampla — indicando que o IMC **sozinho não explica totalmente os altos custos**.

🔍 O gráfico sugere que, apesar de uma leve tendência positiva, existem muitos pacientes com IMC elevado e baixo custo, e vice-versa.

➡️ Isso reforça a importância de considerar **várias variáveis em conjunto**, como foi feito na regressão linear múltipla.

![Captura de tela 2025-04-18 163750](https://github.com/user-attachments/assets/582b14fa-8eda-4990-bda4-4bf09bf3bf97)

### 🚬 Gráfico: Impacto do Fumo nos Custos de Saúde

Este gráfico de barras compara o **gasto médio anual com plano de saúde** entre **fumantes** e **não fumantes**, em dólares.

📊 A diferença é expressiva: fumantes apresentaram um gasto médio acima de **$32.000**, enquanto não fumantes ficaram próximos de **$8.400**.

🔥 Esse contraste evidencia o **alto custo financeiro associado ao tabagismo**, mesmo antes de considerar complicações clínicas mais graves.

➡️ Esse foi um dos insights mais fortes do projeto e foi validado tanto na análise exploratória quanto na regressão linear múltipla.

![Captura de tela 2025-04-18 163903](https://github.com/user-attachments/assets/d5e0df30-8627-4ae5-b322-9c6871b0346e)

### 📉 Gráfico: Resíduos da Regressão Linear

Este gráfico mostra a distribuição dos **resíduos do modelo**, ou seja, a diferença entre os valores **reais** e os **previstos** (Erro = Real − Previsto).

🔍 A linha vermelha representa o ponto ideal onde o erro é zero.  
Pontos acima dela indicam que o modelo **subestimou o valor real** (errou pra menos), enquanto pontos abaixo indicam que **superestimou** (errou pra mais).

📊 A maioria dos resíduos se concentra entre **-5.000 e +5.000**, alinhando-se com as métricas MAE (~3.900) e RMSE (~5.600) obtidas na avaliação.

➡️ A dispersão dos resíduos é relativamente homogênea e sem padrão aparente, o que indica que o modelo não possui viés sistemático e está fazendo previsões consistentes para diferentes faixas de valor.

![Captura de tela 2025-04-18 164256](https://github.com/user-attachments/assets/2598a2c3-7a80-4f9e-93fc-34a6363e261a)


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

Matheus Guimarães – [linkedin.com/in/MatheusGuimaraes007](https://github.com/MatheusGuimaraes007)




