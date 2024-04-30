# Final Project and Implementations for INDE577 

These are implementations of supervised and unsupervised learning from the INDE577 class. The machine learning algorithms implemented in this repository, include:
### Supervised Learning 
- Decision Trees
- Ensemble Learning
- Gradient Descent
- K-Nearest Neighbors
- Linear Regression
- Logistic Regression
- Neural Networks (MLP regression) 
- Perceptron

### Unsupervised Learning
- PCA
- K Means Clustering

## Setup and Environment
It's important to use a virtual environment for many [reasons](https://csguide.cs.princeton.edu/software/virtualenv), and that's what I recommend for running these. I'm using the Anaconda Package Manager, which you can download [here](https://docs.anaconda.com/free/anaconda/pkg-docs/).Specifically, I use miniconda, which is more than enough for my purposes. 

### Packages to install 
Once you have miniconda or anaconda installed, you can install the following packages after you've created the environment by doing the following in the command line. 

`conda create -n [YOUR ENVIRONMENT NAME HERE]` 

`conda init` (if you haven't already)

`conda activate [YOUR ENVIRONMENT NAME HERE]` 

`conda install numpy`
`conda install matplotlib`
`conda install scipy`
`conda install scikit-learn`
`conda install pandas` 
`pip install ucimlrepo` 

### Datasets 
We will use several datasets, including the Seoul Bike Sharing Rental dataset, the Wisconsin Breast Cancer Dataset, and the Dry Bean Dataset. All attributed to their respective authors, but were sourced from the [University of California, Irvine Machine Learning Repository](https://archive.ics.uci.edu/). 

### References

Wolberg,William, Mangasarian,Olvi, Street,Nick, and Street,W.. (1995). Breast Cancer Wisconsin (Diagnostic). UCI Machine Learning Repository. https://doi.org/10.24432/C5DW2B.

Seoul Bike Sharing Demand. (2020). UCI Machine Learning Repository. https://doi.org/10.24432/C5F62R.

Dry Bean. (2020). UCI Machine Learning Repository. https://doi.org/10.24432/C50S4B.

