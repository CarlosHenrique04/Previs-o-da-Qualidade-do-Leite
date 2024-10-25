# Previsão da Qualidade do Leite com Aprendizado Semi-Supervisionado

Este projeto tem como objetivo prever a qualidade do leite utilizando técnicas de aprendizado de máquina supervisionado e semi-supervisionado. O foco está na aplicação de Support Vector Machines (SVM) e no uso de Self-Training para lidar com dados parcialmente rotulados.

## Objetivo

O principal objetivo deste projeto é desenvolver um modelo que possa prever a qualidade do leite com base em características físico-químicas. Como parte deste trabalho, foi explorado o uso de dados não rotulados, aplicando pseudo-rotulagem e Self-Training para melhorar a performance do modelo.

## Etapas do Projeto

1. **Pré-processamento dos Dados**:
   - Leitura e análise do conjunto de dados.
   - Tratamento de valores ausentes.
   - Normalização das variáveis utilizando `MinMaxScaler`.
   - Transformação das variáveis categóricas.

2. **Modelagem Supervisionada**:
   - Implementação de um modelo SVM supervisionado para previsão da qualidade do leite.
   - Avaliação do modelo utilizando métricas como `classification_report` para analisar a acurácia, precisão, recall, e F1-score.

3. **Pseudo-rotulagem**:
   - Utilização de dados não rotulados para realizar pseudo-rotulagem.
   - Treinamento do modelo SVM com dados rotulados manualmente e pseudo-rotulados para melhorar a generalização.

4. **Self-Training**:
   - Implementação da técnica de Self-Training utilizando o classificador SVM, com um limiar de confiança para integrar previsões com alta confiança no processo de treinamento.

5. **Avaliação do Desempenho**:
   - Comparação entre os modelos supervisionado, pseudo-rotulado e Self-Training, utilizando relatórios de classificação e visualizações para a análise dos resultados.

## Tecnologias Utilizadas

- **Linguagem de Programação**: Python
- **Bibliotecas**: pandas, scikit-learn, matplotlib, SVM, Self-Training
- **Técnicas**: SVM, Pseudo-rotulagem, Self-Training, Normalização de Dados, Classificação Semi-Supervisionada

## Conclusão

Este projeto oferece uma visão sobre como lidar com problemas onde uma parte significativa dos dados não é rotulada. Utilizando aprendizado semi-supervisionado e pseudo-rotulagem, é possível melhorar a performance de modelos preditivos e explorar dados não rotulados de maneira eficaz.
