# Dog Breed Classification Project

* Please refer to the original Githubs
    * [Dog Project (Pytorch)](https://github.com/udacity/deep-learning-v2-pytorch/tree/master/project-dog-classification)
    * [Dog Project (Keras)](https://github.com/udacity/dog-project)

## Folder Structure
```python
├── use_keras
│   ├── dog_app.ipynb  # main jupyter notebook using Keras
│   └── extract_bottleneck_features.py
└── use_pytorch
    └── dog_app.ipynb  # main jupyter notebook using Pytorch
```

## Environment

* Please refer to the readme file in the master directory.
* Install [`gputil`](https://pypi.org/project/GPUtil/) package 
```
pip install gputil
```

## Problems met

### Training Loss does not converge

* I increased the `batch_size` parameter, then the training converged.
    * When using small value of `batch_size`, the training may be too stochastic,
which means that the model cannot find the correct direction towards the minimum point.
    * But when using GPU with little memory, the `batch_size` cannot be increased too much.
* I reduced the complexity of the training net, so that more memory can be available for more `batch_size`.
