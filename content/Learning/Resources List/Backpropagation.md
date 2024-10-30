[Backpropagation | Brilliant Math & Science Wiki](https://brilliant.org/wiki/backpropagation/)
[[Neural Networks Links]]

- short form for "backpropagation of errors"
- used in supervised learning, specifically gradient descient
- backpropagation uses NN + error function to calculate gradient of error wrt neural network weights+biases
- **goal to find derivative of cost function $\nabla C$**
- "backwards" because gradients calculations go backwards through the network
	- gradient of final layer of weights is calculated first, first layer is calculated last

## formal definition
1) Dataset: consists of input-output pairs of size N. Denoted by $X = \{(\vec{x_1},\vec{y_1}),...,(\vec{x_N}, \vec{y_N})\}$
2) You can do backpropagation in a feedforward neural network
	1) parameters you can tweak: $w_{ij}^k$ : weight between the $j$th node in the $k$th layer and the node $i$ in the $k-1$ layer
	2) You have to have an error/loss function $C(w,b)$ 
cost function: $C(w,b)$ =


```
# headers

[[headers]]

