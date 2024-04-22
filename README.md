Deep Learning - Processamento de Redes Reurais
==============================

Esse projeto tem como objetivo fazer a classificação de tendencia de compra e venda, de 4 de ações reais usando Redes Neurais Recorrentes (RNN) ou Redes Neurais Convolucionais (CNN) e faz parte do projeto integrado da disciplina de Deep Learning do curso MBA Data Science & Artificial Intelligence da FIAP. 

• VALE3 – Vale do Rio Doce  
• PETR4 – Petrobras  
• BBAS3 – Banco do Brasil  
• CSNA3 - Companhia Siderúrgica Nacional    

Data:
------------
A partir do dados de fechamento dos ativos e posteriormente normalizados:  

RNN -> Para cada um dos ativos foi fornecido dois arquivos no formato csv, um para treino e outro para testes. Todos conjuntos começam em
janeiro de 2000 e o teste em meados de 2019 até dezembro de 2023.

CNN -> Também foi disponibilizado uma pasta contendo gráficos de barras no
formato de imagem png normalizada dos últimos 15 dias de preços para cada
dia de treino e teste.


How to access:
------------
- É necessário ter instalado: `Python / VS Code`  em sua máquina

**MacOS:**

Crie o ambiente virtual python:
```
python -m venv .venv
```
Ative o ambiente virtual:
```
source .venv/bin/activate
```
Baixe as dependencias para ter acesso ao mesmo ambiente de desenvolvimento: 
```
python -m pip install -r requirements.txt
```


Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    │
    ├── notebooks          <- Jupyter notebooks
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── create_comprehend_role.py <- create a role on AWS 
    └── post_install.py <- install pt_core_news_sm model from spacy


--------