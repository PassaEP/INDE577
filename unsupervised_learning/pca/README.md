# Principal Component Analysis (PCA)

PCA is a dimensionality reduction technique used to reduce the dimensionality of high-dimensional datasets while preserving most of the important information. It does this by transforming the original features into a new set of orthogonal features called principal components.

## How PCA Works

1. **Standardization**: PCA requires standardizing the features to have a mean of 0 and a standard deviation of 1.
2. **Covariance Matrix**: Compute the covariance matrix of the standardized features.
3. **Eigenvalue Decomposition**: Perform eigenvalue decomposition on the covariance matrix to obtain the eigenvectors and eigenvalues.
4. **Select Principal Components**: Select the top k eigenvectors (principal components) corresponding to the largest eigenvalues.
5. **Transform Data**: Project the original data onto the selected principal components to obtain the lower-dimensional representation.

## Use Cases

- **Dimensionality Reduction**: PCA is commonly used to reduce the number of features in high-dimensional datasets, making them more manageable and improving computational efficiency.
- **Visualization**: PCA can be used to visualize high-dimensional data in lower dimensions (e.g., 2D or 3D) while preserving the most important patterns and relationships.
- **Noise Reduction**: PCA can help remove noise and redundant information from datasets, leading to improved model performance.

## Math Behind PCA

- **Covariance Matrix**: PCA computes the covariance matrix of the standardized features, which represents the relationships between pairs of features.
- **Eigenvalue Decomposition**: PCA decomposes the covariance matrix into its eigenvectors and eigenvalues. Eigenvectors represent the directions of maximum variance, and eigenvalues represent the amount of variance explained along each eigenvector.
- **Projection**: PCA projects the original data onto the selected principal components, transforming the data into a lower-dimensional space while preserving the maximum amount of variance.

Here, we will use PCA to analyze the Wisconsin Breast Cancer dataset. 