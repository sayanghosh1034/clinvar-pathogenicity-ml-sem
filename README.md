Integrative Pathogenicity Prediction Using Machine Learning and Structural Equation Modelling
Overview: This project presents an integrative framework for analyzing and predicting genetic variant pathogenicity using data from the ClinVar database.
The analysis combines exploratory data analysis, feature engineering, dimensionality reduction, unsupervised learning, supervised machine learning, model interpretability, and Structural Equation Modelling (SEM) to investigate both the prediction of pathogenic variants and the relationships between potential pathogenicity mechanisms.

The project is divided into two major analytical components:
Machine Learning Pipeline — prediction and characterization of genetic variant pathogenicity.
Structural Equation Modelling Pipeline — investigation of latent constructs and direct/indirect relationships associated with pathogenicity mechanisms and disease risk.

Research Objective:
The primary objectives of this project are to:
Explore and preprocess ClinVar genetic variant data.
Identify informative features associated with pathogenicity.
Reduce dimensionality and investigate multicollinearity using PCA.
Identify natural patterns in the data using multiple clustering techniques.
Develop and compare multiple supervised machine learning models.
Evaluate model performance using multiple classification metrics.
Investigate feature importance and model interpretability.
Construct latent constructs representing potential pathogenicity mechanisms.
Estimate direct, indirect, and total relationships using Structural Equation Modelling.
Integrate predictive modeling with statistical pathway analysis to obtain a broader understanding of genetic pathogenicity.

Project Architecture
                         ClinVar Genetic Data
                                  │
                                  ▼
                         Data Preprocessing
                                  │
                                  ▼
                         Exploratory Data Analysis
                                  │
                                  ▼
                         Feature Engineering
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
                    ▼                           ▼
                  PCA                     Clustering Analysis
                    │                           │
                    │              ┌────────────┼────────────┐
                    │              ▼            ▼            ▼
                    │             K-Means       GMM      Agglomerative
                    │                                         │
                    │                                    Spectral
                    │                                         │
                    └───────────────┬─────────────────────────┘
                                    ▼
                         Supervised Machine Learning
                                    │
             ┌──────────────┬───────┼────────┬──────────────┐
             ▼              ▼       ▼        ▼              ▼
        Logistic         Decision  Random   XGBoost       CatBoost
        Regression        Tree     Forest
             │              │       │        │              │
             └──────────────┴───────┼────────┴──────────────┘
                                    │
                       SVM / KNN / AdaBoost / ANN
                                    │
                                    ▼
                           Model Evaluation
                                    │
                                    ▼
                     Feature Importance & Interpretation
                                    │
                                    ▼
                        Selected / Derived Variables
                                    │
                                    ▼
                    Structural Equation Modelling
                                    │
                    ┌───────────────┴───────────────┐
                    ▼                               ▼
             Measurement Model              Structural Model
                    │                               │
                    └───────────────┬───────────────┘
                                    ▼
                         Direct & Indirect Effects
                                    │
                                    ▼
                          Pathogenicity Mechanisms      

Results: The project produces two major categories of results.
Machine Learning Results:
Exploratory data analysis
PCA results
Cluster validation
Clustering comparison
Classification performance
Model comparison
Feature importance
Model interpretability

SEM Results:
Latent-variable relationships
Measurement-model results
Structural paths
Path diagrams                 
