## Transfer Learning

Model is trained on one task is reused (partially or fully) for a different but related task

- Why?
    - training model from scratch is an expensive (computation and data) task
    - transfer learning uses pretrained model to improve efficiency and performance
    - example: person who knows how to ride bicycle find it easy to ride motorcycle with the pre known skills like balance and handling


### 2 Step Process:

1) pre-training:
- model is trained on large dataset, model generallizes features
- example: such as edges and shapes in image, syntax and semantics in text

2) fine tuning:
- pre-trained model is trained on different but related dataset
- some layers my not updated while others are finetuned for specific tasks


Example: VGG 16
- Trained on ImageNet (1.4 million images)
- Its learned image features can be transferred to other image classification tasks, such as identifying specific objects or animals.