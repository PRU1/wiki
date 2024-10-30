# Implementation

- the implementation from [this tutorial](https://www.jeremyong.com/cpp/machine-learning/2020/10/23/cpp-neural-network-in-a-weekend/) uses [[cross entropy loss]]. Not sure why cross entropy loss is used though
- for linear algebra, use the Eigen library: [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page#Download). Also see [How to add Eigen library to c++ project - Stack Overflow](https://stackoverflow.com/questions/36608986/how-to-add-eigen-library-to-c-project)
	- `git clone https://gitlab.com/libeigen/eigen.git`

# Experiments
- use absolute value for error function instead of [[mean squared error]]
- try out different [[activation functions]] 

# Approach
Take a 28x28 pixel image and flatten it to a 784x1 column vector
