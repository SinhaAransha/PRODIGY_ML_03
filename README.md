# Oxford Pets Image Classification

This project implements an image classification model using the **Oxford-IIIT Pet Dataset**. The model is built with TensorFlow and classifies images into one of 37 different pet breeds. It is trained and validated on a split of the dataset using a Convolutional Neural Network (CNN).

## Dataset

The dataset used in this project is the [Oxford-IIIT Pet Dataset](https://www.robots.ox.ac.uk/~vgg/data/pets/), which contains 7,349 images of cats and dogs from 37 different breeds.

### Download Instructions

Download the following files from the dataset page:

- [images.tar.gz](https://www.robots.ox.ac.uk/~vgg/data/pets/images.tar.gz)
- [annotations.tar.gz](https://www.robots.ox.ac.uk/~vgg/data/pets/annotations.tar.gz)

Place both files into a folder named `oxford_pets` in your Google Drive.

## How to Run

Follow these steps in **Google Colab** to train the model:

1. Open Google Colab.
2. Mount Google Drive:

```python
from google.colab import drive
drive.mount('/content/drive', force_remount=True)
Use the full provided script to:

Extract and organize dataset images

Prepare training and validation data

Train a CNN using TensorFlow

Model Architecture
The CNN model includes the following layers:

Input Layer

Convolutional Layers with ReLU Activation

Max Pooling Layers

Flatten Layer

Dense Fully Connected Layers

Softmax Output Layer with 37 Classes

Training Configuration
Input Image Size: 224x224 pixels

Batch Size: 32

Loss Function: Sparse Categorical Crossentropy

Optimizer: Adam

Epochs: 5

License
This project uses the Oxford-IIIT Pet Dataset for educational and research purposes. Refer to the dataset license for more information.
