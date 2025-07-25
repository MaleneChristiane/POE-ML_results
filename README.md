# POE-ML: An automated Pipeline for Optimization and Evaluation of Machine Learning

*Welcome to the repository associated with the paper of same name: "[POE-ML: An automated Pipeline for Optimization and Evaluation of Machine Learning](https://ieeexplore.ieee.org/document/11015031)". Here experiment settings defined for POE-ML and resulting reports are displayed for the interested reader.*

## Introduction

POE-ML is a Pipeline for Optimizing and Evaluation Machine Learing, and to demonstrate the capabilities of the framework, several experiments (E1, E2a, E2b, E3, E4) was conducted on 4 open-source datasets (D1, D2, D3, D4). The complete experiments settings can be found in the config folder, and likewise the link to each dataset can be found in the dataset descriptions. 

Each experiment has been run through POE-ML, and the performance results are automatically collected within the code-generated PDF files, which can be found the the report folder. 

### Paper abstract

The growing adoption of machine learning has increased the need for automatic, scalable, and flexible pipeline development. However, existing automated machine learning solutions often limit customization and optimization options by hiding pipeline details in experiments. This work presents POE-ML, a Pipeline for Optimization and Evaluation of Machine Learning models that enables dynamic creation and testing of pipelines through experimental configurations. It allows exploring a wide range of models with different hyperparameters for model optimization and producing easily comparable results. To validate its effectiveness, the framework was evaluated using multiple datasets in regression and classification tasks. The results indicated that the proposed framework is both robust and adaptable, and offers a practical solution for optimizing machine learning workflows in various applications.

### Repo structure

The repository is structured as follows: 

```

├── config                          <- Configuring data and experiments
│   │
│   ├── dataset_descriptions.yaml   <- For describing all base datasets (D1, D2, D3, D4)
│   │
│   └── experiments                 <- For configuring experiments
│       │
│       ├── classification_wine_quality        <- Experiments on Wine Quality data (D4)
│       │   ├── config_datasets.yaml    <- Configuring training datasets
│       │   └── config_params.yaml      <- Configuring experiments (E4)
│       │
│       ├── real_estate         <- Experiments on Real Estate data (D3)
│       │   ├── config_datasets.yaml    <- Configuring training datasets
│       │   └── config_params.yaml      <- Configuring experiments (E2b, E3)
│       │
│       ├── traffic_volume      <- Experiments on Traffic Volume data (D2)
│       │   ├── config_datasets.yaml    <- Configuring training datasets
│       │   └── config_params.yaml      <- Configuring experiments (E1, E2a)
│       │
│       └── trees_tetouan_city        <- Experiments on Power Consumption data (D1)
│           ├── config_datasets.yaml    <- Configuring training datasets
│           └── config_params.yaml      <- Configuring experiments (E1)
│
│
├── reports           <- Experiment results
│   │
│   ├── experiments   <- For each experiment
│   │   │
│   │   ├── classification_wine_quality        <- Results from Wine Quality experiments (D4)
│   │   │   └── classification  <- Classification experiment (E4)
│   │   │
│   │   ├── real_estate         <- Results from Real Estate experiments (D3)
│   │   │   ├── MLP             <- The MLP experiment (E3)
│   │   │   └── NN              <- The NN experiment (E2b)
│   │   │
│   │   ├── traffic_volume      <- Results from Traffic Volume experiments (D2)
│   │   │   ├── NN              <- The NN experiment (E21)
│   │   │   └── trees           <- The trees experiment (E1)
│   │   │
│   │   └── trees_tetouan_city        <- Results from Power Consumption experiments (D1)
│   │       └── trees           <- The trees experiment (E1)
│   │
│   └── figures       <- Common for all experiments
│
└── README.md         <- This read-me file
```
