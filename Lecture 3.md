
# Linear Regression


## Linear Regression Model

$$y = f(x) = \sum_{j=1}^{D} w_{j}x_{j} + b$$
- y is the prediction
- w = [w1, w2, ... , $w_{D}$] are the weights
- b is the bias
- w and b together are parameters for the linear regression model

The goal is to choose correct parameter values so that the prediction is close to the target $y \approx t$


## Loss Function

A loss function defines how bad the prediction for y is.

$$\mathbb{L}(y,t) = \frac{1}{2}(y-t)^2$$
where $y-t$ is the residual and we want to make the magnitude small.

## Cost Function

The "badness" of an entire hypothesis is the average badness across our training set.$$\epsilon(w,b) = \frac{1}{N}\sum_{i}\mathbb{L}(y^{(i)},t^{(i)})=\frac{1}{2N}\sum_{i}((w^{(i)})+b) - t^{(i)})^2$$where $y^{(i}) = wx^{(i)} + b$. This is called the cost function of a particular hypothesis.


