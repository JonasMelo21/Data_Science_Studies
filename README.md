# 📚 Estudos em Ciência de Dados

Repositório dos meus estudos em **Ciência de Dados**, com foco em:

- 🧼 Limpeza e pré-processamento de dados
- 📊 Análise exploratória e interpretação estatística
- 🤖 Modelos supervisionados com raciocínio crítico
- 🧠 Aprendizado a partir de erros e validações

---

## ⚡ Visão Geral dos Projetos

### ✅ Projeto 01: Classificação da Performance de Estudantes  
📌 **Classificação supervisionada com foco em limpeza de dados e correção de erro crítico no dataset original.**  
Corrigi manualmente os rótulos da variável alvo, que estavam errados no próprio Kaggle, usei SMOTE de forma segura (após o split) e obtive **96% de acurácia e F1-score macro de 0.96**, com desempenho equilibrado nas classes.

### 🚨 Projeto 02: Previsão de Churn com Testes Estatísticos e Rede Neural  
📌 **Combinação de estatística inferencial com machine learning supervisionado.**  
Usei testes como Qui-quadrado, Mann-Whitney e Kruskal-Wallis para validar hipóteses de negócio antes de treinar uma MLP. O projeto mostra capacidade de transformar dados em decisões orientadas e interpretáveis.

### 🏙️ Projeto 03: Previsão de Preço de Aluguel com Regressão Linear e Classificação  
📌 **Análise de impacto de variáveis reais (área, garagem, distância do centro) sobre o preço de aluguel.**  
O modelo atingiu **R² de 0.82** e gerou coeficientes interpretáveis. Também classifiquei se o imóvel está "caro ou barato", com **84% de acurácia** e insights práticos para melhorar a performance.

---

## 📁 Projetos Detalhados

---

### 🧪 Projeto 01: Classificação da Performance de Estudantes  
🔗 **[Notebook → projeto1.ipynb](projeto1.ipynb)**

> Classificação baseada em dados educacionais (idade, etnia, faltas, etc.), com foco em decisões bem fundamentadas desde o pré-processamento.

**🌟 Destaques:**

- Corrigi um **erro do dataset original** na coluna `GradeClass`, que estava rotulando mal os alunos com GPA baixo.
- Identifiquei desbalanceamento severo e usei **SMOTE com segurança**, após o split, evitando vazamento.
- Construí pipeline robusto com foco em evitar enviesamentos.

**📊 Resultados:**

- **Acurácia:** 96%
- **F1-score (macro):** 0.96
- **Desempenho estável** mesmo com dados desbalanceados

---

### 🧠 Projeto 02: Previsão de Churn com EDA, Testes Estatísticos e Rede Neural  
🔗 **[Notebook → projeto2.ipynb](projeto2.ipynb)**

> Predição de churn integrando **estatística inferencial** com **redes neurais**, garantindo não só performance, mas **interpretação e confiança nos dados**.

**🔬 Testes de hipóteses aplicados:**

- Qui-quadrado → 📌 Gênero influencia no churn
- Mann-Whitney → 📌 Salário **não** tem impacto significativo
- Kruskal-Wallis → 📌 Nº de produtos tem relação não-linear com churn

**🤖 Modelagem com MLP:**

- Perceptron multicamadas com ReLU e saída Sigmoid
- Otimizador **Adam**, função de perda **Binary Crossentropy**
- Dados normalizados e balanceados com SMOTE

**📈 Resultados:**

- **Acurácia:** 82%
- **F1-Score:** 59%
- **Recall:** 67%
- **Precision:** 54%

**💡 Insights práticos:**

- Idade > 40 aumenta risco 2x
- Clientes da Alemanha têm maior taxa de churn
- Clientes inativos e com saldo alto saem mais

---

### 🏠 Projeto 03: Previsão de Aluguel com Regressão Linear e Classificação  
🔗 **[Notebook → projeto3.ipynb](projeto3.ipynb)**

> Estimativa do valor de aluguel de apartamentos e classificação como **caro ou barato** baseado em dados reais de área, quartos, banheiros, garagem e localização.

**🔍 EDA — principais descobertas:**

- **Área (m²)** tem forte impacto positivo no preço  
- **Distância do centro** tem impacto negativo  
- Modelo revela coeficientes intuitivos e úteis

**📉 Regressão Linear — Resultados:**

- **MAE:** R$158,61
- **R² Score:** 0.82
- **Coeficientes:**
  - +R$24,03/m²
  - +R$123,95/quarto
  - +R$101,11/banheiro
  - +R$196,86 com garagem
  - –R$51,10/km de distância do centro

**📊 Classificação: Caro ou Barato**

- **Acurácia:** 84%
- **Precisão:** 87%
- **Recall:** 83%
- ⚠️ 18 falsos negativos — imóveis caros classificados como baratos

**🚧 Melhorias sugeridas:**

- Engenharia de atributos
- Remoção de outliers
- Testes com modelos mais robustos (Random Forest, SVM, Gradient Boosting)

---

📌 *Mais projetos serão adicionados em breve, com foco em desafios reais, validação estatística e soluções de alto valor analítico.*

