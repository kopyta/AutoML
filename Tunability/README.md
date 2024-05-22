# Tunability of Machine Learning Algorithms
This project showcases the application of advanced hyperparameter tuning methods and provides insights into the tunability of popular machine learning algorithms, to see how their performance would change if the tuning was not tailor-made to the specific data. It was inspired by the paper [Tunability: Importance of Hyperparameters of Machine Learning Algorithms.](https://jmlr.org/papers/volume20/18-444/18-444.pdf).
Team members: Agata Kopyt, Zuzanna Kotlińska

## Objective
The goal of this project is to analyze the tunability of hyperparameters for three selected machine learning algorithms: XGBoost, Random Forest, and Elastic Net. The analysis is conducted on at least four different datasets. Two different hyperparameter sampling techniques are used to tune the models.

## Sampling Methods
The project employs two primary sampling methods for hyperparameter tuning:

1. **Uniform Distribution-Based Sampling**:
   - **Uniform Grid Search**: A systematic search over a pre-defined hyperparameter grid.
   - **Random Search**: Random selection of hyperparameter combinations within a defined grid.
   
   For consistency, the same hyperparameter grid is used across all datasets and algorithms. This grid helps establish a baseline for the best default hyperparameters, which serve as a reference point in the tunability analysis.

2. **Bayesian Optimization**:
   - Techniques such as those provided by the **SMAC3** package or **scikit-optimize's BayesSearchCV** function are used. Bayesian optimization iteratively builds a probabilistic model to identify promising hyperparameter combinations based on past evaluations.

## Experiment Execution
The experimental setup includes the following steps:

1. **Hyperparameter Grid Definition**: Establish a uniform grid of hyperparameters for each algorithm.
2. **Tuning Methods Application**: Apply both uniform and Bayesian optimization techniques to each dataset-algorithm combination.
3. **Default Hyperparameter Identification**: Determine the best default hyperparameters based on initial grid search results.
4. **Comparison and Analysis**:
   - Evaluate the number of iterations required for each method to achieve stable optimization results.
   - Define hyperparameter ranges based on literature and experimental findings.
   - Assess the tunability of each algorithm and specific hyperparameters.
   - Investigate whether the choice of sampling technique introduces any bias in the tunability conclusions.

## Analysis and Results
Key aspects to be analyzed include:

- The stability of optimization results across different sampling methods.
- Hyperparameter ranges and their motivation from existing literature.
- The tunability of algorithms and individual hyperparameters.
- Impact of sampling techniques on the conclusions about tunability.

