# Neural Network for Digit Recognition (MNIST Dataset)

A simple neural network (built from scratch) to classify handwritten digits using the MNIST dataset. The neural network has an input layer, a hidden layer, and an output layer. The input layer has 784 neurons (28x28 pixels in the image). The hidden layer has 63 neurons, and the output layer has 10 neurons (for each possible digit).

## Libraries Used
numpy
pandas
matplotlib

## Usage
1. Clone the repository.
2. Install the necessary libraries.
3. Run the ntoebook.ipynb file.

## Data
The dataset used is the famous MNIST dataset containing images of handwritten digits. The dataset is split into a training set and a test set. The data is preprocessed by normalizing the pixel values to be between 0 and 1.

## Model Architecture
The model architecture is as follows:
- Input Layer: 784 neurons (28x28 pixels in the image).
- Hidden Layer: 63 neurons.
- Output Layer: 10 neurons (for each possible digit).

## Training
The model is trained using Gradient Descent optimization. The Kaiming initialization method is used to initialize the weights and biases. The activation function used for the hidden layer is the Rectified Linear Unit (ReLU), while the Softmax function is used for the output layer. The learning rate starts at 0.45, and the number of iterations is 100. The learning rate is changed dynamically based on the model's accuracy. The accuracy threshold for changing the learning rate is set at 72%, 81%, and 90%.

## Evaluation
The model's accuracy is evaluated on the test set. The achieved accuracy is printed during training. During training, the accuracy is checked every iteration, and if a specified accuracy threshold is achieved, the learning rate is decreased. The final accuracy achieved on the test set is roundabout 90%.

## References
- [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)
- [Kaiming Initialization](https://arxiv.org/abs/1502.01852)
