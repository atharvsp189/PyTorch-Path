# PyTorch (nn and optim) Module

### torch.nn

torch.nn is a core library provide functionality to help delveloper design and develope neural network efficiently and effectively. It absstract complexity of creating and training neural networks by offering pre-built components such as layers, loss function, optimizer, optimization function and other utilities.  

#### Key Components:

1. Layers:
    - Includes layers like nn.Linear(fully connected layer) and nn.Conv2d (convolutional layer) and nn.LSTM (recurrent layers) and many others

2. Loss Functions:
    - provide loss function to calculate loss such as cross-entropy loss nn.CrossEntropyLoss, MSE loss nn.MSELoss etc.

3. Activation Functions:
    - provide implementation of functions like relu nn.ReLu, sigmoid nn.Sigmoid and tanh nn.Tanh etc.

4. Regularizationa and Dropout:
    - Layers like nn.Dropout and nn.BatchNorm2d to help prevent overfitting and improve model's ability to generalize


### torch.optim

torch.optim provide multiple optimization algorithms used to update the parameters of model during training.  Stochastic Gradient Descent (SGD), ADAM, RMSProp and more