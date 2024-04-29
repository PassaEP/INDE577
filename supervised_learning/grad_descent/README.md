### Example of Using Gradient Descent on a Single Variable Function 


Gradient descent is an optimization algorithm commonly used in machine learning to minimize the cost function of a model by iteratively adjusting its parameters. The main idea behind gradient descent is to update the parameters in the direction of the steepest decrease of the cost function.

Here's a summary of how it works:

Initialization: Start with an initial guess for the parameters of the model.
Compute Gradient: Calculate the gradient of the cost function with respect to each parameter. The gradient indicates the direction of the steepest increase of the cost function.
Update Parameters: Adjust the parameters in the opposite direction of the gradient to minimize the cost function. This adjustment is done by taking a step proportional to the negative of the gradient.
Repeat: Iterate steps 2 and 3 until convergence criteria are met, such as reaching a certain number of iterations or when the improvement in the cost function is below a predefined threshold.
Gradient descent comes in different variants, such as batch gradient descent, stochastic gradient descent, and mini-batch gradient descent, each with its own characteristics and trade-offs in terms of convergence speed and computational efficiency.

Here, we juist demonstrate how to do this with simple single-variable and multivariable steps. 