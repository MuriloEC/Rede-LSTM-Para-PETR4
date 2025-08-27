# 📈 Previsão de Preço da Ação PETR4 com LSTM

Este projeto utiliza uma rede neural do tipo LSTM (Long Short-Term Memory) para prever o preço de fechamento da ação **PETR4 (Petrobras)**, com base em dados históricos obtidos do Yahoo Finance.

## 📦 Bibliotecas Utilizadas

- yfinance – Para download dos dados financeiros históricos
- pandas – Manipulação de dados
- numpy – Operações matemáticas e vetoriais
- matplotlib – Visualização dos resultados
- scikit-learn – Normalização dos dados
- TensorFlow / Keras – Construção e treinamento da rede LSTM

## 📊 O que o código faz?

1. **Coleta os dados históricos da ação PETR4** usando a API do Yahoo Finance.
2. **Seleciona os preços de fechamento** e normaliza os dados para o intervalo entre 0 e 1.
3. **Cria sequências temporais** de 60 dias para usar como entrada na LSTM, e o dia seguinte como saída.
4. **Divide os dados em treino e teste** (80% treino / 20% teste).
5. **Cria e treina uma rede neural LSTM**, com uma camada LSTM e uma camada densa de saída.
6. **Faz previsões** sobre os dados de teste.
7. **Desnormaliza os dados** para visualização.
8. **Plota um gráfico** comparando os valores reais e os previstos.


## 📈 Exemplo de Saída Gráfica

O gráfico gerado apresenta duas curvas:
- **Real**: preço real de fechamento da PETR4 no período de teste
- **Previsto**: preço previsto pela LSTM

Isso permite avaliar visualmente a performance do modelo.
