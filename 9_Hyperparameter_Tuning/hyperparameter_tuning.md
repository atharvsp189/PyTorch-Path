# Hyperparameter Tuning

To know what should be the right architecture
    - number of hidden layers
    - neurons per layer
    - numbe of epoch
    - learning rate
    - batch_size 
    - dropout rate
    - weight decay (lambda) regularization

**Optuna** uses bayesian optimization. hyperparameter tuning library use in machine learning and deep learning. 

Objective Function: 
    - search space
    - model init
    - parameter init
    - training loop
    - evaluation loop
returns accuracy

Study object trail is used as parameter to the objective function.