# Projects of Deep Learning Nanodegree by Udacity

## Environment

### Install `GPU` enabled frameworks on Windows

* Installing `pytorch` with `cuda` using `anaconda`

`conda install pytorch torchvision cudatoolkit=10.1 -c pytorch`

* Installing `Tensorflow` with `cuda` using `anaconda`

`conda install -c anaconda tensorflow-gpu`

### Install `GPU` enabled frameworks on Ubuntu 18

* Install the latest `Nvidia` driver via `Software & Updates` app.
* Reboot the system and Activate the conda environment
* Install `pytorch` through `conda install pytorch torchvision cudatoolkit=10.1 -c pytorch` ([pytorch org](https://pytorch.org/))

---

### Test the GPU function

* Run `nvidia-smi` (Ubuntu) to check if the Nvidia driver works well.
* Run the following python script to check if the GPU is available.

```python
import torch
torch.cuda.is_available()
```

```python
import tensorflow as tf
tf.test.is_gpu_available()
```

### References:
* [How to install cuda on Ubuntu 18](https://www.pugetsystems.com/labs/hpc/How-to-install-CUDA-9-2-on-Ubuntu-18-04-1184/) 
* [Install Pytorch Tensorflow GPU on Ubuntu](https://medium.com/@balaprasannav2009/install-tensorflow-pytorch-in-ubuntu-18-04-lts-with-cuda-9-0-for-nvidia-1080-ti-9e45eca99573)

## Projects
### Project 1: Predict Bike Sharing (Simple Neural Network)

`numpy` is used in this project, to be familiar with the mathematics behind Deep Learning

* [Project Folder](./P1_PredictBikeSharing) 

### Project 2: Dog Breed Classifier (Convolutional Neural Network)

* [Project Folder (pytorch)](./P2_DogBreedClassifier/use_pytorch)

### Project 3: Generate TV Script (Recurrent Neural Network)

### Project 4: Generate Faces using Tensorflow (Generative Adversarial Network)

### Project 5: Sentiment Analysis Model

(unfinished)

## Other Projects
For example the projects in the previous version of this Nanodegree

### Project: Image Classification using Tensorflow (CNN)

### Project: Language Translation (RNN)

