<!-- Tab simulation using details -->
<details open>
<summary>🇧🇷 Português</summary>

# Artigo Científico – Análise Preditiva de Propriedades da Madeira com Espectroscopia NIR Sintética

Este repositório contém o conjunto de dados sintéticos e o código-fonte (notebooks Jupyter) utilizados nas análises apresentadas no artigo científico: **"Análise Preditiva da Densidade e Umidade de Madeiras Tropicais Utilizando Espectroscopia NIR Sintética e Modelos de Regressão"**.

O objetivo deste projeto é demonstrar a viabilidade da aplicação de técnicas de Machine Learning para prever propriedades físico-químicas de madeiras tropicais, utilizando uma base de dados espectrais sintética e robusta, fundamentada em estudos experimentais.

## 🎯 Objetivo do Repositório

Este repositório visa garantir a **reprodutibilidade completa** dos experimentos e análises descritos no artigo científico associado. Ele permite a exploração, validação ou adaptação dos modelos preditivos para densidade e umidade da madeira, e serve como um recurso para pesquisadores interessados na aplicação de aprendizado de máquina à quimiometria e ciência da madeira, particularmente utilizando conjuntos de dados sintéticos.

## 📁 Estrutura do Repositório

-   **`/data/`**: Contém a base de dados sintética.
    -   📄 `base_sintetica_identificacao_madeira.xlsx`: Dataset com 9.999 registros, simulando 11 espécies de madeiras tropicais com suas respectivas propriedades (densidade, umidade) e espectros NIR.
-   **`/notebooks/`**: Contém os notebooks Jupyter com todo o fluxo de análise.
    -   📄 `01_synthetic_data_generation.ipynb`: Código para a geração da base de dados sintética com base nos parâmetros do estudo de referência.
    -   📄 `02_eda_and_dimensionality_reduction.ipynb`: Análise exploratória, pré-processamento (StandardScaler) e redução de dimensionalidade com PCA, incluindo a geração de matrizes de correlação.
    -   📄 `03_regression_model_training_evaluation.ipynb`: Treinamento e avaliação de mais de 20 modelos de regressão para prever a densidade e a umidade.
    -   📄 `04_model_interpretation_with_shap.ipynb`: Análise de interpretabilidade (XAI) do melhor modelo preditivo para densidade utilizando a biblioteca SHAP.
-   **`/figures/`**: Contém as visualizações geradas pelos notebooks.
    -   📄 `heatmap_pca_correlation.png`: Heatmap da matriz de correlação entre propriedades físicas e os componentes principais.
    -   📄 `pca_explained_variance.png`: Gráfico de variância explicada acumulada pelo PCA.
    -   📄 `r2_performance_density.png`: Gráfico de barras comparando o R² dos modelos para predição de densidade.
    -   📄 `r2_performance_humidity.png`: Gráfico de barras comparando o R² dos modelos para predição de umidade.
    -   📄 `shap_summary_plots.png`: Gráficos de importância e distribuição de impacto do SHAP.
-   **`/results/`**: Armazena as métricas de desempenho dos modelos em formato CSV.
    -   📄 `performance_metrics_density.csv`: Métricas (R², MAE, RMSE) para os modelos de predição de densidade.
    -   📄 `performance_metrics_humidity.csv`: Métricas para os modelos de predição de umidade.
-   **`/article/`**: Contém os arquivos-fonte do manuscrito.
    -   📄 `manuscrito.tex`: Código-fonte LaTeX do artigo científico.
    -   📄 `referencias_pt.bib`: Arquivo de bibliografia BibTeX.

## 📝 Observações Metodológicas

-   Todos os dados são **sintéticos**, gerados com base nos parâmetros estatísticos e relações fenomenológicas reportadas no estudo de referência de **Gomes (2024), *Transferência de Calibração para Identificação de Madeiras Tropicais por Espectroscopia NIR Independente da Umidade***.
-   A lógica de geração dos dados buscou refletir as interações físico-químicas plausíveis (e.g., efeito da umidade no espectro, relação da composição com a densidade), mas é, por natureza, uma simulação controlada.
-   As dependências Python necessárias para executar os notebooks estão listadas no arquivo `requirements.txt`.

## 🚀 Como Utilizar

1.  **Clone o repositório:**
    ```bash
    git clone [URL_DO_SEU_REPOSITORIO_GIT]
    cd [NOME_DA_PASTA_DO_REPOSITORIO]
    ```
2.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Execute os notebooks:** Abra os notebooks na pasta `/notebooks/` utilizando Jupyter Lab ou Google Colab para replicar as análises.

## 📄 Como Citar

Se você utilizar este repositório, a base de dados ou os conceitos apresentados no artigo, por favor cite o trabalho original (a citação completa será atualizada após a publicação):

> Brandão Junior, L.C. & Magalhães, R.R. (Ano). Análise Preditiva da Densidade e Umidade de Madeiras Tropicais Utilizando Espectroscopia NIR Sintética e Modelos de Regressão. *Nome do Periódico*, Volume(Edição), Páginas. DOI (se disponível)

## ⚖️ Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE.md).

</details>

<details>
<summary>🇺🇸 English</summary>

# Scientific Article – Predictive Analysis of Wood Properties with Synthetic NIR Spectroscopy

This repository contains the synthetic dataset and source code (Jupyter notebooks) utilized in the analyses presented in the scientific article: **"Predictive Analysis of Density and Moisture Content in Tropical Woods Using Synthetic NIR Spectroscopy and Regression Models"**.

The goal of this project is to demonstrate the feasibility of applying Machine Learning techniques to predict the physicochemical properties of tropical woods, using a robust, synthetic spectral database grounded in experimental studies.

## 🎯 Repository Objective

This repository aims to ensure **full reproducibility** of the experiments and analyses described in the associated scientific article. It allows for the exploration, validation, or adaptation of predictive models for wood density and moisture content, and serves as a resource for researchers interested in applying machine learning to chemometrics and wood science, particularly using synthetic datasets.

## 📁 Repository Structure

-   **`/data/`**: Contains the synthetic dataset.
    -   📄 `base_sintetica_identificacao_madeira.xlsx`: Dataset with 9,999 records, simulating 11 tropical wood species with their respective properties (density, moisture) and NIR spectra.
-   **`/notebooks/`**: Contains the Jupyter notebooks with the entire analysis workflow.
    -   📄 `01_synthetic_data_generation.ipynb`: Code for generating the synthetic dataset based on parameters from the reference study.
    -   📄 `02_eda_and_dimensionality_reduction.ipynb`: Exploratory data analysis, preprocessing (StandardScaler), and dimensionality reduction with PCA, including correlation matrix generation.
    -   📄 `03_regression_model_training_evaluation.ipynb`: Training and evaluation of over 20 regression models to predict density and moisture content.
    -   📄 `04_model_interpretation_with_shap.ipynb`: Interpretable AI (XAI) analysis of the best density prediction model using the SHAP library.
-   **`/figures/`**: Contains visualizations generated by the notebooks.
    -   📄 `heatmap_pca_correlation.png`: Correlation matrix heatmap between physical properties and principal components.
    -   📄 `pca_explained_variance.png`: Cumulative explained variance plot for PCA.
    -   📄 `r2_performance_density.png`: Bar chart comparing the R² scores of models for density prediction.
    -   📄 `r2_performance_humidity.png`: Bar chart comparing the R² scores of models for moisture prediction.
    -   📄 `shap_summary_plots.png`: SHAP feature importance and impact distribution plots.
-   **`/results/`**: Stores model performance metrics in CSV format.
    -   📄 `performance_metrics_density.csv`: Metrics (R², MAE, RMSE) for density prediction models.
    -   📄 `performance_metrics_humidity.csv`: Metrics for moisture prediction models.
-   **`/article/`**: Contains the source files for the manuscript.
    -   📄 `manuscript.tex`: LaTeX source code for the scientific article.
    -   📄 `references_en.bib`: BibTeX bibliography file.

## 📝 Methodological Notes

-   All data are **synthetic**, generated based on the statistical parameters and phenomenological relationships reported in the reference study by **Gomes (2024), *Transferência de Calibração para Identificação de Madeiras Tropicais por Espectroscopia NIR Independente da Umidade***.
-   The data generation logic aimed to reflect plausible physicochemical interactions (e.g., the effect of moisture on the spectrum, the relationship between composition and density) but is, by nature, a controlled simulation.
-   The Python dependencies required to run the notebooks are listed in the `requirements.txt` file.

## 🚀 How to Use

1.  **Clone the repository:**
    ```bash
    git clone [YOUR_GIT_REPOSITORY_URL]
    cd [REPOSITORY_FOLDER_NAME]
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the notebooks:** Open the notebooks in the `/notebooks/` folder using Jupyter Lab or Google Colab to replicate the analyses.

## 📄 How to Cite

If you use this repository, the dataset, or the concepts presented in the article, please cite the original work (full citation will be updated upon publication):

> Brandão Junior, L.C. & Magalhães, R.R. (Year). Predictive Analysis of Density and Moisture Content in Tropical Woods Using Synthetic NIR Spectroscopy and Regression Models. *Journal Name*, Volume(Issue), Pages. DOI (if available)

## ⚖️ License

This project is licensed under the [MIT License](LICENSE.md).

</details>
