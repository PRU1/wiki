[[Neural Networks Links]]

la conception est inspirée du fonctionnement des neurones biologiques. C'est une représentation mathématique. Si on met des neurones sur un réseau, on fait



this is interesting:
![[Pasted image 20240513215244.png]]
## Task
The goal is to implement an [[ANN in C++]], and compare its performance to a Python implementation. 

Things I need to learn/review
- [ ] [[Classes in C++]]
- [ ] [[Matrix multiplication]]
- [ ] [[Backpropagation]]
- [ ] [[Gradient Descent]]

# Background

A neural network can be grouped into 3 functions
1. create an actual function that maps inputs with the intended output
2. create a loss function that measures how far away we are from the intended output
3. optimization strategy: figure out how to adjust model parameters to minimize the loss function

# The loss function
- a simple loss function we can use is called [[mean squared error]]