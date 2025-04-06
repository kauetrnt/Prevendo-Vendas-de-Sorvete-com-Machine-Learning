# 🍦 Previsão de Vendas de Sorvete com Machine Learning - Gelato Mágico

Este projeto tem como objetivo aplicar técnicas de aprendizado de máquina para prever a quantidade de sorvetes vendidos com base na temperatura do dia. Ele foi desenvolvido no **Azure Machine Learning Studio**, utilizando o ambiente em nuvem para facilitar a criação, o treino e o deploy do modelo de forma estruturada e reprodutível.

---

## 🔧 Tecnologias Utilizadas

- Azure Machine Learning Studio
- Scikit-learn
- Pandas
- MLflow (para registro e rastreamento dos experimentos)
- Jupyter Notebook (via Azure)
- Python 3.x

---

## 🎯 Objetivo do Projeto

- Treinar um modelo preditivo de regressão que utiliza a temperatura como entrada para prever vendas.
- Gerenciar e versionar o modelo com MLflow.
- Utilizar o Azure como ambiente principal, sem necessidade de instalação local.
- Estruturar um pipeline reprodutível de Machine Learning.

---

## 📈 Etapas Realizadas

1. **Upload dos dados para Azure**
   - Arquivo CSV com dados de temperatura e vendas diárias.

2. **Exploração e Visualização**
   - Análise da correlação entre temperatura e volume de vendas.

3. **Pré-processamento**
   - Limpeza dos dados e separação em treino/teste.

4. **Treinamento**
   - Regressão Linear como primeiro modelo.
   - Avaliação com métricas como MAE, RMSE e R².

5. **Registro do Modelo**
   - Uso do MLflow para log de parâmetros, métricas e artefatos.

6. **Previsão**
   - Simulação de entrada de dados para prever novas vendas com base em temperatura.

---

## 📂 Pasta `inputs/`

Contém o arquivo `dados_sorvete.csv`, que deve conter os seguintes campos:

| Temperatura (°C) | Vendas (unidades) |
|------------------|-------------------|
| 22.5             | 105               |
| 30.1             | 220               |
| 18.0             | 60                |

---

## 📷 Prints Recomendados para Incluir

- Gráfico de dispersão: Temperatura x Vendas
- Resultado da regressão linear
- Interface do MLflow com métricas logadas
- Previsão de exemplo no Azure Notebook

---

## 💡 Aprendizados

- A temperatura é um ótimo preditor para vendas em dias quentes.
- O Azure ML Studio permite controle total do fluxo de trabalho sem depender de IDEs locais.
- O uso de MLflow facilita o rastreamento e versionamento dos experimentos.

---

## 🚀 Próximos Passos

- Incluir outras variáveis (ex: dia da semana, feriado, horário)
- Deploy do modelo como endpoint de previsão em tempo real via Azure
- Treinamento automático com novos dados adicionados ao workspace
