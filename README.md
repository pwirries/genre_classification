# genre_classification
Final Exercise for Udacity Machine Learning Pipelines Course \
The code within this repository is meant to demonstrate an end to end machine learning pipeline using
mlflow, hydra and weights and biases for experiment tracking.

Since the pipeline uses Weights & Biases be sure to login beforehand using ``` wandb.login() ``` \

The pipeline can be ran by calling \
``` mlflow run . ```
from the main directory, or individual steps can be called by overriding the \
hydra option default for "main.execute_step". \
``` mlflow run . -P hydra_options="main.execute_steps=download" ''' \
All default hydra configurations can be overridden in a similar manner.