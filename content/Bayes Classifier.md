in [[classification]] there's something called the **test error rate**

basically count how many times $y_{i}\neq \hat{y}_i$ (prediction does not match label) and divide by the number of elements in a data set.

$$\frac{1}{n}\sum\limits_{i=0}^{n}I\left(y_i\neq\hat{y}_i\right)$$where $I(y\neq\hat{y})$ returns 1 if $y\neq\hat{y}$ and 0 if not

The Bayes Classifier says that if we want to 
![[Pasted image 20240730165121.png]]

The 