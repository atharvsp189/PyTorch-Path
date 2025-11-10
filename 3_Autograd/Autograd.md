# Autograd

- Automatic differentiation tool of PyTorch. provides automatic differentiation for tensor
- as the nested function get complex finding their derivative is a difficult task

### Why to calculate derivative?

x (input) -> w (weight) -> |sigmoid| -> y_pred -> loss

#### Training Process

1. Forward pass computation:
    - linear transformation - z = w*x + b
    - sigmoid function - sigmoid(z) - 1 / (1 + e^(-z))
    - loss function - L

2. Calculate loss:
    - calculate loss function to quantify error

3. Backward pass: 
    - compute gradient of the loss with respect to the parameter

4. Update Gradient:
    - adjust parameter using optimization algorithm

- neural network function as the nested function
- chain rule on a network
    - d(L)/d(y_pred) * d(y_pred)/d(z) * d(z)/d(w)

- when network becomes bigger gradient calculation is complex process
