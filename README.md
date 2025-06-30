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

### Projeto 02: Previsão de Churn com EDA, Testes Estatísticos e Rede Neural Multicamadas (MLP)  
**🔗 Link para o notebook → [projeto2.ipynb](projeto2.ipynb)**

Neste projeto, desenvolvi uma **rede neural perceptron multicamadas (MLP)** para prever **quais clientes têm maior probabilidade de deixar a empresa (churn)** com base em dados demográficos e comportamentais. O projeto integrou **análise exploratória detalhada**, **testes estatísticos de hipóteses**, **balanceamento de dados com SMOTE** e a construção de um pipeline robusto com redes neurais.

> Essa experiência me permitiu integrar métodos estatísticos com redes neurais, validando hipóteses de negócio com testes clássicos e depois transformando os dados em insights para uma arquitetura de aprendizado profundo.

**Hipóteses testadas e validadas:**

- **Mulheres apresentam 1.5x mais churn** que os homens (🔎 Teste do Qui-Quadrado).
- **Salário não tem influência estatística significativa** no churn (🔎 Teste de Mann-Whitney).
- **Número de produtos influencia o churn de forma não-linear** (🔎 Teste de Kruskal-Wallis).
- Identificação de variáveis com **classes desbalanceadas**, tratadas com **SMOTE** após o split.

**Modelagem:**

- Rede neural **Multilayer Perceptron (MLP)** com função de ativação ReLU e saída sigmoid.
- Dados normalizados e balanceados.
- Função de custo: Binary Crossentropy  
- Otimizador: Adam

**Resultados do modelo:**

- **Acurácia:** 82%
- **F1-Score:** 59%
- **Precision:** 54% — presença de falsos positivos (clientes previstos como churn, mas que não saíram).
- **Recall:** 67% — o modelo capturou 67% dos churns reais.

**Erros principais:**

- **226 falsos positivos:** clientes que ficaram, mas foram classificados como churn.
- **131 falsos negativos:** clientes que saíram, mas não foram detectados.

**Fatores relevantes para churn identificados na análise:**

- **Idade > 40 anos:** risco 2x maior de churn.
- **Clientes da Alemanha:** taxa de churn de 32% (vs. 16% na França).
- **Clientes inativos (`IsActiveMember=0`)**: 27% de churn (vs. 15% entre os ativos).
- **Saldo elevado (> €100 mil):** mais propensos a sair.

**Possibilidade de melhoria:**

- Ajustar o **limiar de decisão (threshold)** da MLP para melhorar o recall e reduzir os falsos negativos.
- Explorar regularização ou arquiteturas mais profundas para maior capacidade de generalização.

---

Mais projetos serão adicionados em breve, abordando problemas reais com foco em análise de dados, validação estatística e aplicação prática de modelos preditivos e redes neurais.
