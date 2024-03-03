# Digit Recognizer MNIST
Welcome to the Digit Recognizer MNIST project! Our primary goal is to develop a system capable of accurately identifying digits from a large dataset of handwritten images. 
Through the exploration of 2D convolutional neural networks (CNNs), we aim to create a robust digit recognition model.


The task involves utilizing two CSV files from the Kaggle competition "Digit Recognizer": https://www.kaggle.com/competitions/digit-recognizer/data  

The training dataset contains 48,000 rows, with each row consisting of an image ID, a label, and 784 pixel values; the test dataset contains 20,000 rows, each comprising 784 pixel values without corresponding labels. 
The objective is to accurately predict the image labels based on the test dataset.  

In order to build a robust digit recognition model we make use of **Convolutional Neural Network (CNN)** model implemented using TensorFlow's Keras API for the purpose of digit recognition.  

The model architecture is as follows:  

Layers:
Two Convolutional Layers:
1st layer: 100 filters, kernel size of (5, 5), ReLU activation function.
2nd layer: 50 filters, kernel size of (5, 5), ReLU activation function.
Flatten Layer: To transform the 2D feature maps into a 1D vector.
Two Dense (Fully Connected) Layers:
1st layer: 128 neurons, ReLU activation function.
2nd layer (Output Layer): 10 neurons with softmax activation for multi-class classification (digits 0-9).
Input Shape: (28, 28, 1) - Corresponding to grayscale images of size 28x28 pixels.
 
