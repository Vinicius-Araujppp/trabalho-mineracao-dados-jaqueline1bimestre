# Trabalho de Mineração de Dados \- 1º Bimestre

**Instituição:** Faculdade de Tecnologia de Franca (Fatec Franca) \- "Dr. Thomaz Novelino"  
**Disciplina:** Mineração de Dados  
**Professora:** Jaqueline Brigladori Pugliesi

## Sobre o Projeto

Este repositório contém o trabalho prático do 1º Bimestre, que tem como objetivo a utilização de algoritmos de seleção de atributos como parte de um processo de Mineração de Dados para duas tarefas principais:

1. **Classificação** (utilizando a base citológica *Breast Cancer Wisconsin*).  
2. **Regressão** (utilizando a base de custos médicos *insurance.csv*).

## Estrutura do Repositório

* `data/raw/`: Pasta destinada ao armazenamento dos dados brutos (ex: `insurance.csv`).  
* `notebooks/`: Contém os notebooks Jupyter com as análises:  
  * `01_classificacao_breast_cancer.ipynb`: Tarefa de Classificação aplicando Eliminação Recursiva de Atributos (RFE).  
  * `02_regressao_insurance.ipynb`: Tarefa de Regressão aplicando penalização Lasso (L1).

## Metodologia Aplicada

Em cada um dos notebooks, foram rigorosamente seguidas as 8 etapas exigidas para o trabalho:

1. **Introdução:** Apresentação da base de dados e objetivos.  
2. **Pré-processamento e exploração dos dados:** Padronização (StandardScaler), verificação e codificação de variáveis (OneHotEncoder).  
3. **Divisão em conjunto de treinamento e teste:** Utilizando proporção 80/20 (com estratificação para classificação).  
4. **Treinamento e avaliação do modelo inicial:** Regressão Logística (Classificação) e Regressão Linear (Regressão) com todos os atributos.  
5. **Seleção de Atributos:** RFE (reduzindo dimensões) e Lasso (zerando coeficientes).  
6. **Treinamento e avaliação do modelo com seleção de atributos:** Re-treinamento usando o subconjunto ideal de variáveis.  
7. **Discussão dos resultados:** Análise visual e de métricas (Matriz de Confusão, Gráficos de Coeficientes e Resíduos, RMSE, R2, Acurácia).  
8. **Conclusão:** Síntese final sobre o ganho de interpretabilidade e impacto da remoção de variáveis irrelevantes.

## Como Executar

1. Clone este repositório ou abra os arquivos `.ipynb` diretamente no Google Colab.  
2. Para o notebook de Regressão, certifique-se de fazer o upload do arquivo `insurance.csv` no ambiente de execução.  
3. Execute todas as células sequencialmente (`Ambiente de Execução > Executar Tudo` no Colab) para gerar as saídas e gráficos.