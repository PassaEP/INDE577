# Ensemble Learning with KNN, MLP, and RF

## Introduction

Ensemble learning is a powerful technique in machine learning where multiple models are combined to improve the overall performance of the system. The idea behind ensemble learning is to leverage the diversity of individual models to collectively make better predictions than any single model alone.

## How Ensemble Learning Works

### Voting-Based Approach

One common approach in ensemble learning is the voting-based method, where predictions from multiple models are combined through a voting mechanism. In this approach, each model in the ensemble provides its prediction for a given input, and the final prediction is determined based on a majority or weighted vote.

### Math Behind Ensemble Learning

Let $ M $ be the number of models in the ensemble, and let $ P_i(x) $ denote the prediction of the $ i $-th model for input $ x $. The final prediction $ P(x) $ of the ensemble is computed as:

$$
P(x) = \text{argmax}_{c} \sum_{i=1}^{M} w_i \cdot \mathbb{1}(P_i(x) = c)
$$

where $ \mathbb{1} $ is the indicator function, and $ w_i $ are optional weights assigned to each model.

## Ensemble Members

In this example, we use three different machine learning models as ensemble members:

1. **K-Nearest Neighbors (KNN)**: A non-parametric classification algorithm that assigns labels to new data points based on the majority class among its $ k $ nearest neighbors.

2. **Multilayer Perceptron (MLP)**: A type of artificial neural network with multiple layers of nodes, capable of learning complex patterns in data.

3. **Random Forest (RF)**: An ensemble learning method based on decision trees, where multiple decision trees are trained on random subsets of the data and their predictions are combined through voting.

Here we use ensemble learning to try to classify the types of beans based on about 17 metrics. 
