- squared so all error is positive
- why not just use absolute value? this will be tested in my [[ANN in C++]].
- also $x^2$ is differentiable but $\mid x\mid$ is not at $x=0$

$$ \frac{1}{n}\sum_{i}\left((y(i)-a\right)$$
where $a$ is the intended output of some function $y(x)$, and $y(n)$ is the actual output

# Training MSE and Test MSE
usually the MSE is higher for the test cases. 

$$E\left(y_o-\hat{f}(x_o)\right)^{2}= \text{Var}(\hat{f}(x_o))+[\text{Bias}(\hat{f}(x_{o}))]^2+\text{Var}(\epsilon)$$
- you can prove this but I'm feeling lazy right now: [Mean squared error - Wikipedia](https://en.wikipedia.org/wiki/Mean_squared_error#Proof_of_variance_and_bias_relationship) 
- this equation is known as the *bias-variance trade-off*

**Bias** means the error introduced by approximating a (possibly) complicated real-life problem to a simple model. This is like using a linear model for weather predictions; the predictions are *biased* towards a line. Generally, bias decreases as the flexibility increases