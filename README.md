# Projeto de Previsão de Renda

Este projeto tem como objetivo prever a **renda** com base em um conjunto de dados, utilizando técnicas de **regressão linear**. O projeto segue as etapas do **Crisp-DM** (Cross-Industry Standard Process for Data Mining), abordando desde a análise exploratória de dados até a implementação do modelo.

## Índice

1. [Descrição do Projeto](#descrição-do-projeto)
2. [Objetivos](#objetivos)
3. [Tecnologias Utilizadas](#tecnologias-utilizadas)
4. [Etapas do Projeto](#etapas-do-projeto)
5. [Resultados](#resultados)
6. [Conclusão](#conclusão)
7. [Extras](#extras)

## Descrição do Projeto

Este projeto busca analisar a relação entre diferentes variáveis e a **renda** de indivíduos, utilizando modelos de regressão linear. A partir de uma análise exploratória, foi realizado o tratamento dos dados, seleção das variáveis mais relevantes, e finalmente a construção de modelos de previsão, incluindo a aplicação de transformações logarítmicas para melhorar o desempenho dos modelos.

## Objetivos

- Analisar os dados para entender o comportamento das variáveis.
- Realizar o tratamento dos dados, incluindo a remoção de valores ausentes e a transformação de variáveis.
- Construir e comparar diferentes modelos de regressão para prever a renda.
- Avaliar o desempenho dos modelos utilizando a métrica **RMSE** (Root Mean Squared Error).
- Identificar o modelo com o melhor desempenho.

## Tecnologias Utilizadas

- **Python 3.x**
- **Pandas**: Manipulação e análise de dados.
- **NumPy**: Cálculos numéricos.
- **Matplotlib & Seaborn**: Visualização de dados.
- **Scikit-learn**: Construção de modelos e avaliação de desempenho.
- **Statsmodels**: Modelos de regressão e análise estatística.
- **Streamlit**: Interface web interativa.
- **Jupyter Notebook**: Desenvolvimento interativo do código.

## Etapas do Projeto

O projeto segue o processo do **Crisp-DM** e as principais etapas incluem:

1. **Entendimento do Negócio**: O objetivo principal é prever a renda de indivíduos com base em várias variáveis.
   
2. **Entendimento dos Dados**: A partir de uma base de dados, foram feitas análises exploratórias para identificar padrões e comportamentos das variáveis.

   - Durante a análise exploratória, a variável **'renda'** não apresentou uma correlação forte com outras variáveis do dataset.
   - A categoria **'pensionista'** foi removida devido à grande diversidade dentro desse grupo. Não foi possível estabelecer uma relação direta entre ser pensionista e a renda, o que poderia comprometer a previsão do modelo.
   - Constatou-se que a informação sobre ser pensionista não fornece insights relevantes, pois dentro desse grupo existem tanto indivíduos que possuem carro quanto aqueles que não possuem, dificultando a identificação de padrões claros.

3. **Preparação dos Dados**: Durante esta etapa, foram realizadas:
   - Limpeza dos dados (tratamento de valores).
   - Transformações de variáveis, incluindo a normalização e a transformação logarítmica da variável de renda.

4. **Modelagem**:
   - Modelos de regressão linear foram treinados com diferentes conjuntos de variáveis e abordagens, incluindo:
     - Regressão com todas as variáveis.
     - Regressão com variáveis selecionadas por um método stepwise.
     - Regressão com transformação logarítmica na variável de renda.

5. **Avaliação**: A métrica de avaliação escolhida foi o **RMSE** (Root Mean Squared Error). Os modelos foram avaliados e comparados para determinar qual modelo teve o melhor desempenho.

6. **Implantação**: Não houve implementação, rs

## Resultados

Durante a avaliação dos modelos, foram calculados os **RMSE** de cada modelo:

1. **Modelo 'resultado'**:
   - **RMSE**: 7442.74

2. **Modelo 'resultado2'**:
   - **RMSE**: 7432.03

3. **Modelo 'resultado3'** (com transformação logarítmica na variável de renda):
   - **RMSE**: 6952.15

### Discussão:

- O **Modelo `'resultado3'`** obteve o melhor desempenho, com o menor RMSE, indicando que a transformação logarítmica na variável de renda foi eficaz.
- O **Modelo `'resultado2'`**, apesar de utilizar menos variáveis, também apresentou um bom desempenho.
- A transformação logarítmica mostrou-se útil para modelar a variável de renda, que tende a seguir um comportamento multiplicativo.

## Conclusão

O modelo com a transformação logarítmica da variável de renda (Modelo `'resultado3'`) foi o mais eficaz, apresentando o menor RMSE. A análise sugeriu que a transformação de variáveis pode ser uma estratégia importante para melhorar o desempenho do modelo. Este projeto é um exemplo de como diferentes abordagens de modelagem podem ser testadas para resolver um problema de previsão.

## Licença

Este projeto está licenciado sob a Licença MIT - consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

## Extras


https://github.com/user-attachments/assets/eae22504-0630-429b-8760-a0d6fd2e3a76




