📊 TelecomX – Predição de Churn (Parte 2)
📌 Contexto do Projeto
Este repositório corresponde à segunda fase do desafio “TelecomX – Análise de Evasão de Clientes”, cujo propósito é compreender os fatores que levam clientes de uma empresa de telecomunicações a cancelar seus serviços.

Após a etapa inicial de tratamento e exploração dos dados, avançamos para a construção de modelos preditivos que apoiem estratégias de retenção e ofereçam insights acionáveis para o negócio.

A base utilizada contém informações contratuais, financeiras e demográficas dos clientes, além do status de churn, já devidamente tratada na Parte 1.

🎯 Objetivo
O foco desta etapa é desenvolver e avaliar modelos de Machine Learning capazes de prever com precisão o churn.
A análise busca identificar variáveis críticas — como tipo de contrato, tempo de permanência e serviços adicionais — que funcionam como gatilhos de evasão, permitindo ações preventivas e direcionadas.

Link do Colab: https://colab.research.google.com/drive/1i-AUVCAnA7n2yq1fBk0UXNWTtC-KHMwn?usp=sharing

📂 Estrutura
README.md → Documentação do projeto

TelecomX2.ipynb → Notebook principal com todo o pipeline de análise e modelagem

dados_tratados.csv → Base de dados limpa (gerada na Parte 1)

🛠️ Preparação dos Dados
Etapas realizadas para garantir consistência e qualidade dos modelos:

Classificação de variáveis

Numéricas: tempo_contrato, valor_mensal, total_cobrado

Categóricas: tipo_contrato, forma_pagamento, servicos_internet, etc.

Transformações

One-Hot Encoding para variáveis categóricas

MinMaxScaler para normalização das variáveis numéricas (escala 0–1)

Divisão da base

70% treino / 30% teste

Amostragem estratificada para preservar a proporção de churn

📈 Principais Insights (EDA)
Contratos mensais apresentam risco significativamente maior de evasão.

Clientes recentes são os mais propensos ao churn.

Serviços adicionais como suporte técnico e segurança online reduzem a probabilidade de cancelamento.

🤖 Modelagem
Modelos testados e suas contribuições:

Regressão Logística (80,4% acurácia): melhor desempenho geral e alta interpretabilidade.

SVM (80,0% acurácia): bom ajuste para fronteiras de decisão complexas.

Random Forest: útil para avaliar importância das variáveis.

Árvore de Decisão: fornece regras claras e visualmente compreensíveis.

🚀 Execução
Para rodar o projeto no Google Colab:

Faça upload do notebook e do arquivo dados_tratados.csv.

Abra o notebook no Colab.

Execute as células na ordem indicada.
