# walmart-store-sales-prediction
> Este projeto foi desenvolvido na disciplina de Aplicações de Machine Learning no Programa de Especialização em Software da Embraer em parceria com o CIn-UFPE, realizado em 2023

Repositório com análises de dados de varejo e predição das vendas futuras de lojas.

**Estrutura de Arquivos:**
- .gitignore: lista de pastas e arquivos ignorados pelo controle de versionamento do repositório
- README.md: este arquivo de descrição do repositório
- Arquivo notebook.ipynb: notebook com análises descritivas e exploratórias dos dados, além de realizar alguns tratamentos nos mesmos. Também contém aplicação de modelos de ML para predição das vendas
- pyproject.toml: arquivo com as dependências do projeto utilizado pelo gerenciador de dependências *poetry*
- poetry.lock: arquivo com as exatas versões utilizadas para cada uma das dependência do projeto utilizado pelo gerenciador de dependências *poetry*

**Dataset utilizado:** https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting/data

**Ferramentas e pacotes utilizados:**
- Gerenciador de dependências: poetry
- Virtualização de ambiente: python venv
- Manipulação de dados: pandas, numpy
- Visualização de dados: seaborn
- Preparação de dados para modelagem: sklearn (MinMaxScaler, OrdinalEncoder)
- Workflow de modelagem: sklearn (TimeSeriesSplit para separação dos dados em função do tempo, Pipeline e ColumnTransformer para evitar data leakage e facilitar reprodução do processo de treinamento, ParameterGrid para busca de hiper-parâmetros)
- Modelagem: sklearn (DecisionTreeRegressor, RandomForestRegressor, AdaBoostRegressor)
- Log de modelos e métricas: mlflow
- Métrica de avaliação: sklearn (mean_squared_error)
