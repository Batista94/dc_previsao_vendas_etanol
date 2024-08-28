# Modelagem Preditiva de Vendas de Etanol na Região Sudeste do Brasil

Este repositório contém o projeto completo de previsão de vendas de etanol na região Sudeste do Brasil, desenvolvido como caso de estudo de minha monografia do MBA em Inteligência Artificial e Big Data no ICMC-USP. O projeto utiliza técnicas avançadas de machine learning para prever as vendas de etanol, considerando as complexidades e desafios do agronegócio de cana-de-açúcar.

## Visão Geral do Projeto

A produção de etanol desempenha um papel importante no setor sucroenergético do Brasil, com a região Sudeste sendo uma grande contribuinte. Este projeto visa melhorar a previsibilidade das vendas de etanol através da aplicação de Inteligência Artificial (IA) e modelos de machine learning, para previsão de vendas em m³ de etanol.

### Principais Características

- **Dataset Abrangente**: O dataset inclui dados históricos sobre a produção, capacidade e vendas de etanol nos estados da região Sudeste, de janeiro de 2019 a dezembro de 2023.
- **Pré-processamento Avançado**: Pré-processamento detalhado dos dados, incluindo tratamento de valores ausentes através de interpolação cúbica, normalização e tratamento de outliers para garantir a integridade dos dados.
- **Diversidade de Modelos Preditivos**: Implementação de vários modelos preditivos, incluindo ARIMA, SARIMA, XGBoost e Prophet, com uma comparação detalhada de seus desempenhos.
- **Análise de Séries Temporais**: Utilização de validação cruzada em séries temporais e validação cruzada em janela expansiva para avaliar o desempenho dos modelos de forma realista.

### Estrutura do Repositório

- `Dados/`: Contém os datasets processados utilizados para a modelagem.
- `Codigos/`: Notebooks Jupyter usados para o pré-processamento, modelagem e análise dos dados.
  - `unificado-com-interpolacao.ipynb`: Notebook detalhando as etapas de pré-processamento dos dados, incluindo interpolação e normalização.
  - `comparacao-modelos-preditivos.ipynb`: Notebook comparando o desempenho de diferentes modelos preditivos.
  - `comparacao-modelos-preditivos_atualizado_final.ipynb`: Notebook atualizado com as comparações finais dos modelos e resultados.
- `README.md`: Este arquivo, fornecendo uma visão geral do projeto.

### Pré-processamento de Dados

O pré-processamento dos dados foi uma etapa crucial neste projeto, envolvendo:
- **Conversão de Datas**: Transformação das colunas de data para o formato DateTime para uma análise precisa das séries temporais.
- **Tratamento de Valores Ausentes**: Aplicação de interpolação cúbica para lidar com valores ausentes nas colunas de produção e capacidade.
- **Normalização**: Utilização da escala Min-Max para normalizar os dados, garantindo que todas as variáveis estejam na mesma escala.

### Modelos e Avaliação

O projeto explora uma variedade de modelos:
- **ARIMA e SARIMA**: Utilizados para capturar tendências lineares e sazonalidade em dados de séries temporais.
- **XGBoost**: Escolhido pela sua capacidade de lidar com relações não-lineares e interações complexas.
- **Prophet**: Um modelo robusto, projetado para lidar com sazonalidade e feriados, especialmente útil para séries temporais relacionadas a negócios.

#### Métricas de Desempenho
- **RMSE (Root Mean Squared Error)** e **MAE (Mean Absolute Error)** foram as principais métricas usadas para avaliar a precisão dos modelos.
- O modelo **XGBoost** demonstrou superioridade com o menor RMSE, especialmente na previsão de vendas de etanol em cenários com alta variabilidade.

### Principais Insights

- O modelo **XGBoost** foi o mais eficaz em lidar com as complexidades da previsão de vendas de etanol, superando os modelos tradicionais de séries temporais em termos de precisão.
- A sazonalidade desempenha um papel significativo nas vendas de etanol, e modelos que incorporam este aspecto, como SARIMA e Prophet, fornecem insights valiosos, apesar de algumas limitações em contextos não sazonais.

### Trabalhos Futuros

Futuras melhorias podem incluir:
- Integração de mais variáveis externas, como indicadores econômicos ou condições climáticas, para melhorar ainda mais a precisão das previsões.
- Exploração de modelos de deep learning, como LSTM, para capturar dependências de longo prazo nos dados de séries temporais.

### Autor

Este projeto foi desenvolvido por Weslei Rodrigues Batista como parte do MBA em Inteligência Artificial e Big Data no ICMC-USP.
