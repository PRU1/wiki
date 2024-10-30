- In an [[artificial neural network]] we need to find the minimum of a cost function (optimization).
- this can be done with [[Gradient Descent|gradient descent]]. 

# the cost function
a common cost function is [[mean squared error]] or [[cross entropy loss]].
$C(w,b) = \sum\limits_x\frac{1}{2n}\bigl|y(x)-a\bigr|^2$, where $y(x)$ is the $x^{\text{th}}$ label in a data set, $n$ is the number of training examples and $a = \sigma(w\cdot x+b)$.

Note: the $\frac{1}{2}$ factor leaves the function cleaner-looking after differentiation
