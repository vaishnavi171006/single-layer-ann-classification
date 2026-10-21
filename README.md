# single-layer-ann-classification
Implementation of a single-layer Artificial Neural Network using Python and NumPy for classification with a sigmoid activation function.
 Single-Layer Artificial Neural Network

## Aim
To build and implement a single-layer Artificial Neural Network (ANN) using Python to solve a simple classification problem.

## Objectives
1. To understand the basic structure and working of a single-layer Artificial Neural Network.
2. To implement a neural network using Python and NumPy.
3. To train the network using input data and predict the class of new data.
4. To evaluate the performance of the network on a simple classification problem.

## Introduction
An Artificial Neural Network (ANN) is a machine learning model inspired by the structure and functioning of the human brain. It consists of interconnected processing units called neurons that process input data and produce outputs.

ANNs learn patterns from training data by adjusting weights and biases.

A single-layer ANN contains an input layer and an output layer, with no hidden layer between them. It is one of the simplest neural network models and provides a foundation for understanding deep learning.

## Theory

### Components of a Single-Layer ANN
1. **Input:** The input features supplied to the network.
2. **Weights:** Values that determine the importance of each input feature.
3. **Bias:** An additional value that helps adjust the neuron's output.
4. **Weighted Sum:** The sum of the products of inputs and their corresponding weights, plus the bias.
5. **Activation Function:** Converts the weighted sum into an output used for classification.
6. **Output:** The predicted class label.

### Mathematical Model

The weighted sum is calculated as:

z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b

Where:
- x represents the input features.
- w represents the weights.
- b represents the bias.
- z represents the weighted sum.

### Sigmoid Activation Function

For binary classification, the sigmoid activation function converts the weighted sum into a value between 0 and 1.

σ(z) = 1 / (1 + e⁻ᶻ)

A threshold of 0.5 can be used to determine the predicted class:
- If the predicted probability is greater than or equal to 0.5, predict class 1.
- Otherwise, predict class 0.

### Learning Process
1. Provide input data to the network.
2. Multiply each input by its corresponding weight.
3. Add the weighted inputs and bias.
4. Apply the activation function to calculate the output.
5. Compare the predicted output with the actual output.
6. Adjust weights and bias to reduce prediction error.
7. Repeat the process over multiple training iterations.
8. Use the trained network to predict new data.

### Loss Function
For binary classification, binary cross-entropy can be used to measure prediction error.

L = −[y log(p) + (1 − y) log(1 − p)]

Where:
- y is the actual class label.
- p is the predicted probability.
- L is the loss.

Gradient descent can be used to minimize the loss by updating the weights and bias.

## Applications
- Spam detection
- Pass/fail prediction
- Basic binary classification
- Pattern recognition
- Classification of simple datasets

## Technologies Used
- Python
- NumPy
- Jupyter Notebook

## Methodology
1. Prepare a dataset containing input features and class labels.
2. Initialize the weights and bias.
3. Calculate the weighted sum of the inputs.
4. Apply the sigmoid activation function.
5. Calculate the prediction error using a loss function.
6. Update the weights and bias during training.
7. Repeat training for multiple iterations.
8. Predict class labels for new input data.
9. Evaluate the model's classification performance.

## How to Run
1. Clone or download this repository.
2. Open `single_layer_ann.ipynb` in Jupyter Notebook.
3. If required, install the libraries using the terminal command:

   `pip install numpy jupyter`

4. Run all notebook cells in order.
5. Observe the training results and predicted class labels.

## Expected Output
The program should demonstrate:
- Training of a single-layer neural network.
- Learning through weight and bias updates.
- Predicted probabilities using the sigmoid function.
- Predicted class labels for input samples.
- Model evaluation results, if evaluation metrics are included in the implementation.

The exact results depend on the dataset, initialization, and training settings.

## Advantages
- Simple to understand and implement.
- Requires relatively few computational resources.
- Useful for learning basic neural network concepts.
- Can solve suitable binary classification problems.

## Limitations
- Does not contain a hidden layer.
- Cannot learn complex nonlinear decision boundaries in its basic form.
- Performance depends on the quality of the training data.
- The basic sigmoid-based model is primarily suited to binary classification.

## Conclusion
This experiment demonstrates the implementation of a single-layer Artificial Neural Network using Python. The network learns from training examples by adjusting weights and bias, applies the sigmoid activation function, and predicts class labels for a simple classification problem.

## License
This project is intended for educational and academic purposes.
