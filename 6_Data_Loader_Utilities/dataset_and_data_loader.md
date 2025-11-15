# Dataset & DataLoader Class in PyTorch

### Why?

In **loss calculation**
- using whole data for loss calculation
- not memory efficient
- batch gradient descent
- use mini batch gardient descent(calculate gradient over mini bateches) instead

Problem:
1. No standard interface
2. No easy way to apply transformationn
3. Shuffling and sampling
4. Batch management and parallelization

### Dataset and DataLoader classes

Dataset and DataLoader are core abstraction in pytorch that decouple hwo you define data from how you efficiently iterate over it in training loops

1. Dataset Class:
    - loads the data in memory
    - It is like a blueprint, when the dataset is created you can decide how data is loaded and returned

2. DataLoader Class:
    - wraps a dataset and handles batching, shuffling and parallel loading
    - DataLoader Control Flow:
        - At the start of each epoch, the DataLoader (if shuffle=True) shuffles indices(using a sampler)
        - It divides the indices into chunks of batch_size. for each index in the chunk, data samples are fetched from the Dataset object
        - The samples are then collected and combined into a batch (using collate_fn). The batch is returned to the main training loop

#### Sample

PyTorch provides several predefined samples
1. SequentialSampler;
    - sample sequentially int the order as thery appear dataset (Shuffle = False) 

2. RandomSampler:
    - randomly shuffle the dataset
    - when (Shuffle = True)

We can also specifies according to our usecase for example imbalanced dataset

#### Collate Function

- specifies how to combine the list of samples form dataset into a single batch
- we can also customize our collate function