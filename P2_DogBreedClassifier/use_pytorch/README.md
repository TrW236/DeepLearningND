# Dog Breed Classification Project

## Folder Structure
* `dog_app.ipynb` is the main jupyter notebook of this project.
* The training data and other files are not shared.

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
