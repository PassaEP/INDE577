# Understanding the Math Behind Neural Networks

Neural networks are based on the concept of artificial neurons, which are mathematical models inspired by the behavior of biological neurons in the brain. Let's delve into the mathematical operations performed by neurons in a neural network:

## 1. Linear Transformation

Each neuron in a neural network applies a linear transformation to the inputs it receives. This transformation involves multiplying the input values by corresponding weights and summing the results.

Mathematically, this operation can be represented as:

$$
z = \sum_{i=1}^{n} w_i \cdot x_i + b
$$

where:
- \(z\) is the weighted sum of inputs \(x_i\)
- \(w_i\) are the corresponding weights
- \(b\) is the bias term
- \(n\) is the number of input features

## 2. Activation Function

The output of the linear transformation is then passed through an activation function, which introduces non-linearity into the network. Activation functions allow neural networks to capture complex patterns in data by enabling the modeling of non-linear relationships between input and output variables.

Common activation functions include:
- **Sigmoid**: $$\sigma(z) = \frac{1}{1 + e^{-z}}$$
- **ReLU (Rectified Linear Unit)**: $$ReLU(z) = \max(0, z)$$
- **Tanh (Hyperbolic Tangent)**: $$\text{tanh}(z) = \frac{e^z - e^{-z}}{e^z + e^{-z}}$$

## 3. Loss Function

The output of the neural network is compared to the true labels of the data using a loss function, which measures the difference between predicted and actual values. The goal of training the neural network is to minimize this loss function by adjusting the weights and biases of the network.

Common loss functions for regression tasks include:
- **Mean Squared Error (MSE)**: $$\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2$$
- **Mean Absolute Error (MAE)**: $$\text{MAE} = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$

## 4. Optimization Algorithm

To minimize the loss function and update the parameters (weights and biases) of the neural network, optimization algorithms such as Gradient Descent are used. Gradient Descent iteratively adjusts the parameters in the direction that reduces the loss function.

Mathematically, the weight update rule for Gradient Descent can be expressed as:

$$
w_{i+1} = w_i - \alpha \cdot \frac{\partial L}{\partial w_i}
$$

where:
- $ w_i $ is the current weight
- $(\alpha)$ is the learning rate
- $(\frac{\partial L}{\partial w_i})$ is the gradient of the loss function with respect to the weight

By iteratively adjusting the weights and biases of the neural network based on the gradients of the loss function, neural networks can learn to approximate complex functions and make predictions on new data. This process of learning from data is known as training the neural network.

### Multilayer Perceptron (MLP) Regression

MLP regression is a type of neural network model commonly used for regression tasks, where the goal is to predict continuous-valued outputs. It consists of multiple layers of neurons, including an input layer, one or more hidden layers, and an output layer. Each neuron in the input layer corresponds to a feature of the input data, and neurons in subsequent layers learn increasingly complex representations of the data. The output layer produces the predicted continuous values.

## Problem Statement: Bike Rental Prediction in Seoul

The problem addressed in this project is predicting the number of bikes rented per hour in Seoul based on various factors such as time of day, weather conditions, and calendar information. The dataset includes features such as hour, temperature, humidity, windspeed, visibility, dewpoint, solar radiation, snowfall, rainfall, and whether it was a functioning bike rental day. The objective is to develop a regression model that accurately forecasts bike rental demand, which can be valuable for urban planning and resource allocation.