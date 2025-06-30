# Estudos Ciência de Dados

Repositório dos meus estudos em Ciência de Dados, com foco em **análise crítica**, **limpeza de dados** e **modelagem supervisionada** com interpretação estatística.

## Projetos

---

### Projeto 01: Classificação da Performance de Estudantes — Limpeza, Análise e Balanceamento  
**🔗 Link para o notebook → [projeto1.ipynb](projeto1.ipynb)**

Projeto de classificação baseado em dados educacionais (idade, etnia, faltas, etc.), com forte ênfase em preparação de dados e decisões fundamentadas. Pois sem o pré-processamento correto, um aspecto *indesejado* teria enviesado a análise e o treinamento do modelo desde o início.

> O projeto melhorou minha capacidade de identificar falhas na estrutura do dataset, como valores inconsistentes nas colunas, aplicar técnicas apropriadas de balanceamento e construir um pipeline de classificação confiável e bem justificado.

**Pontos-chave:**

- **Correção da variável alvo:** A coluna `GradeClass`, que representa faixas de GPA, apresentava classificações incorretas — alunos com nota abaixo de 3.5 estavam rotulados como se tivessem nota acima. Refiz a segmentação com base no GPA real. Sem essa correção, a análise e o modelo estariam enviesados desde o início.
- **Desbalanceamento identificado:** Diversas colunas apresentavam forte desequilíbrio entre as classes, tanto nas variáveis preditoras quanto na variável alvo.
- **Uso de SMOTE:** Após análise da distribuição, utilizei SMOTE para balancear as classes da variável alvo, garantindo que o modelo não fosse tendencioso. A técnica foi aplicada **após o split de treino e teste**, evitando vazamento de dados.

**Resultados:**

- **Acurácia:** 96%
- **F1-score (macro):** 0.96
- **Desempenho estável** em todas as classes, mesmo com dados originalmente desbalanceados.

---

### Projeto 02: Previsão de Churn com EDA, Testes Estatísticos e Rede Neural (MLP)

🔗 **[Notebook do Projeto](projeto2.ipynb)**

Desenvolvi um modelo preditivo para identificar clientes com maior risco de **churn**, integrando **análise exploratória**, **testes estatísticos de hipóteses** e uma **rede neural MLP**.

O projeto evidenciou raciocínio analítico ao combinar **validação estatística de hipóteses de negócio** com técnicas de **machine learning supervisionado**, garantindo uma abordagem robusta e interpretável.

---

#### 🔍 Principais insights e hipóteses validadas:

* **Gênero:** mulheres têm 1.5x mais chance de churn (*Teste do Qui-Quadrado*).
* **Salário:** sem influência estatística significativa (*Teste de Mann-Whitney*).
* **Número de produtos:** relação não-linear com churn (*Teste de Kruskal-Wallis*).
* Dados desbalanceados tratados com **SMOTE**, aplicado após o *split* para evitar vazamento de informação.

---

#### 🧠 Modelagem com Rede Neural MLP:

* Arquitetura: Perceptron multicamadas com ReLU e saída sigmoid
* Normalização dos dados e função de custo: *Binary Crossentropy*
* Otimizador: **Adam**

**Métricas de desempenho:**

* **Acurácia:** 82%
* **F1-Score:** 59%
* **Recall:** 67% (captura da maioria dos churns reais)
* **Precision:** 54% (alguns falsos positivos)

---

#### 💡 Fatores de churn identificados:

* **Idade > 40:** risco 2x maior
* **Clientes da Alemanha:** 32% de churn (vs. 16% na França)
* **Clientes inativos:** churn de 27% (vs. 15% dos ativos)
* **Saldo alto (> €100 mil):** maior propensão a sair

---

#### 🚀 Próximos passos:

* Ajustar o **threshold de decisão** para reduzir falsos negativos
* Testar arquiteturas mais profundas e regularização para melhorar generalização

---

Mais projetos serão adicionados em breve, abordando problemas reais com foco em análise de dados, validação estatística e aplicação prática de modelos preditivos e redes neurais.
