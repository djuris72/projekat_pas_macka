# Dog vs Cat Image Classification 

A simple deep learning project built with PyTorch for classifying images of dogs and cats.

## About the Project

The goal of this project is to train a Convolutional Neural Network (CNN) to distinguish between images of dogs and cats. It serves as an introduction to image classification and computer vision using PyTorch.

The model is trained on labeled images and learns to identify visual patterns that differentiate the two classes.

## Features

- Image classification using a CNN
- Data preprocessing and normalization
- Training and validation workflow
- Loss monitoring during training
- Model saving and loading
- Prediction on custom images

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Pillow
- Jupyter Notebook

## Dataset

The dataset is not included in this repository due to its size.

To run the project, download a Dog vs Cat dataset and organize it in the following structure:

```text
dataset/
├── train/
│   ├── cat/
│   └── dog/
│
└── test/
    ├── cat/
    └── dog/
```

A suitable dataset can be obtained from the Kaggle Dogs vs Cats challenge:

https://www.kaggle.com/c/dogs-vs-cats

After downloading the dataset, place the images in the appropriate folders before running the notebook.

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/dog-cat-classification.git
cd dog-cat-classification
```

Install the required dependencies:

```bash
pip install torch torchvision matplotlib numpy pillow
```

## Running the Project

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
pas_macka.ipynb
```

and run the cells sequentially.

## Model Architecture

The project uses a Convolutional Neural Network consisting of:

- Convolutional layers for feature extraction
- ReLU activation functions
- Max Pooling layers
- Fully connected layers for classification
- Sigmoid output activation for binary classification

## Training

The model is trained using:

- Binary Cross Entropy Loss (BCELoss)
- Adam Optimizer
- Batch training

During training, both training and validation losses are tracked and visualized.

## Saving the Model

After training, the model weights can be saved for future use:

```python
torch.save(model.state_dict(), "pas_macka_model6.pth")
```

## Making Predictions

Once trained, the model can be used to classify new images as either:

- Dog
- Cat

Simply load the saved model and provide an image for prediction.

## Learning Outcomes

This project helped explore:

- Image preprocessing
- Convolutional Neural Networks
- Binary image classification
- Model evaluation
- Deep learning workflows in PyTorch

## Future Improvements

Some possible improvements include:

- Using a larger dataset
- Applying data augmentation
- Adding more convolutional layers
- Experimenting with transfer learning models such as ResNet or MobileNet
- Improving overall classification accuracy
