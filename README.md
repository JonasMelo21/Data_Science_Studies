# 🧠 Data Science Studies

📝 *This README is available in English and Portuguese.*  
📌 [Click here to read in Portuguese.](#-estudos-em-ciência-de-dados)

---

## 📚 Focus Areas

This repository documents my Data Science journey, with emphasis on:

- 🧼 Robust data cleaning and preprocessing  
- 📊 Exploratory analysis and statistical validation (hipotesis tests)  
- 🤖 Supervised machine learning with critical thinking  
- 🧠 Learning from mistakes and validation procedures  

---

## ⚡ Project Highlights (Click on the title of the project to be redirected to more detailed description of the project)

### ✅ [Project 01: Student Performance Classification(Click here for more information on the project such as metrics,approach,etc...)](#-project-01-student-performance-classification-1)  
📌 **Supervised classification with critical label correction and safe SMOTE application.**  
I manually corrected mislabeled target values (present in the original Kaggle dataset), applied SMOTE only after the data split, and built solid pipelines that achieved **96% accuracy and macro F1-score**.  
🔗 **[Notebook → projeto1.ipynb](projeto1.ipynb)**

---

### 🚨 [Project 02: Churn Prediction with Statistical Testing + MLP (Click here for more information on the project such as metrics,approach,etc...)](#-project-02-churn-prediction-with-eda-statistical-tests--neural-networks)  
📌 **Combination of inferential statistics and neural networks.**  
I applied hypothesis tests (Chi-square, Mann-Whitney, Kruskal-Wallis) before modeling to validate business assumptions and improve interpretability.  
🔗 **[Notebook → projeto2.ipynb](estudo_caso_5_churn.ipynb)**

---

### 🏙️ [Project 03: Rent Price Prediction with Regression & Classification(Click here for more information on the project such as metrics,approach,etc...)](#-project-03-rent-price-prediction-with-regression--classification)  
📌 **Linear regression and interpretable classification based on real-world housing features.**  
Achieved **R² of 0.82** and classified listings as "cheap or expensive" with **84% accuracy**, using real estate attributes like size, rooms, garage, and distance from city center.  
🔗 **[Notebook → projeto3.ipynb](projeto3.ipynb)**

---

## 📁 Detailed Projects

### 🧪 Project 01: Student Performance Classification  
🔗 **[Notebook → projeto1.ipynb](projeto1.ipynb)**

> Supervised classification task using educational data (age, race, GPA, etc.), with a strong focus on data cleaning and class balance.

**🌟 Key Points:**

- Fixed **target labeling issues** in the `GradeClass` column  
- Applied **SMOTE after train-test split** to avoid data leakage  
- Built a clean and interpretable pipeline

**📊 Results:**

- **Accuracy:** 96%  
- **Macro F1-score:** 0.96  
- High generalization even under imbalance

---

### 🧠 Project 02: Churn Prediction with EDA, Statistical Tests & Neural Networks  
🔗 **[Notebook → projeto2.ipynb](estudo_caso_5_churn.ipynb)**

> Used statistical inference and MLPs to predict customer churn while ensuring explainability.

**🔬 Statistical Tests:**

- Chi-square → 📌 Gender influences churn  
- Mann-Whitney → 📌 Salary has **no** significant impact  
- Kruskal-Wallis → 📌 Product count is related to churn

**🤖 Modeling:**

- MLP with ReLU hidden layers and Sigmoid output  
- Adam optimizer, Binary Crossentropy loss  
- SMOTE balancing and normalized features

**📈 Results:**

- **Accuracy:** 82%  
- **F1-score:** 59%  
- **Recall:** 67%  
- **Precision:** 54%

**💡 Insights:**

- Age > 40 doubles churn risk  
- German clients churn more  
- Inactive users with high balances are more likely to leave

---

### 🏠 Project 03: Rent Price Prediction with Regression & Classification  
🔗 **[Notebook → projeto3.ipynb](projeto3.ipynb)**

> Estimated apartment rental prices and built a binary classifier for "cheap vs expensive".

**🔍 Key Insights from EDA:**

- Apartment size has a strong positive impact  
- Distance from downtown has negative impact  
- Coefficients are easy to interpret and useful

**📉 Regression Results:**

- **MAE:** R$158.61  
- **R²:** 0.82  
- **Coefficients:**
  - +R$24.03/m²
  - +R$123.95/room
  - +R$101.11/bathroom
  - +R$196.86 for garage
  - –R$51.10/km from city center

**📊 Classification Results:**

- **Accuracy:** 84%  
- **Precision:** 87%  
- **Recall:** 83%  
- ⚠️ 18 false negatives → Expensive rentals classified as cheap

**🚧 Next Steps:**

- Feature engineering  
- Outlier handling  
- Try advanced models (Random Forest, SVM, Gradient Boosting)

---

# 🇧🇷 Estudos em Ciência de Dados

📌 [Clique aqui para voltar ao topo em inglês.](#-data-science-studies)

---

## 📚 Áreas de Foco

Este repositório documenta meus estudos em Ciência de Dados, com foco em:

- 🧼 Limpeza e pré-processamento robusto  
- 📊 Análise exploratória e validação estatística(testes de hipótese)  
- 🤖 Modelagem supervisionada com raciocínio crítico  
- 🧠 Aprendizado com validações e erros

---

## ⚡ Visão Geral dos Projetos (Clique no subtítulo do projeto para ser direcionado a mais detalhes)

### ✅ [Projeto 01: Classificação da Performance de Estudantes(Clique aqui para mais detalhes)](https://github.com/JonasMelo21/Data_Science_Studies?tab=readme-ov-file#-project-01-student-performance-classification)  
📌 **Classificação supervisionada com correção crítica de rótulos e SMOTE aplicado de forma segura.**  
Corrigi manualmente os rótulos da variável alvo (que estavam errados no Kaggle), apliquei SMOTE após o split e construí pipelines limpas que resultaram em **96% de acurácia e F1-score macro**.  
🔗 **[Notebook → projeto1.ipynb](projeto1.ipynb)**

---

### 🚨 [Projeto 02: Previsão de Churn com Testes Estatísticos e MLP(Clique aqui para mais detalhes do projeto)](#-projeto-02-previs%C3%A3o-de-churn-com-eda-testes-estat%C3%ADsticos-e-rede-neural)  
📌 **Integração de testes estatísticos com rede neural supervisionada.**  
Utilizei testes como Qui-quadrado, Mann-Whitney e Kruskal-Wallis antes de treinar uma MLP, garantindo **decisões interpretáveis e validadas**.  
🔗 **[Notebook → projeto2.ipynb](projeto2.ipynb)**

---

### 🏙️ [Projeto 03: Previsão de Preço de Aluguel com Regressão e Classificação(Clique aqui para mais detalhes do projeto)](#-projeto-03-previs%C3%A3o-de-aluguel-com-regress%C3%A3o-linear-e-classifica%C3%A7%C3%A3o) 
📌 **Regressão linear e classificação interpretável baseada em variáveis reais de imóveis.**  
Obtive **R² de 0.82** e classifiquei os imóveis como “caros ou baratos” com **84% de acurácia**, com base em características como metragem, quartos, garagem e distância do centro.  
🔗 **[Notebook → projeto3.ipynb](projeto3.ipynb)**

---

## 📁 Projetos Detalhados

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
