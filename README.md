# Análise de Regressão Linear: Seleção de Variáveis e Simplificação do Modelo

Este repositório contém uma análise detalhada de como selecionar variáveis significativas para um modelo de regressão linear e simplificar o modelo para melhor interpretabilidade sem comprometer significativamente a capacidade explicativa.

## Descrição do Projeto

O objetivo deste projeto foi ajustar um modelo de regressão linear para explicar a variável dependente `log_renda` usando várias variáveis categóricas e contínuas. A análise focou em identificar as variáveis mais significativas estatisticamente, remover variáveis menos significativas, e avaliar o impacto dessas remoções no ajuste do modelo.

## Métodos Utilizados

- **Seleção de Variáveis**: Utilizamos p-valores para identificar e remover variáveis menos significativas do modelo.
- **Ajuste do Modelo**: Aplicamos a regressão linear ordinária (OLS) para ajustar o modelo com as variáveis selecionadas.
- **Avaliação de Modelo**: Comparamos os modelos ajustados usando R-quadrado e outros critérios para avaliar o ajuste do modelo.

## Ferramentas e Bibliotecas

- Python
- Pandas para manipulação de dados
- Statsmodels para ajuste do modelo de regressão linear
- Patsy para especificação de modelos

## Processo

1. **Preparação dos Dados**: Carregamos e preparamos os dados, incluindo a imputação de valores ausentes e a transformação logarítmica da variável dependente.

2. **Ajuste do Modelo Inicial**: Ajustamos um modelo inicial incluindo todas as variáveis disponíveis.

3. **Seleção de Variáveis**: Removemos iterativamente as variáveis menos significativas com base nos p-valores, reajustando o modelo após cada remoção.

4. **Avaliação do Modelo Final**: Comparamos o modelo final simplificado com o modelo inicial para avaliar as mudanças no ajuste do modelo.

## Resultados

O modelo final, simplificado, manteve apenas as variáveis com significância estatística (p-valor < 0.005), resultando em um modelo mais interpretável com uma diminuição mínima na capacidade explicativa (R-quadrado).

## Conclusão

A seleção criteriosa de variáveis com base na significância estatística pode simplificar modelos de regressão linear sem comprometer demasiadamente a capacidade explicativa. Este processo destaca a importância de variáveis chave, facilitando a interpretação e a aplicação do modelo.
