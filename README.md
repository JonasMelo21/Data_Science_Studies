# 🧠 Data Science Studies

📝 *This README is available in English and Portuguese.*  
👉 **[Click here to jump to the Portuguese version](#-estudos-em-ciência-de-dados)**  
or scroll down to continue in English.

---

## 📚 Focus Areas

This repository documents my Data Science journey, with emphasis on:

- 🧼 Robust data cleaning and preprocessing  
- 📊 Exploratory analysis and statistical interpretation  
- 🤖 Supervised machine learning with critical thinking  
- 🧠 Learning from mistakes and validation procedures  

---

## ⚡ Project Highlights

### ✅ [Project 01: Student Performance Classification](#-project-01-student-performance-classification)  
📌 **Supervised classification with critical label correction and safe SMOTE application.**  
I manually corrected mislabeled target values (present in the original Kaggle dataset), applied SMOTE only after the data split, and built solid pipelines that achieved **96% accuracy and macro F1-score**.  
🔗 **[Notebook → projeto1.ipynb](projeto1.ipynb)**

---

### 🚨 [Project 02: Churn Prediction with Statistical Testing + MLP](#-project-02-churn-prediction-with-eda-statistical-tests--neural-networks)  
📌 **Combination of inferential statistics and neural networks.**  
I applied hypothesis tests (Chi-square, Mann-Whitney, Kruskal-Wallis) before modeling to validate business assumptions and improve interpretability.  
🔗 **[Notebook → projeto2.ipynb](projeto2.ipynb)**

---

### 🏙️ [Project 03: Rent Price Prediction with Regression & Classification](#-project-03-rent-price-prediction-with-regression--classification)  
📌 **Linear regression and interpretable classification based on real-world housing features.**  
Achieved **R² of 0.82** and classified listings as "cheap or expensive" with **84% accuracy**, using real estate attributes like size, rooms, garage, and distance from city center.  
🔗 **[Notebook → projeto3.ipynb](projeto3.ipynb)**

---

Claro! Abaixo está a seção **“📁 Detailed Projects”** completa — primeiro em **inglês**, depois em **português**. Ela já está com os títulos em formato de âncoras para funcionar com os links internos do sumário. Basta colar isso no lugar da parte comentada como `<!-- detailed sections omitted for brevity -->`:

---

### 📁 Detailed Projects (English)

---

### 🧪 Project 01: Student Performance Classification

🔗 **[Notebook → projeto1.ipynb](projeto1.ipynb)**

> Supervised classification based on educational data (age, ethnicity, absences, etc.) with careful preprocessing and decision-making.

**🌟 Highlights:**

* Corrected a **critical labeling issue** in the `GradeClass` column from the original dataset.
* Tackled heavy class imbalance using **SMOTE**, applied *after* the split to avoid leakage.
* Built a robust pipeline focused on bias reduction and generalization.

**📊 Results:**

* **Accuracy:** 96%
* **Macro F1-score:** 0.96
* **Stable performance**, even on unbalanced data.

---

### 🧠 Project 02: Churn Prediction with EDA, Statistical Tests & Neural Networks

🔗 **[Notebook → projeto2.ipynb](projeto2.ipynb)**

> Integrated inferential statistics with neural networks to ensure **performance + interpretability** in churn modeling.

**🔬 Hypothesis Testing:**

* Chi-square → 📌 Gender influences churn
* Mann-Whitney → 📌 Salary has **no** significant effect
* Kruskal-Wallis → 📌 Number of products has nonlinear relationship with churn

**🤖 Modeling with MLP:**

* Multi-layer perceptron with **ReLU** and **sigmoid**
* **Adam optimizer**, **Binary Crossentropy** loss
* Data normalized and balanced with SMOTE

**📈 Results:**

* **Accuracy:** 82%
* **F1-score:** 59%
* **Recall:** 67%
* **Precision:** 54%

**💡 Key Insights:**

* Age > 40 → 2x higher churn risk
* German customers had higher churn rates
* High balance and inactivity were strong churn indicators

---

### 🏠 Project 03: Rent Price Prediction with Regression & Classification

🔗 **[Notebook → projeto3.ipynb](projeto3.ipynb)**

> Price estimation and classification of rental listings based on real-world apartment data (area, rooms, bathrooms, garage, distance from downtown).

**🔍 EDA Highlights:**

* **Area (m²)** has strong positive effect on price
* **Distance to city center** has a negative correlation
* Model produced useful, intuitive coefficients

**📉 Regression Results:**

* **MAE:** R\$158.61
* **R² Score:** 0.82
* **Coefficients:**

  * +R\$24.03/m²
  * +R\$123.95 per room
  * +R\$101.11 per bathroom
  * +R\$196.86 if garage exists
  * –R\$51.10 per km away from center

**📊 Classification Results:**

* **Accuracy:** 84%
* **Precision:** 87%
* **Recall:** 83%
* ⚠️ 18 false negatives (expensive apartments classified as cheap)

**🚧 Improvements Suggested:**

* Feature engineering
* Outlier treatment
* More robust models (Random Forest, SVM, Gradient Boosting)


---

# 🇧🇷 Estudos em Ciência de Dados

📝 *Este README está disponível em inglês e português.*  
👉 **[Clique aqui para voltar ao topo (versão em inglês)](#-data-science-studies)**  
ou continue lendo em português.

---

## 📚 Áreas de Foco

Este repositório documenta meus estudos em Ciência de Dados, com foco em:

- 🧼 Limpeza e pré-processamento robusto  
- 📊 Análise exploratória e validação estatística  
- 🤖 Modelagem supervisionada com raciocínio crítico  
- 🧠 Aprendizado com validações e erros  

---

## ⚡ Visão Geral dos Projetos

### ✅ [Projeto 01: Classificação da Performance de Estudantes](#-projeto-01-classificação-da-performance-de-estudantes)  
📌 **Classificação supervisionada com correção crítica de rótulos e SMOTE aplicado de forma segura.**  
Corrigi manualmente os rótulos da variável alvo (que estavam errados no Kaggle), apliquei SMOTE após o split e construí pipelines limpas que resultaram em **96% de acurácia e F1-score macro**.  
🔗 **[Notebook → projeto1.ipynb](projeto1.ipynb)**

---

### 🚨 [Projeto 02: Previsão de Churn com Testes Estatísticos e MLP](#-projeto-02-previsão-de-churn-com-eda-testes-estatísticos-e-rede-neural)  
📌 **Integração de testes estatísticos com rede neural supervisionada.**  
Utilizei testes como Qui-quadrado, Mann-Whitney e Kruskal-Wallis antes de treinar uma MLP, garantindo **decisões interpretáveis e validadas**.  
🔗 **[Notebook → projeto2.ipynb](projeto2.ipynb)**

---

### 🏙️ [Projeto 03: Previsão de Preço de Aluguel com Regressão e Classificação](#-projeto-03-previsão-de-aluguel-com-regressão-linear-e-classificação)  
📌 **Regressão linear e classificação interpretável baseada em variáveis reais de imóveis.**  
Obtive **R² de 0.82** e classifiquei os imóveis como “caros ou baratos” com **84% de acurácia**, com base em características como metragem, quartos, garagem e distância do centro.  
🔗 **[Notebook → projeto3.ipynb](projeto3.ipynb)**

---


## 📁 Projetos Detalhados

---

### 🧪 Projeto 01: Classificação da Performance de Estudantes  
🔗 **[Notebook → projeto1.ipynb](projeto1.ipynb)**

> Classificação baseada em dados educacionais (idade, etnia, faltas, etc.), com foco em decisões bem fundamentadas desde o pré-processamento.

**🌟 Destaques:**

- Corrigi um **erro do dataset original** na coluna `GradeClass`, que rotulava mal alunos com GPA baixo  
- Usei **SMOTE com segurança**, após o split, evitando vazamento  
- Construi pipeline robusto e interpretável

**📊 Resultados:**

- **Acurácia:** 96%  
- **F1-score (macro):** 0.96  
- Estabilidade mesmo com dados desbalanceados

---

### 🧠 Projeto 02: Previsão de Churn com EDA, Testes Estatísticos e Rede Neural  
🔗 **[Notebook → projeto2.ipynb](projeto2.ipynb)**

> Predição de churn usando inferência estatística e MLP com foco em **confiabilidade e explicabilidade**.

**🔬 Testes aplicados:**

- Qui-quadrado → 📌 Gênero influencia no churn  
- Mann-Whitney → 📌 Salário **não** tem impacto significativo  
- Kruskal-Wallis → 📌 Número de produtos tem relação com churn

**🤖 Modelagem:**

- MLP com ReLU e saída Sigmoid  
- Otimizador Adam, Binary Crossentropy  
- SMOTE + normalização dos dados

**📈 Resultados:**

- **Acurácia:** 82%  
- **F1-score:** 59%  
- **Recall:** 67%  
- **Precisão:** 54%

**💡 Insights práticos:**

- Idade > 40 dobra o risco de churn  
- Clientes da Alemanha saem mais  
- Clientes inativos com saldo alto têm maior chance de sair

---

### 🏠 Projeto 03: Previsão de Aluguel com Regressão Linear e Classificação  
🔗 **[Notebook → projeto3.ipynb](projeto3.ipynb)**

> Estimativa do preço do aluguel e classificação de imóveis como **caros ou baratos**.

**🔍 Descobertas da EDA:**

- Área do imóvel impacta positivamente  
- Distância do centro impacta negativamente  
- Coeficientes intuitivos e úteis

**📉 Resultados da Regressão:**

- **MAE:** R$158,61  
- **R²:** 0.82  
- **Coeficientes:**
  - +R$24,03/m²  
  - +R$123,95/quarto  
  - +R$101,11/banheiro  
  - +R$196,86 com garagem  
  - –R$51,10/km do centro

**📊 Resultados da Classificação:**

- **Acurácia:** 84%  
- **Precisão:** 87%  
- **Recall:** 83%  
- ⚠️ 18 falsos negativos → imóveis caros classificados como baratos

**🚧 Melhorias futuras:**

- Engenharia de atributos  
- Tratamento de outliers  
- Testar modelos robustos (Random Forest, SVM, Gradient Boosting)

---

📌 *Novos projetos em breve, com foco em desafios reais, rigor estatístico e alto valor analítico.*
