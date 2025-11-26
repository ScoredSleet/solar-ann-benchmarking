# Solar Irradiance Assessment AI ☀️🧠

> Avaliação abrangente e comparação de modelos de Redes Neurais Artificiais (ANN) para previsão de irradiação solar em múltiplas zonas climáticas utilizando PyTorch.

Este repositório contém um pipeline completo de **Deep Learning** desenvolvido para prever componentes de irradiação solar (GHI, DNI, DHI, GSR, DSR) com base em dados meteorológicos históricos. O projeto processa dados de diversas fontes (World Bank, TMY, SARAH) e automatiza o treinamento, validação e comparação de arquiteturas MLP em **9 locais distintos** na África.

## 🚀 Funcionalidades

* **Cobertura Geográfica:** Suporte configurado para 9 cidades com diferentes perfis climáticos:
    * **Senegal:** Touba, Fatick
    * **África do Sul:** Northern Cape
    * **República Centro-Africana:** Vakaga
    * **Egito:** Mut
    * **Argélia:** Tamanrasset
    * **Nigéria:** Borno, Abuja, Akure
* **Suporte Multi-Fonte:** Carregadores de dados dedicados para formatos *World Bank*, *TMY* (Typical Meteorological Year) e *SARAH*.
* **Arquitetura Dinâmica:** Configuração flexível de camadas ocultas, neurônios e dropouts específica para cada cidade/alvo.
* **Grid Search Automatizado:** Loop de treinamento que itera sobre otimizadores (`Adam`, `SGD`) e taxas de aprendizado.
* **Pipeline de Avaliação:** Normalização (`StandardScaler`), geração de gráficos comparativos e cálculo de métricas (MAE, RMSE, R²).

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.x
* **Deep Learning:** PyTorch
* **Manipulação de Dados:** Pandas, NumPy
* **Visualização:** Matplotlib
* **Métricas:** Scikit-Learn
* **Exportação:** OpenPyXL

## 📂 Estrutura e Configuração

O núcleo do projeto é controlado pelo dicionário `CIDADES`, que contém a configuração exata para cada local estudado.