ML models were able to automate a lot of stuff
and do a better job than human experts

one thing ML couldn't do --> to see!
- image recognition 
- all ML models are curve fitting models
- pretty much any task can be represented as a curve fitting task
![[Pasted image 20240110200737.png]]
we can't describe an image as a single number
i.e. pixels can be described as 3 numbers RGB 
![[Pasted image 20240110201118.png]]
--> not enough data points? BAD. every time you add a dimensional input, the training data points you need increases by a factor of 9 to have a good enough density for accurate prediction
density of point in space (image linear regression; more points is more accurate. make it 2d and you need more points for the same density)
- have 3x3 patches. Look at each 3x3 patch
- but this may not be small enough to decide what the image is! You may have to look at the entire image
- But looking at the entire image as an input is difficult (too computationally intensive)
- Solution: apply neural network to every patch
- apply another neural network to the output of each patch
![[Pasted image 20240110232447.png]]
each layer looks at larger and larger layers 
do this enough time and the CNN can look at the entire network
average outputs of the final layer to get a prediction.
All the layers are trained at the same time; early layers are not predicting output correctly, they are just useful numbers
Problem: output loses information about the input
will not contain all the information; only a small amount of information gets through a layer --> you are compressing the input dimensions. Every layer has a low dimensional input so you can easily train the network
output contains task relevant information --> compresses input (rewatch video if confused/forget)

- Rearrange input image and you get bad results because CNNs rely on spatial information
![[Pasted image 20240110233104.png]]
EE example: CNN vs deep learning network. CNN is like human! but deep neural network performs better

[What Is a Convolutional Neural Network? | 3 things you need to know - MATLAB & Simulink (mathworks.com)](https://www.mathworks.com/discovery/convolutional-neural-network.html)

convolution: puts input images through convolutional filters, each activates from certain features in the image
ReLU activation --> so output of neuron is between 0 and 1
Pooling: reduces the number of parameters needs to learn with

CNNs can find trends in images. One area it is being used is [[radiology]]. See [[CNN use in radiology]]
