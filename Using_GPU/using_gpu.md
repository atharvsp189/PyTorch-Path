# Using GPU

In Colab:
set runtime as GPU

1. check GPU:
```
torch.cuda.is_available()
```

2. Move Model to GPU
```
model.to(device)
```

3. Move Batch Features and Batch Labels on GPU:

- change in evaluation loop as well
```
batch_features = batch_features.to(device)
batch_labels = batch_labels.to(device)
```

4. Optimize the GPU usage:
- use larger batch size
- keep pin_memory = True in DataLoader class