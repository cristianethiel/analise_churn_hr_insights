# Churn de Colaboradores - HR Insights

Análise de rotatividade de funcionários com foco na identificação de padrões associados à saída de colaboradores. O projeto visa apoiar estratégias de retenção e otimização do clima organizacional com base em dados reais da empresa.

## Visão Geral

A HR Insights identificou uma taxa crescente de turnover em determinados setores da empresa. O objetivo deste projeto é construir um modelo preditivo que identifique os principais fatores associados à saída de funcionários, permitindo ações mais estratégicas por parte da área de Recursos Humanos.

## Problema Central

A ausência de critérios objetivos dificultava a identificação de funcionários em risco de saída. Era necessário:

- Uma análise exploratória profunda das características dos colaboradores.
- Um modelo preditivo que sinalizasse os principais fatores de risco.
- Uma base para tomada de decisão com foco em retenção e alocação estratégica.

## Ferramentas e Tecnologias

- **Linguagens:** Python
- **Bibliotecas:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost
- **Ambiente:** Jupyter Notebook / VS Code

## Estrutura do Repositório

- `/dataset`: Base de dados original e tratada (CSV).
- `/documentacao`: Documentos técnicos do projeto.
  - `apresentacao_churn_colaboradores.pdf`: Metodologia, Tratamento de Dados e Insights.
  - `ficha_tecnica_churn_colaboradores`: Insights e Recomendações.
- `rh_churn.ipynb`: Notebook com EDA, engenharia de atributos e modelagem preditiva.
- `requirements.txt`: Bibliotecas utilizadas.

## Metodologia

- **Tratamento e Pré-processamento:**
  - Exclusão de variáveis irrelevantes ou sensíveis (como gênero e estado civil).
  - Correção de nulos e transformação de tipos de dados.

- **Análise Exploratória (EDA):**
  - Boxplots e histogramas para distribuição e outliers.
  - Correlação entre variáveis.
  - Comparações bivariadas entre variáveis e o churn.

- **Feature Engineering e Preparação dos Dados para os Modelos:**
  - Criação de variáveis dummies para variáveis categóricas.
  - Seleção das variáveis mais relevantes.
  - Criação do dataframe final para modelagem.

- **Modelagem Preditiva:**
  - Divisão dos dados em treino e teste.
  - Treinamento com XGBoost.
  - Avaliação com matriz de confusão e relatório de classificação.
  - Treinamento com Random Forest.
  - Avaliação com matriz de confusão e relatório de classificação.
  - Avaliação, Otimização e Benchmark.
  - Curvas ROC, Precision-Recall e Learning Curve.
  - Análise de Fairness (Sem Viés e Decisões Justas).


## Principais Insights Estratégicos da Análise de Churn

- **Viagens frequentes representam o maior fator de risco individual.** Colaboradores que viajam com frequência apresentam taxa de churn de 25%, mais de 3x superior aos que não viajam (8%). O desgaste físico e emocional das viagens constantes impacta diretamente na retenção, exigindo políticas de flexibilidade pós-viagem, pausas programadas e alternativas de trabalho remoto.

- **Perfil demográfico e financeiro são preditores críticos.** Funcionários mais jovens (18-30 anos) e com menor renda mensal (até R$ 30.000) concentram o maior risco de saída. A mediana salarial dos que permanecem é aproximadamente o dobro dos que saem (R$ 50.000 vs R$ 25.000), indicando que estratégias de retenção devem priorizar revisão de remuneração e benefícios personalizados para esses grupos.

- **Cargos estratégicos de P&D e funções comerciais demandam atenção especial.** Além dos tradicionais cargos de vendas, funções críticas como Research Director (23% churn) e Research Scientist (18%) apresentam alta rotatividade. Perdas nessas áreas afetam diretamente inovação e competitividade, exigindo programas de retenção específicos com planos de desenvolvimento científico e reconhecimento diferenciado.

- **Experiência profissional supera tempo de empresa como preditor.** O tempo total de carreira (TotalWorkingYears) mostrou-se mais preditivo que o tempo na empresa atual, sugerindo que o momento de carreira influencia mais que a antiguidade no cargo. O relacionamento com a liderança também é crítico, com o tempo com o gestor atual aparecendo consistentemente como fator relevante nos dois modelos preditivos.

- **Modelo preditivo alcança 94% de precisão sem viés demográfico.** A análise de fairness confirmou que o modelo mantém alta performance em todos os grupos demográficos, com recall de 94.2% para jovens e F1-Score de 95.1% para baixa renda. Isso permite implementar ações preventivas baseadas em dados com 94% de precisão, identificando colaboradores em risco antes da saída efetiva.

## Analista de Dados

**Cristiane Thiel**  
🌐 [https://cristianethiel.com.br/](https://cristianethiel.com.br/)  
🔗 [https://www.linkedin.com/in/cristianethiel/](https://www.linkedin.com/in/cristianethiel/)
