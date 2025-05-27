# 2. Experiment tracking and model management

## 2.1 Experiment tracking intro

## 2.2 Getting started with MLflow

In this session, we still use conda to install mlflow. Create (if not already done in last week) and then activate the conda environment for installing packages required.

```sh
conda activate zoomcamp
mamba install mlflow hyperopt xgboost
```

Run the following command to start MLflow with local sqlite backend:

```sh
mlflow ui --backend-store-uri sqlite:////workspaces/mlops-zoompcamp/02-experiment-tracking/mlflow.db
```

## 2.3 Experiment tracking with MLflow

Add the following code segments into any existing code (e.g. Jupyter notebook):

```python
import mlflow

mlfow.set_tracking_uri("sqlite:////workspaces/mlops-zoompcamp/02-experiment-tracking/mlflow.db")
```

Set up an experiment name to capture information across several runs of the same model taining as an experiment, e.g.:

```python
EXPERIMENT_NAME = "taxi-xgboost-experiment"
mlflow.set_experiment(EXPERIMENT_NAME)
```

## 2.4 Model management

## 2.5 Model registry

## 2.6 MLFlow in practice

## 2.7 MLflow: benefits, limitations and alternatives
