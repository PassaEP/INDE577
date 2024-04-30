# Logistic Regression for Binary Classification

Logistic regression is a popular algorithm used for binary classification tasks, where the goal is to predict a binary outcome (e.g., yes/no, true/false) based on one or more input features. Despite its name, logistic regression is a classification algorithm rather than a regression algorithm.

## Mathematical Formulation

### Logistic Function (Sigmoid)

The logistic regression model applies the logistic function, also known as the sigmoid function, to the linear combination of input features:

$$
\sigma(z) = \frac{1}{1 + e^{-z}}
$$

where $z = w_0 + w_1x_1 + w_2x_2 + \ldots + w_nx_n$ is the linear combination of input features $x_1, x_2, \ldots, x_n$ weighted by parameters $w_1, w_2, \ldots, w_n$, and $w_0$ is the bias term.

The sigmoid function maps the linear combination $z$ to a value between 0 and 1, representing the probability of the positive class (class 1).

### Decision Boundary

The decision boundary of logistic regression is a hyperplane that separates the feature space into regions corresponding to different class labels. In a binary classification problem, the decision boundary is typically defined as the set of points where the probability of the positive class is 0.5:

$$
\sigma(z) = 0.5
$$

This equation can be solved to find the threshold value of $$ z $$ that separates the classes.

## Training Process

### Cost Function (Cross-Entropy Loss)

Logistic regression is trained using maximum likelihood estimation, where the goal is to maximize the likelihood of observing the training labels given the input features and model parameters. This is equivalent to minimizing the cross-entropy loss function:

$$
J(w) = -\frac{1}{m} \sum_{i=1}^{m} \left( y^{(i)} \log(\hat{y}^{(i)}) + (1 - y^{(i)}) \log(1 - \hat{y}^{(i)}) \right)
$$

where $m$ is the number of training examples, $y^{(i)}$ is the true label of the $ i $$-th example (0 or 1), and $\hat{y}^{(i)}$ is the predicted probability of the positive class for the $i$-th example.

### Optimization

Logistic regression is typically optimized using gradient descent or its variants. The gradient of the cost function with respect to the parameters is computed, and the parameters are updated in the opposite direction of the gradient to minimize the cost.

## Interpretation

### Probability Outputs

One advantage of logistic regression is that it provides probabilistic outputs, allowing for intuitive interpretation of the model predictions. The predicted probabilities can be thresholded to obtain binary class labels based on a chosen decision threshold.

### Coefficients

The coefficients $w_1, w_2, \ldots, w_n$ represent the influence of each input feature on the log-odds of the positive class. Positive coefficients indicate a positive association with the positive class, while negative coefficients indicate a negative association.

## Advantages

- **Interpretability:** Logistic regression provides interpretable coefficients that represent the influence of each feature on the outcome.
- **Efficiency:** Logistic regression is computationally efficient and can handle large datasets with relatively low computational resources.
- **Probabilistic Outputs:** Logistic regression provides probabilistic predictions, allowing for uncertainty quantification and decision threshold tuning.

## Disadvantages

- **Linearity Assumption:** Logistic regression assumes a linear relationship between the input features and the log-odds of the positive class, which may not always hold in practice.
- **Limited Expressiveness:** Logistic regression is limited in its ability to capture complex relationships between features and the target variable compared to more flexible models like neural networks.
- **Feature Engineering Dependence:** The performance of logistic regression heavily depends on feature engineering and selection, requiring domain knowledge and manual intervention.

## Our Problem

Here, we will use logistic regression to classify tumors from the Wisconsin Breast Cancer dataset as benign or malignant. 

