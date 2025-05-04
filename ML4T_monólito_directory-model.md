## Modelo de diretório baseado no documento 'ML4T Monólito.pdf'
### Por Miguel R Ferreira F (25/02/24)

O texto abaixo divide o fluxograma disponível no arquivo em pdf chamado 'ML4T Monólito.pdf' em sessões, e designa um modelo com os nomes dos códigos, arquivos e pastas necessários ao funcionamento do algoritmo Monólito.  

***Para uma melhor compreensão, verifique o fluxograma e leia-o em conjunto com este documento.***

Vejamos:

## /feature_engineering:

1. Obtenção de dados
2. Limpeza de dados
3. Visualização

## /alpha_factors:

1. Criação de Alpha Factors
    1. Análise Técnica 
    2. Gerenciamento de Risco
2. Alpha Factors provenientes de notícias analisadas com NLP

## /models:

1. Criação de modelo preditivo
2. Criação de modelo para gestão de capital
3. Criação de modelo para notícias analisadas com NLP

## /order_opening

1. Criação de modelo para abertura de ordem (*Reinforcement Learning*)

## /vectorized_backtesting:

1. Vectorized Backtesting
    1. *VB* para modelo preditivo
    2. *VB* para modelo para gestão de capital
    3. *VB* para modelo de notícias analisadas por NLP
2. *VB* para modelo de abertura de ordem (*Reinforcement Learning*)

## /insfrastructure_codes:

1. Hospedagem, paralelização e distribuição de processamento, escalabilidade e monitoramento

# Modelo principal

Cada sessão será convertida em uma pasta específica. O resultado será semelhante a isso:

    --|/feature_engineering
        --|data_obtention.ipynb
        --|data_cleaning.ipynb
        --|data_visualization.ipynb
    --|/alpha_factors
        --|/alpha_factors_creation
            --|technical_analysis.ipynb
            --|risk_management.ipynb
        --|alpha_factors_nlp-news.ipynb
    --|/models
        --|/base_models_building
            --|forecast_model.ipynb
            --|cap_mangmnt_model.ipynb
            --|nlp_news_models.ipynb
        --|/order_opening_model
            --|rl_order_opening_model   
    --|/vectorized_backtesting
        --|/base_models_vb
            --|forecast_vb.ipynb
            --|cap_mangmnt_vb.ipynb
            --|nlp_news_vb.ipynb
        --|rl_order_opening_model_vb
    --|/infrastructure_codes
        --| ...
        --| ...
    --| ...


## Modelo para diretórios

Além destes arquivos, haverá ainda diretórios avulsos sobre a hospedagem, distribuição de processamento, escalabilidade e monitoramento. Podem assemelhar-se a isto:

    --|/distributed_computing
        --|/tensorflow_distributed
            --|tflow_forecast.ipynb
            --|tflow_cap_mangmnt.ipynb
            --|tflow_nlp_news.ipynb
        --|/ray
            --|ray_forecast.ipynb
            --|ray_cap_mangmnt.ipynb
            --|ray_nlp_news.ipynb
    --|/scaling
    --|/hosting

