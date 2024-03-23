Template
==============================

Template do CookieCutter

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
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
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>


# PROJETO EM ANDAMENTO

Será desenvolvido os seguintes tópicos:

- Responder a pergunta de negócio: Quais seriam os ganhos financeiros com a implementação do modelo que identifica clientes com alta probabilidade de indimplência?
- Tendo em mãos as probabilidades de inadimplência (Logistic Regression / Modelos Arvores): Montar o quadro com dez percentis e avaliar o threshold da probabilidade de operação para aprovação de crédito;
- Tendo em mãos as probabilidades de inadimplência (Logistic Regression / Modelos Arvores): Criar um score de 0 á 1000 de risco de crédito.


# RESULTADOS PARCIAIS

## TESTES DE HIPOTESE A/B - Técnica Bootstrap


H1: A taxa de inadimplência de clientes do sexo Masculino é maior em comparação aos clientes do sexo Feminino - VERDADEIRO  
H2: A taxa de inadimplência de clientes que tem apenas o ensino médio completo é maior em comparação aos outros clientes - VERDADEIRO  
H3: A taxa de inadimplência de clientes com estado civil "Outros" é maior em comparação aos outros clientes - FALSO  
H4: A taxa de inadimplência de clientes com estado civil "Casado" é maior em comparação aos outros clientes - VERDADEIRO  
H5: A taxa de inadimplência de clientes que atrasaram a fatura em 2 meses é maior em comparação aos clientes que não atrasaram - VERDADEIRO  
H6: A taxa de inadimplência de clientes que pagaram o total da fatura e é maior em comparação aos clientes que pagaram parcialmente - VERDADEIRO  


## MODELOS

LGBM  
Recall_0: 0.872030815322063  
Recall_1: 0.5508666164280331  
Acuracia: 0.801  
AUC: 0.7114487158750481  

NEAREST_CENTROID  
Recall_0: 0.8159640487909267  
Recall_1: 0.5772418990203466  
Acuracia: 0.7631666666666667  
AUC: 0.6966029739056365  

LOGISTIC REGRESSION
Recall_0: 0.8159640487909267    
Recall_1: 0.5772418990203466    
Acuracia: 0.7631666666666667    
AUC: 0.6966029739056365    

