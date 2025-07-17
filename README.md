# Diagnóstico Inteligente de Falhas em Máquinas Industriais

Este projeto apresenta uma solução de manutenção preditiva orientada por dados, capaz de detectar falhas iminentes e identificar o tipo provável de falha com base em variáveis operacionais de sensores de máquinas industriais. A abordagem combina técnicas robustas de machine learning supervisionado, tratamento de desbalanceamento e visualização interativa dos resultados.

## Objetivo

Construir modelos capazes de:
- Detectar se uma máquina irá falhar em breve (classificação binária)
- Classificar automaticamente o tipo de falha (classificação multiclasse)
A solução pode ser usada por equipes de engenharia e operação para antecipar paradas, otimizar manutenção e aumentar a confiabilidade operacional.

## Metodologia

1. Preparação dos dados:
   - Análise estatística e tratamento de valores ausentes
   - Avaliação do desbalanceamento nas variáveis-alvo
   - Escalonamento com StandardScaler

2. Balanceamento e codificação:
   - Aplicação de SMOTE para balancear os dados
   - Codificação de variáveis categóricas (quando necessário)

3. Modelagem:
   - Random Forest, XGBoost e StackingClassifier
   - Avaliação com accuracy, recall, precision, f1-score, ROC AUC

4. Visualização:
   - Matrizes de confusão
   - Classificação por tipo de falha
   - Painel interativo com Dash + Plotly

## Bibliotecas Utilizadas

pandas  
numpy  
matplotlib  
seaborn  
scikit-learn  
xgboost  
imblearn  
dash  
plotly

## Execução

O notebook contém todas as análises, modelagens e visualizações interativas.  
Pode ser aberto diretamente em qualquer ambiente Jupyter ou Google Colab.

## Estrutura

diagnostico-falhas-maquinas/  
├── notebooks/  
│   └── Diagnostico_inteligente_de_falhas_maquinas.ipynb  
├── README.md    
└── LICENSE

## Autor

Heitor Tonet  
Engenheiro de Controle e Automação e Cientista de Dados, com foco em manutenção preditiva industrial, especializado em modelos de RUL, detecção de falhas, séries temporais e simulações baseadas em física.

## Licença

Este projeto está sob a licença MIT.
