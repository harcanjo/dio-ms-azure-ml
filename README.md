# Dio - Microsoft Azure AI Fundamentals -  Trabalhando com Machine Learning na Prática no Azure ML

**Criando um Modelo de Previsão com Pontos de Extremidade no Azure Machine Learning**

*Descrição*
Modelo de previsão de regressão linear usando o Azure Machine Learning (AML) e configuração de um ponto de extremidade para que o modelo possa ser usado em aplicações de produção. 
O modelo prediz o preço de imóveis com base em características como tamanho, número de quartos e localização.

*Pré-requisitos*
- [ ] Conta do Azure
- [ ] Espaço de Trabalho do Azure Machine Learning
- [ ] SDK do Azure Machine Learning
- [ ] Arquivo CSV com dados de treinamento

*Passo a Passo*
1. Criar um Espaço de Trabalho do Azure Machine Learning
- Siga as instruções no portal do Azure para criar um novo Espaço de Trabalho do Azure Machine Learning.

2. Carregar os Dados
- No portal do AML, navegue até a seção Dados.
- Clique em Criar conjunto de dados.
- Selecione a opção De armazenamento Blob.
- Carregue o arquivo CSV que contém os dados de treinamento.
- Defina o nome do conjunto de dados e configure o esquema.

3. Treinar o Modelo
- No portal do AML, navegue até a seção Experimentos.
- Clique em Criar experimento.
- Selecione o script de treinamento train_regression_model.py.
- Defina os parâmetros do experimento, como o nome do modelo e o tipo de algoritmo.
- Clique em Iniciar.
- Aguarde alguns minutos para que o modelo seja treinado.

4. Avaliar o Modelo
- No portal do AML, navegue até a seção Modelos.
- Selecione o modelo que você treinou.
- Clique na guia Métricas.
- Analise as métricas de avaliação, como R^2 e RMSE.

5. Criar um Ponto de Extremidade
- No portal do AML, navegue até a seção Modelos.
- Selecione o modelo que você treinou.
Clique na guia Pontos de extremidade.
Clique em Criar ponto de extremidade.
Selecione o tipo de ponto de extremidade (por exemplo, Batch ou Real-time).
Configure as opções de deployment.
Clique em Criar.
Aguarde alguns minutos para que o ponto de extremidade seja criado.

6. Testar o Ponto de Extremidade
- Use o SDK do Azure Machine Learning para enviar dados de entrada para o ponto de extremidade.
- Receba as previsões do modelo.
- Arquivos
- [x] imoveis.json
