# Optimization to improve performance

#### Reduce Overfitting:

**Possible Soluations:**

1. Adding more data
2. Reducing complexity of NN architecture
3. Regularization:
    - l2 - regularization
    - applied ot penalize the large valur and anocourage smaller, more generalizable weights
    - Loss = Loss + $\lambda \sum_{i=1}^n w_i^2$
    - shrinks the weights during training
    - encourages the network to distribute learning across multiple parameters, avoiding reliance on a few large weights.
    - Active during training only
4. Dropout
    - randomly turning ON/OFF neurons
    - after actiavation function is applied
    - Applied only on hidden layers
    - Active during training only - During evaluation dropout is not used
5. Data Augmentation - (RST, rotate, scale, transformation - Transformations)
6. Batch Normalization
    - Improved training stability
    - During every mini batch activation from previous iterationis normalizes
    - typically applied to hidden layer | Not Output layer
    - after linear layer and before activation
    - Active during training only - During evaluation batch normalization is not used 
7. Early Stopping