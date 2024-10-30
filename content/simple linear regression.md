[[parametric methods]]
simple linear regression is a simple type of [[supervised learning]]. See also [[Regression|regression]].

## notation
$y \approx \beta_{0}+\beta_{1}x$  is the equation for a linear equation. I'll follow An Introduction to Statistical Learning and denote the estimated coefficients by regression as $\hat{y}\approx\hat{\beta_0}+\hat{\beta_1}x$
# least square method
you have a set of labelled data $\{(x_{0},y_0),(x_1,y_1),...(x_n,y_n)\}$. start by randomly assigning the values for $\hat{\beta_0}$ and $\hat{\beta_1}$. 
then calculate the squared error, $e_i$ for the $i$th training sample. $e_{i}= (y_i-\hat{y}_i)^2$. you can sum errors for all $n$ samples which gives you the RSS - residual sum of squares: $\mathrm{RSS} = e_1^2+e_2^2+...+e_n^2$

Equivalently, you can express RSS as $\mathrm{RSS}=\sum\limits_i^n(y-\hat{\beta_0}-\hat{\beta_1}x_i)^2$.

The goal of least square method is to choose $\hat{\beta_0}$ and $\hat{\beta_0}$ which minimizes the RSS. We can minimize the RSS by finding when the function is at a minimum (set derivate to 0).

Start by finding $\dfrac{\partial{S}}{\partial{\hat{\beta_{0}}}}$ and setting it equal to 0
$$\begin{align}
\dfrac{\partial{S}}{\partial \beta_{0}} = 2\sum\limits_i^n(y-\hat{\beta_0}-\hat{\beta_1}x_i)(-1)\\
0 = 2\sum\limits_i^n(y-\hat{\beta_0}-\hat{\beta_1}x_i)(-1)

\end{align}$$
Similarly, $\dfrac{\partial{S}}{\partial{\hat{\beta_{1}}}}$
$$\begin{align}
\dfrac{\partial{S}}{\partial \beta_{0}} = 2\sum\limits_i^n(y-\hat{\beta_0}-\hat{\beta_1}x_i)(-x_i)
\end{align}$$

