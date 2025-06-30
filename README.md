
# Estudos Ciência de Dados

Repositório dos meus estudos em Ciência de Dados, com foco em análise crítica, limpeza de dados e modelagem.

## Projetos

### Projeto 01: Classificação da Performance de Estudantes — Limpeza, Análise e Balanceamento
**Link para o notebook --> [projeto1](projeto1.ipynb)**

Projeto de classificação baseado em dados educacionais (idade, etnia, faltas, etc.), com forte ênfase em preparação de dados e decisões fundamentadas. Pois sem o pré-processamento correto, um aspecto *indesejado* teria enviesado a análise e o treinamento do modelo desde o início.

> O projeto melhorou minha capacidade de identificar falhas na estrutura do dataset,como valores inconsistentes nas colunas e  aplicar técnicas apropriadas de balanceamento e construir um pipeline de classificação confiável e bem justificado.

**Pontos-chave:**

* **Correção da variável alvo:** A coluna `GradeClass`, que representa faixas de GPA, apresentava classificações incorretas — alunos com nota abaixo de 3.5 estavam rotulados como se tivessem nota acima. Refiz a segmentação com base no GPA real. Sem essa correção, a análise e o modelo estariam enviesados desde o início.
* **Desbalanceamento identificado:** Diversas colunas apresentavam forte desequilíbrio entre as classes, tanto nas variáveis preditoras quanto na variável alvo.
* **Uso de SMOTE:** Após análise da distribuição, utilizei SMOTE para balancear as classes da variável alvo, garantindo que o modelo não fosse tendencioso. A técnica foi aplicada **após o split de treino e teste**, evitando vazamento de dados.

**Resultados:**

* **Acurácia:** 96%
* **F1-score (macro):** 0.96
* Desempenho estável em todas as classes, mesmo com dados originalmente desbalanceados.

