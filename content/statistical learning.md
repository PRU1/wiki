# introduction
- create an accurate model to predict how one variable affects another (fit a function to data).

we assume there is some relationship between $Y$ and $X=\{X_1,X_2,...,X_p\}$ which can be written as $Y = f(X) + \epsilon$.

## prediction
- $f(X)$ is a function and $\epsilon$ is "random error term"
- the goal is for the sum of all $\epsilon$ for every value of $X$ to be as close to 0 as possible![[Pasted image 20240704114247.png]]
### types of error
1. reducible error
- error you can reduce
you fit arbitrarily fit a curve to a model. there is big error. by changing the curve fit you can reduce the error - reducible error
2. irreducible error
you can't reduce $\epsilon$ (error) any further

example:
$$
\begin{align*}
E(Y-\hat{Y})^{2}&=[(f(X)+\epsilon-\hat{f}(X))]^2\\\\
&=[f(X)-\hat{f}(X)]^{2}+ \text{Var}(\epsilon)
\end{align*}
$$ 
since $\text{Var}(\epsilon)$ is just the sum of all squared error for a set of predictions compared to their expected value.

## inference
- predict the function that maps $X$ to $Y$
difference between prediction and inference: inference figures out a pattern between a dependent and independent variable. prediction guesses output for unseen inputs 

# how to estimate $f$ 
- have training data
training data is data used to make observations and to train a method to estimate $f$

the methods to estimate $f$ are classified as *parametric* or *non-parametric*
![[parametric methods]]

![[non-parametric methods]]