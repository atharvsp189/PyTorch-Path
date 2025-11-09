# Tensors

### What are Tensors?

> Tensor is specialized multi-dimensional array designed for mathematical and computational of efficiency.

### Type of Tensors

1. 0D tensors:
    - single dot
    - Scalars -single number
2. 1D tensors:
    - Line
    - vectors - sequence or a collection of values
3. 2D tensors:
    - two-dimensional (plane)
    - matriuces - plane (representation of 2D image)
4. 3D tensors:
    - Multi-dimensional vectors
    - cube (repersentaion of RGB image)
5. 4D Tensors:
    - adds extra variable to 2D tensors
    - e.g batch size is added as the additional dimension to 3D data
    - (batch_size * width * length * channels)
6. 5D Tensors:
    - add time dimension for data that changes over time
    - e.g video frames

### Why are Tensors useful?

1. Mathematical Operation:
    - enables efficient computation (addition, multiplication, dot product etc.) for neural netwrork operations

2. Representation of real-world data:
    - complex data such as audio, video, images can be represnted with tensors

3. Efficient Computations:
    - computation can be parallelized with the help of GPU and TPU's
    - crucial for deep learning

### Where are Tensors used in Deep Learning?

1. Data Storage - Training data is stored in tensors
2. weights and biases - can be stroed as tensors
3. Matrix Operations - (w.x + b)
4. Training Process - During forward passes tensors flows through network, Gradients are represented as tensors, are calculated during the backward pass